---
layout: post
title:  "Today's Dojo"
date:   2016-08-27
category: dojo
author: eugene
---

## Newbies

Today, it's using computational thinking to draw.

[Artist Sequence][1] - Code.org, Course 1, Stage 8

Help the little kid draw pictures! See if you can finish each step with a *green* dot - given for successful completion.

As before, our mentors will throw names into a hat, and pair-up the students. One student drives and one navigates. After each step, the students switch roles and work through the same step with a different Chrome user. Then switch roles again and move on to the next step.

## Hackers

We continue working through the [MySQL][2] database Sushi cards, [Beginner Databases][3].

### Launching MySQL Monitor

Use the following method to get to the MySQL command line (this replaces Card 1, Steps 8 - 10):

![XAMPP Control Panel](/assets/images/xampp-cpanel.png)

1. Click the `Shell` button on the XAMPP Control Panel to launch the shell.
2. In the shell, type `mysql -u root` then press `[enter]`.

This will start the MySQL monitor where we can interact with the MySQL server. The `-u root` suffix we used gives us `root` authority, full access.

### Pair Programming

If you have a partner, switch seats after your partner finishes a Sushi card. The second partner **must create and use their own database**:

1. In the MySQL monitor, if you haven't already, create your own database: `CREATE database CrazyGene;` (use any name you like).
2. When it is your turn at the keyboard, type: `USE CrazyGene;` (the name you used).
3. If you are the first programmer, type: `USE CoderDojo;` (to use the database we created last week).

[1]: https://studio.code.org/s/course1/stage/8/puzzle/1
[2]: https://en.wikipedia.org/wiki/MySQL
[3]: http://kata.coderdojo.com/wiki/Beginner_Databases
