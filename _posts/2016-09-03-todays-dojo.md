---
layout: post
title:  "Today's Dojo"
date:   2016-09-03
category: dojo
author: eugene
---

## Newbies

Today, we take our computational thinking further by working with loops.

[Maze: Loops][1] - Code.org, Course 1, Stage 13

Help the angry bird use **repeat** blocks to get the pigs! See if you can finish each step with a *green* dot - given for successful completion.

As before, our mentors will throw names into a hat, and pair-up the students. One student drives and one navigates. After each step, the students switch roles and work through the same step with a different Chrome user. Then move on to the next step.

## Hackers

We continue working through the [MySQL][2] database Sushi cards, [Beginner Databases][3].

As before, students work in pairs. One drives and one navigates. After each card, the students switch roles and work through the same card using their own database (via the `USE` command we discussed in last week's [dojo][4]). Then move on to the next card.

Below are some MySQL commands that may come in handy as you work through the Sushi cards.

### Rename Database

You want your own database? No problem. There are a couple of ways to do this. The simple / safe way to rename a database is to copy it. For example, let's say I want to change the database name from `CoderDojo` to `Spongebob`:

1. Click the `Shell` button on the XAMPP Control Panel to launch the shell.
2. Backup the database into a file, type `mysqldump -u root CoderDojo > dump.sql`.
3. Now launch the MySQL monitor, type `mysql -u root`.
4. Create your new database, type `create database Spongebob;`.
5. Switch to it, type `use Spongebob;`.
6. Now load it with the backup, type `source dump.sql`.

### Rename Table

To change a table name from `oldname` to `newname` we can use the following command:

```
ALTER TABLE oldname RENAME newname;
```

### Rename Column

Unfortunately, renaming a column forces us to replace it with a new column. For example, if we accidently created the `Cartoons` table with `carton_name varchar(50)`, we would fix it by using the following alter command:

```
ALTER TABLE `Cartoons` CHANGE `carton_name` `cartoon_name` varchar(50);
```

Note how we had to specify all the details for the column we replaced.

[1]: http://studio.code.org/s/course1/stage/13/puzzle/1
[2]: https://en.wikipedia.org/wiki/MySQL
[3]: http://kata.coderdojo.com/wiki/Beginner_Databases
[4]: http://dojosamoa.org/dojo/2016/08/27/todays-dojo.html
