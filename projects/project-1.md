---
layout: project
type: project
image: images/micromouse.jpg
title: Morse Code
permalink: projects/micromouse
# All dates must be YYYY-MM-DD format!
date: 2019-03-12
labels:
  - C
  - C++
summary: I developed a program that would translate Morse Code into English.
---

One of the assignments for my ICS 212 course had me create a program that could accurately translate a phrase in Morse Code into the English equivalent. The purpose of the assignment was to learn how to take inputs from the command line as well as be able to compare the input string to morse. 

The most difficult part of the task was to compare the input string with the Morse Code library within the program. It forced me to get used to methods such as strcmp (string compare) which makes everything that much easier.

It shows the importance of libraries and the use of helpful functions that may autmatically do something you were trying to figure out.

Here's how I used strcmp to overcome the difficulty:

```js
// loop through the commandline input
  for (index = 1; index < argc; index++) {
    for (index2 = 0; index2 < SIZE; index2++) {
      // Comparing input string to morse 
      if (strcmp(argv[index], morse[index2]+2) == 0) {
        printf("%c", morse[index2][0]);
      }
    }
  }
```





