---
layout: post
title:  "Today's Dojo"
date:   2016-09-10
category: dojo
author: eugene
---

## Newbies

Today, we continue our march through Code.org's first course by using our creativity plus computational thinking to create a story.

[Create a Story][1] - Code.org, Course 1, Stage 16

Time permitting, we'll try to finish the course with Stage 18's artist loops.

[Artist Loops][5] - Code.org, Course 1, Stage 18

As before, our mentors will throw names into a hat, and pair-up the students. One student drives and one navigates. After each step, the students switch roles and work through the same step with a different Chrome user. Then move on to the next step.

## Hackers

Today, we try to finish the [MySQL][2] database Sushi cards, [Beginner Databases][3].

As before, students work in pairs. One drives and one navigates. After each card, the students switch roles and work through the same card using their own database (via the `USE` command we discussed in last week's [dojo][4]). Then move on to the next card.

Below are some MySQL commands that may come in handy today.

### Backup Database

MySQL includes a program called `mysqldump` to create backups. It *dumps* the content of your database into a backup file.

1. Click the `Shell` button on the XAMPP Control Panel to launch the shell.
2. Backup the database into a file, type `mysqldump -u root Spongebob > Spongebob.sql`. (Don't be silly, replace `Spongebob` with the name of *your* database!)

### Restore Database

To restore a database, we create a new database, then load it with the backup `.sql` file we created. This backup file is just a list of SQL commands (just like the ones we type in MySQL monitor).

1. Now launch the MySQL monitor, type `mysql -u root`.
2. Create your new database, type `create database Spongebob;`.
3. Switch to it, type `use Spongebob;`.
4. Now load it with the backup, type `source dump.sql`.

[1]: https://studio.code.org/s/course1/stage/16/puzzle/1
[2]: https://en.wikipedia.org/wiki/MySQL
[3]: http://kata.coderdojo.com/wiki/Beginner_Databases
[4]: http://dojosamoa.org/dojo/2016/08/27/todays-dojo.html
[5]: http://studio.code.org/s/course1/stage/18/puzzle/1
