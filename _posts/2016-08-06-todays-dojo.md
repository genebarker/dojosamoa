---
layout: post
title:  "Today's Dojo"
date:   2016-08-06
category: dojo
author: eugene
---

## Newbies

Good morning. Today is all about improving our PC navigation skills and using the flat screen to work in three dimensions (spatial mapping). A great way to build these skills is to build stuff with virtual Legos!

[Build Academy][1]

Dojo students throw their names in a hat, pair-up, and work through the Build Academy. Students work through each challenge. Once a student completes a challenge, they swap seats with their partner, and the partner completes the same challenge with a different Chrome user. Teamwork!

## Hackers

Level-up time. The fast lane Hackers finish their kata into [Regular Expressions][2] by using their new found skills to solve some fun mind-bending puzzles.

And new Hackers continue their march through the [My First Website][3] kata.

### RegEx Puzzles

It's time to slay regular expressions. Finish these puzzles successfully and a kata badge will be coming your way.

1. Open chrome and go to `http://regexr.com` (type it in the address bar).
2. Click on the `flags` icon (top right) and make sure the following options are selected:
  - global
  - multiline
3. Work through the puzzles below by copying the text into the `Text` area of the RegExr site, and entering a regular expression in the `Expression` line to solve each puzzle.
4. Have fun!

**Tip:** Use the `Cheatsheet` on the left side of the RegExr site to help work through each puzzle.

#### 1. Capture the Numbers

Write a regular expression that captures phone numbers with Samoa's international prefix `+685`. Hint: The `+` is a reserved character, so use an escape (the backslash). 

```text
+64 9 888 777 (NO)
Not this line (NO)
+685 22333 (YES)
+0 800-234-5678 (NO)
+685 7754444 (YES)
+685 22-444 (YES)
```

#### 2. Find ID Numbers

Find ID numbers in text - specifically, a number following the `#` character.

```text
Not this line. (NO)
I like problem #24. (YES)
What a weird # character! (NO)
I have 5 dogs. (NO)
Item #978 rocks! (YES)
This #hashtag is weak. (NO)
```

#### 3. Find Lines that Start with Words

Find lines that start with a word. Hint: Try using an anchor.

```text
Tacos are yummy.
Chillies are hot.
99 cockroaches are in my backpack.
(3) monsters are chasing me.
No 1 found me.
```

#### 4. Find Lines that Start with Capital Letter

Find lines that start with a capital letter. Hint: Try using character range.

```text
I like my CoderDojo! (YES)
dojosamoa.org is our new domain name. (NO)
My mentor made me type this. (YES)
(7) Geckos are on my ceiling. (NO)
```

#### 5. Find Lines that Contain Specific Words

Find lines that contain `apples` or `oranges`. Hint: Try using a capturing group.

```text
I like oranges and popcorn. (YES)
I like candy and popcorn. (NO)
I like apples and popcorn. (YES)
```

[1]: https://www.buildwithchrome.com/buildacademy
[2]: https://en.wikipedia.org/wiki/Regular_expression
[3]: http://kata.coderdojo.com/wiki/My_First_Website