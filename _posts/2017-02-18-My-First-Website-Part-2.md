---
layout: post
title:  "My First Website Part 2"
date:   2017-02-18
category: dojo
author: eugene
---

## 1. Update your Repository

Last week you setup your own exact copy of the dojo's repository. At the start of each session you need to pull in the latest updates (i.e. this week we added notes).

1. Open _Git Bash_ (use Windows button on bottom left).  
    ![Find Git Bash](/assets/images/launch-git-bash.png)
2. Go to your repository's directory in the file system:  
    `$ cd Documents/workspace/dojo2017q1`  
    _Tip:_ Type first few characters of directory name, then use the  
    tab key.
3. Check the status of the repository:  
    `$ git status` (note the selected branch)
    ![Check Repo Status](/assets/images/git-status-output.png)
4. Checkout the `master` branch:  
    `$ git checkout master`
5. Get the latest updates:  
    `$ git pull origin master`  
    Git pulls an *exact* copy of all the changes that occurred since  
    your last pull from the server!  
    ![Pull Latest Updates](/assets/images/git-pull-output.png)
6. Now switch back to our personal branch created last week (remember to use your own name in-place of `elvis`):  
    `$ git checkout elvis`
7. Now merge in the latest updates from the master branch:  
    `$ git merge master`  
    Git merges-in the latest updates from the master into your branch!  
    ![Merge Updates into Your Branch](/assets/images/git-merge-output.png)
8. Your branch is now up-to-date with dojo's master repository!

## 2. Do Some Coding

Using the handout from your mentor, start with Card 1. There is a copy in the repository named `My_first_website.pdf`, also available online [here][1].

## 3. Save Your Work

At the end of class, we need to save our work. This is easy in Git!

1. Open _Git Bash_ (use Windows button on bottom left).
2. Go to your repository's directory in the file system:  
    `$ cd` (make sure we're in the home directory)  
    `$ cd Documents/workspace/dojo2017q1`
3. Review the files that have changed:  
    `git status`  
    ![Check Branch Changes](/assets/images/git-status-changes.png)
4. Stage your files for commit:  
    `git add --all`  
    `git status` (notice that your files are staged, in-green)
5. Now commit (save) your changes:  
    `git commit -m 'My first commit!'`
6. And push them to the server (replace `elvis` with your branch name):
    `git push origin elvis`
7. Done!


[1]: http://kata.coderdojo.com/images/c/c0/My_first_website.pdf
