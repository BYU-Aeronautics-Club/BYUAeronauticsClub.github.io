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
First things first, you'll need to get familiar with Markdown syntax, which is what almost all of these pages are written in.  It's pretty easy, actually. Just go ahead and complete a tutorial like [markdowntutorial.com](https://www.google.com/search?q=markdown+tutorial&rlz=1C5CHFA_enUS705US705&oq=markdown+tutorial&aqs=chrome.0.69i59j69i57j69i60l4.1839j0j9&sourceid=chrome&ie=UTF-8), or find a [markdown cheat sheet](https://www.google.com/search?safe=active&rlz=1C5CHFA_enUS705US705&sxsrf=ACYBGNSGWnGGLLpeBiFetZKDb-TNLFU9VQ%3A1579216137828&ei=Ce0gXuWVMsrH-gT0qKHQAQ&q=markdown+cheat+sheet&oq=markdown+cheat+sheet&gs_l=psy-ab.3..35i39j0l9.3941.3941..4521...0.1..0.93.93.1......0....2j1..gws-wiz.......0i71.WiUTo0b6wFg&ved=0ahUKEwilvqzHnonnAhXKo54KHXRUCBoQ4dUDCAs&uact=5) with all the basics.

### Git a github account

If you don't already, go get a [github account](https://github.com/). You can also register for the [student account](https://education.github.com/pack). An account is free, and the student account gives you a few more freebies.

After you've registered for an account, let the repository owner know your github username and s/he will be able to give you access to add and modify files to the website repository.

### Learn how to use git

You need to learn how to use git too; but don't worry, it's pretty easy. If you've got a Mac or Linux computer, or if you use PowerShell on Windows, it's an inherent feature. [Go ahead and learn](https://try.github.io/) how to clone, add, commit, pull, push, and also how to create branches. That's about all you need to know for the basics.

Now you just need to clone the  [BYU-Aeronautics-Club.github.io repository]([BYU-Aeronautics-Club.github.io](https://github.com/BYU-Aeronautics-Club/BYU-Aeronautics-Club.github.io) and get going!

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

Now that it's all pushed and in the repo for everyone to see, your page still isn't on the website. Never fear, however, you're on the final step. You need to submit a pull request.  You can do that on github.com in the repository. [This Link](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request) has a pretty good explanations of how to do that (it is official after all).  After you've submitted your request, the repository owner can go in, merge your branch into master, and your page will be up and running! Congrats!