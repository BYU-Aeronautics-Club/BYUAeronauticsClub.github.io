---
permalink: /tutorials/addingsitecontent/
title: "Adding Content to the Club Website"
layout: single
---

Are you a member of the BYU Aeronautics Club? Have you been given an assignment to create a tutorial and add it to the website? Are you confused as to how to go about making that happen? Did someone in the club point you to this page? If you answered yes to any of these questions, you're most likely in the right place.  Let's figure out the easiest way to start adding tutorials to the club website.

## Adding Tutorials

### Learn Markdown
First things first, you'll need to get familiar with Markdown syntax, which is what almost all of these pages are written in.  It's pretty easy, actually. Just go ahead and complete a tutorial like [markdowntutorial.com](https://www.markdowntutorial.com/), or find a [markdown cheat sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#links) with all the basics.

### Git a github account

If you don't already, go get a [github account](https://github.com/). You can also register for the [student account](https://education.github.com/pack). An account is free, and the student account gives you a few more freebies.

After you've registered for an account, let the repository owner know your github username and s/he will be able to give you access to add and modify files to the website repository.

### Learn how to use git

You need to learn how to use git. It's easy. If you've got a Mac or Linux computer, or if you use PowerShell on Windows, it's an inherent feature. [Go ahead and learn](https://try.github.io/) how to clone, add, commit, pull, and push, oh, and creating branches. That's about all you need to know for the basics.

Now you just need to clone the  [BYU-Aeronautics-Club.github.io repository]([BYU-Aeronautics-Club.github.io](https://github.com/BYU-Aeronautics-Club/BYU-Aeronautics-Club.github.io)) and get going!

### Create a branch

After you've cloned the repository, you need to make a branch. This helps things function smoothly and keeps people out of each other's way.
In case you didn't see this when you were learning git, you can create and switch to a new branch in the repository like this:

```git checkout -b branch_name```

where branch_name has no spaces, and is whatever you want to call your branch (probably the name of the tutorial). Now you can do all the adding and committing you want without bothering anyone else.

### Make a page

You'll find a [_pages](https://github.com/BYU-Aeronautics-Club/BYU-Aeronautics-Club.github.io/tree/master/_pages) directory in the website repository. Inside that directory, there is a [tutorials](https://github.com/BYU-Aeronautics-Club/BYU-Aeronautics-Club.github.io/tree/master/_pages/tutorials) subdirectory. You should add your file there.  It should be named name_of_tutorial.md, where you pick what your tutorial name is.  Then add all the content you want to the file and save it.

Also note that if you're adding figures to your page, you'll need to add the figures to the [figures](https://github.com/BYU-Aeronautics-Club/BYU-Aeronautics-Club.github.io/tree/master/_pages/tutorials/figures) subdirectory within the tutorials directory.

##### VERY IMPORTANT
In order to make your page show up you need to add a specific header to your file of the form

    ---
    permalink: /tutorials/pagefilename/
    title: "Title to Put on Page"
    layout: single
    ---

### Make the page accessible

You'll probably want to make sure everyone can find your new page, so go ahead and find the tutorials.md file in the [_pages](https://github.com/BYU-Aeronautics-Club/BYU-Aeronautics-Club.github.io/tree/master/_pages) directory. Right now we just have a basic list of the tutorial pages, so add a link formatted like the others in that file. (Pay special attention to the relative paths format, and make sure it matches your file header.) After you've saved your files, go ahead and add, commit, and push them.

Note that when you're first pushing your new brach, you'll have to use a slightly different syntax so that git knows what you're doing. Use this command:

``` git push -u origin branch_name```

### Create a Pull request

Now that it's all pushed and in the repo for everyone to see, your page still isn't on the website. Never fear, however, you're on the final step. You need to submit a pull request.  You can do that on github.com in the repository. [This Link](https://yangsu.github.io/pull-request-tutorial/) and [This Link](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request) have pretty good explanations of how to do that.  After you've submitted your request, the repository owner can go in, merge your branch into master, and your page will be up and running! Congrats!