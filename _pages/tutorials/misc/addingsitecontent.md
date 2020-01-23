---
permalink: /tutorials/misc/addingsitecontent/
title: "Adding Content to the Club Website"
layout: single
sidebar:
    nav: "tutorials"
---

Are you a member of the BYU Aeronautics Club? Have you been given an assignment to create a tutorial and add it to the website? Are you confused as to how to go about making that happen? Did someone in the club point you to this page? If you answered yes to any of these questions, you're most likely in the right place.  Let's figure out the easiest way to start adding tutorials to the club website.

## Adding Tutorials

### Learn Markdown
First things first, you'll need to get familiar with Markdown syntax, which is what almost all of these pages are written in.  It's pretty easy, actually. Just go ahead and complete a tutorial like <a href="https://www.markdowntutorial.com/" target="_blank">markdowntutorial.com</a>, or find a <a href="https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet" tarket="_blank">markdown cheat sheet</a> with all the basics.

### Git a github account

If you don't already, go get a <a href="https://github.com/" target="_blank">github account</a>. You can also register for the <a href="https://education.github.com/pack" target="_blank">student account</a>. An account is free, and the student account gives you a few more freebies.

After you've registered for an account, let the repository owner know your github username and s/he will be able to give you access to add and modify files to the website repository.

### Learn how to use git

You need to learn how to use git too; but don't worry, it's pretty easy. If you've got a Mac or Linux computer, or if you use PowerShell on Windows, it's an inherent feature. <a href="https://try.github.io/" target="_blank">Go ahead and learn</a> how to clone, add, commit, pull, push, and also how to create branches. That's about all you need to know for the basics.

Now you just need to clone the <a href="https://github.com/BYU-Aeronautics-Club/BYU-Aeronautics-Club.github.io" target="_blank">BYU-Aeronautics-Club.github.io</a> and get going!

### Create a branch

After you've cloned the repository, you need to make a branch. This helps things function smoothly and keeps people out of each other's way.
In case you didn't see this when you were learning git, you can create and switch to a new branch in the repository like this:

```git checkout -b branch_name```

where branch_name has no spaces, and is whatever you want to call your branch (probably the name of the tutorial). Now you can do all the adding and committing you want without bothering anyone else.

### Make a page

You'll find a <a href="https://github.com/BYU-Aeronautics-Club/BYU-Aeronautics-Club.github.io/tree/master/_pages" target="_blank">_pages</a> directory in the website repository. Inside that directory, there is a <a href="https://github.com/BYU-Aeronautics-Club/BYU-Aeronautics-Club.github.io/tree/master/_pages/tutorials" target="_blank">tutorials</a> subdirectory. You should add your file there.  It should be named name_of_tutorial.md, where you pick what your tutorial name is.  Then add all the content you want to the file and save it.

Also note that if you're adding figures to your page, you'll need to add the figures to the <a href="https://github.com/BYU-Aeronautics-Club/BYU-Aeronautics-Club.github.io/tree/master/_pages/tutorials/figures" target="figures">_pages</a> subdirectory within the tutorials directory.

##### VERY IMPORTANT
In order to make your page show up you need to add a specific header to your file of the form

    ---
    permalink: /tutorials/path_to_tutorial/
    title: "Title to Put on Page"
    layout: single
    sidebar:
        nav: "tutorials"
    ---

### Make the page accessible

You'll probably want to make sure everyone can find your new page. This is a little bit tricky, so pay attention to this part.  You'll have noticed the sidebar navigation on the left hand side of the tutorials pages. This comes from the sidebar part of the header. As long as you use the header template above, you should be fine. Unfortunately, that's not all that is required.

Next, you'll need to navigate to the _data/navigation.yml file (_data/ is in the root directory). Inside, you'll need to find the tutorials: section and then add your page into the navigation where it goes.  For example, if you've got a miscellaneous tutorial on how to put tutorials on the website, you'd add something like

      - title: "Miscellaneous"
        children:
        - title: "Adding Tutorials"
          url: /tutorials/misc/addingsitecontent/

in a reasonable spot in the lineup. You may consider asking the repository owner where the best place to put this would be.

After all of that, you're ready to add, commit, and push your branch. Note that when you're first pushing your new brach, you'll have to use a slightly different syntax so that git knows what you're doing. Use this command:

``` git push -u origin branch_name```

### Create a Pull request

Now that it's all pushed and in the repo for everyone to see, your page still isn't on the website. Never fear, however, you're on the final step. You need to submit a pull request.  You can do that on github.com in the repository. <a href="https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request" target="figures">This Link</a> has a pretty good explanations of how to do that (it is official after all).  After you've submitted your request, the repository owner can go in, merge your branch into master, and your page will be up and running! Congrats!