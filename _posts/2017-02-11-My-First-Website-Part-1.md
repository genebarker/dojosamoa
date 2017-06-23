---
layout: post
title:  "My First Website Part 1"
date:   2017-02-11
category: dojo
author: eugene
---

## Install Git

We'll be using [Git][1], the world's most advanced and popular source code management system (SCM). An SCM is a handy tool to hold our files and track their changes.

1. Download latest version of [Git for Windows][2].
2. Install Git; use and accept the default options.
3. Open _Git Bash_ (use Windows button on bottom left).  
    ![Find Git Bash](/assets/images/launch-git-bash.png)
4. Create a directory for this laptop's SSH key:  
    `$ cd` (make sure we're in the home directory)  
    `$ mkdir .ssh`
5. Insert flash drive from your mentor into your laptop's USB port AND **get the drive letter it's assigned** (it will appear on bottom right).  
    ![Get the Drive Letter](/assets/images/usb-drive-letter-popup.png)
6. Ask your mentor for the laptop's key number is (i.e. `04`).
7. Copy the laptop's private SSH key from the flash drive using the drive letter you noted in Step 5 and the key number you were given in Step 6. For example, for drive `F` and key `04` the command is:  
    `$ cp /f/dojo/keys/key04-id_rsa .ssh/id_rsa`  
    (remember to use the drive letter and key number in-place of `f` and `04`)
8. Copy the laptop's public SSH key using the same method. Example:  
    `$ cp /f/dojo/keys/key04-id_rsa.pub .ssh/id_rsa.pub`  
    (note the `.pub` file extension for *public*)
9. Ask your mentor for the laptop's unique name (i.e. coderdojo-7). There should be no spaces!
10. Set your laptop's name and email in Git:  
    `$ git config --global user.name "coderdojo-7"`  
    `$ git config --global user.email coderdojo-7@example.com`

## Get the Code

We need a copy of our files so that we can get coding!

1. If not already open, open _Git Bash_ (use Windows button on bottom left).
2. Change to the *Documents* directory in Windows:  
    `$ cd` (make sure we're in the home directory)  
    `$ cd Documents`
3. Create a directory named *workspace* for our work:  
    `$ mkdir workspace` (make it!)  
    `$ cd workspace` (change to it)
4. Enter command to clone our dojo's repository for My First Website:  
    `$ git clone ssh://ninja@go.dojosamoa.org:4422/~/repo/dojo2017q1.git`
5. Verify that the host fingerprint matches that shown in image below, then answer by typing: `yes`  
    ![Verify Host](/assets/images/git-fingerprint.png)
6. Git will now securely download an *exact* copy of the repository to your machine. The output should be similar to that shown in the image below.  
    ![Cloning Output](/assets/images/git-cloning-output.png)
7. Change to the directory for the repository and check it:  
    `$ cd dojo2017q1`  
    `$ git status`
8. Create a *branch* using your own name (no spaces!) for your work:  
    `$ git checkout -b elvis` (replace `elvis` with your name)  
    `$ git status`
9. You're now working in your very own area of the repository. Time to code!

## Start Coding

Using the handout from your mentor, start with Card 1. There is a copy in the repository named `My_first_website.pdf`, also available online [here][3].


[1]: https://git-scm.com
[2]: https://git-scm.com/download/win
[3]: http://kata.coderdojo.com/images/c/c0/My_first_website.pdf
