---
layout: post
title:  "My First Website Part 4 Plus"
date:   2017-03-04
category: dojo
author: eugene
---

For the remainder of the the _My First Website_ kata, we'll be using the
following process to load and save our code.

## 1. Pull Changes from Server

1. Open _Git Bash_.
2. Change to your repository's directory.  
    `$ cd` (make sure we're in the home directory)  
    `$ cd Documents/workspace/dojo2017q1`
3. Checkout the master branch - where your mentor makes updates for  
   everyone (notes, images, etc.).  
    `$ git checkout master`
4. Pull the latest changes from the server to your local copy.  
    `$ git pull origin master`  
    ![Git Pull Master](/assets/images/git-pull-origin-master.png)
5. Now checkout your own branch.  
    `$ git checkout elvis` (replace `elvis` with your branch name)
6. Pull your latest code from the server to this laptop, *because* you
   probably used a different laptop last week.  
    `$ git pull origin elvis` (replace `elvis` with your brach name)
7. And merge in the latest updates from your mentor in the `master`
   branch.  
    `$ git merge master`
8. If a *Merge* message pops-up like that shown, we'll just accept the
   default message.  
    ![Merge Message](/assets/images/git-merge-message-in-vi.png)  
   The message is displayed in an *old fashioned* editor named *VI*.
   We'll learn more about *VI* in another kata. For now, let's just
   accept this message and type in the following exactly:  
    `:wq`  
   then press `[enter]`. If the letters don't appear at the bottom of
   the screen as you type them, press the `[esc]` key, then try again.
9. Done!

## 2. Do Some Coding

Continue your work on the _My First Website_ kata. Get a physical copy
from your mentor. Optionally, you can check out the copy in your
repository named `My_first_website.pdf` or download it [here][1].

## 3. Push Your Changes to Server

1. Open _Git Bash_ (if still open from earlier, go to step 3).
2. Change to your repository's directory.  
    `$ cd` (make sure we're in the home directory)  
    `$ cd Documents/workspace/dojo2017q1`
3. Review the files that have changed:  
    `git status`  
    ![Check Branch Changes](/assets/images/git-status-changes.png)
4. Stage your files for commit:  
    `git add --all`  
    `git status` (notice that your files are staged, in-green)
5. Now commit your changes with a message to help your remember the work you performed today:  
    `git commit -m 'Finished card 3 today!'`  
    (replace the message in quotes after the `-m` with your own!)
6. And push them to the server (replace `elvis` with your branch name):
    `git push origin elvis`
7. Done!


[1]: http://kata.coderdojo.com/images/c/c0/My_first_website.pdf
