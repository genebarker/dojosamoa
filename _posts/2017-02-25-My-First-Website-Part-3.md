---
layout: post
title:  "My First Website Part 3"
date:   2017-02-25
category: dojo
author: eugene
---

## 1. Move workspace to Documents

To make things easier when working with Windows, we need to make sure our `workspace` folder (directory) is in your Windows `Documents` folder.

1. Open _Git Bash_ (use Windows button on bottom left).  
    ![Find Git Bash](/assets/images/launch-git-bash.png)
2. List the contents of your home directory.  
    `$ ls`
3. Check if your `workspace` folder is listed.  
    ![Find Workspace Folder](/assets/images/git-ls-output.png)
4. If listed, move it to Documents via the following command:  
    `$ mv workspace Documents`
5. Done!

## 2. Pull Repository Changes from Server

From now on, repeat this step at the start of every dojo. By using this method, you can use any laptop from week-to-week and not lose any of your work. It's how professional developers (programmers) work with their code. So why not us!

1. Open _Git Bash_.
2. Change to your repository's directory.  
    `$ cd` (make sure we're in the home directory)  
    `$ cd Documents/workspace/dojo2017q1`
3. Checkout the master branch.  
    `$ git checkout master`
4. Pull the latest changes from the server to your local copy.  
    `$ git pull`  
    ![New Branches](/assets/images/git-pull-new-branches.png)
5. Now checkout (switch) to your own branch.  
    `$ git checkout elvis` (replace `elvis` with your branch name)
6. And merge in the updates your mentor made to the `master` branch.  
    `$ git merge master`  
    ![Merge in Changes](/assets/images/git-merge-master.png)
7. If a *Merge* message pops-up like that shown, we'll just accept the
   default message.  
    ![Merge Message](/assets/images/git-merge-message-in-vi.png)  
   The message is displayed in an *old fashioned* editor named *VI*.
   We'll learn more about *VI* in another kata. For now, let's just
   accept this message and type in the following exactly:  
    `:wq`  
   then press `[enter]`. If the letters don't appear at the bottom of
   the screen as you type them, press the `[esc]` key, then try again.
8. Done!

## 3. Do Some Coding

This week, we are moving-on to Card 2 of the _My First Website_ kata. Get a physical copy from your mentor. Optionally, you can check out the copy in your repository named `My_first_website.pdf` or download it [here][1].

## 4. Push Repository Changes to Server

From now on, repeat this step at the end of every dojo. This will save all of your work on the server.

1. Open _Git Bash_.
2. Change to your repository's directory.  
    `$ cd` (make sure we're in the home directory)  
    `$ cd Documents/workspace/dojo2017q1`
3. Review the files that have changed:  
    `git status`  
    ![Check Branch Changes](/assets/images/git-status-changes.png)
4. Stage your files for commit:  
    `git add --all`  
    `git status` (notice that your files are staged, in-green)
5. Now commit (save) your changes, place a message to help your remember the work you performed today:  
    `git commit -m 'Finished card 3 today!'` (replace message in quotes with your own)
6. And push them to the server (replace `elvis` with your branch name):
    `git push origin elvis`
7. Done!


[1]: http://kata.coderdojo.com/images/c/c0/My_first_website.pdf
