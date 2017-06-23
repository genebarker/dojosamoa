---
layout: post
title:  "My First Website Part 5 Plus"
date:   2017-03-25
category: dojo
author: eugene
---

This is an *improved* version of our process for working on the
_My First Website_ kata. We use this process to make sure we don't lose
our work.

## 1. Pull Changes from Server

1. Open _Git Bash_.
2. Change to your repository's directory.  
    `$ cd` (make sure we're in the home directory)  
    `$ cd Documents/workspace/dojo2017q1`
3. Check if local repository is clean.  
    `$ git status`  
    ![Clean Repository](/assets/images/git-status-clean.png)
4. If the last two lines of the command's output matches the example
   above, skip to Step 6.
5. Uh-oh, someone did not save their work and left the repository
   dirty. Let's disregard all the un-pushed changes (make sure you use
   the current branch name, not elvis).  
    `$ git reset --hard origin/elvis`
6. Pull the latest changes from the server to your local copy.  
        `$ git pull origin`  
        ![Git Pull Origin](/assets/images/git-pull-origin.png)
7. Now checkout your own branch.  
    `$ git checkout elvis` (replace `elvis` with your branch name)
8. Make sure the local copy is up-to-date with the server's.  
    `$ git pull`
9. Now merge in the latest updates from your mentor in the `master`
   branch.  
    `$ git merge master`
10. If a *Merge* message pops-up like that shown, we'll just accept the
   default message.  
    ![Merge Message](/assets/images/git-merge-message-in-vi.png)  
   The message is displayed in an *old fashioned* editor named *VI*.
   We'll learn more about *VI* in another kata. For now, let's just
   accept this message and type in the following exactly:  
    `:wq`  
   then press `[enter]`. If the letters don't appear at the bottom of
   the screen as you type them, press the `[esc]` key, then try again.
11. Done! Minimize the _Git Bash_ window.

## 2. Do Some Coding

Continue your work on the _My First Website_ kata. Get a physical copy
from your mentor. Optionally, you can check out the copy in your
repository named `My_first_website.pdf` or download it [here][1].

## 3. Push Your Changes to Server

1. Re-select the _Git Bash_ window.
2. Review the files that have changed:  
    `git status`  
    ![Check Branch Changes](/assets/images/git-status-changes.png)
3. Stage your files for commit:  
    `git add --all`  
    `git status` (notice that your files are staged, in-green)
4. Now commit your changes with a message to help your remember the work
   you performed today:  
    `git commit -m 'Finished card 3 today!'`  
    (replace the message in quotes after the `-m` with your own!)
5. And push them to the server (replace `elvis` with your branch name):  
    `git push origin elvis`
6. Done!


[1]: http://kata.coderdojo.com/images/c/c0/My_first_website.pdf
