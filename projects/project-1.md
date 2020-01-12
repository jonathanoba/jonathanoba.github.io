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

<div class="ui small rounded images">
  <img class="ui image" src="../images/micromouse-robot.png">
  <img class="ui image" src="../images/micromouse-robot-2.jpg">
  <img class="ui image" src="../images/micromouse.jpg">
  <img class="ui image" src="../images/micromouse-circuit.png">
</div>

One of the assignments for my ICS 212 course had me create a program that could accurately translate a phrase in Morse Code into the English equivalent. The purpose of the assignment was to learn how to take inputs from the command line as well as be able to compare the input string to morse. 

The most difficult part of the task was to compare the input string and the Morse Code library within the program. It forced me to get used to methods such as strcmp (string compare) which makes everything that much easier.

It shows the importance of libraries and the use of helpful functions that may autmatically do something you were trying to figure out.

Here's how I used strcmp to overcome the difficulty:

```js
byte ADCRead(byte ch)
{
    word value;
    ADC1SC1 = ch;
    while (ADC1SC1_COCO != 1)
    {   // wait until ADC conversion is completed   
    }
    return ADC1RL;  // lower 8-bit value out of 10-bit data from the ADC
}
```





