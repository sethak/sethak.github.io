---
layout: project
type: project
image: images/micromouse.jpg
title: Collection 
permalink: projects/collection
# All dates must be YYYY-MM-DD format!
date: 2016-02-14
labels:
  - Java 
summary: This is my first ever project created in my computer science career, I hope you all enjoy! 
---

This was my first project that I have ever coded not only in my Computer Science career, but the first coding project I did in my entire life. I did not have any experience with coding until I had reached this class. I was pretty proud of this particular project because it was a milestone that I was able to complete. The difficulty of the project wasn't to hard, but its amazing how writing simple code can create a very interesting project. 

For this project, I was the lead programmer who was responsible for programming the various capabilities of the mouse.  I started by programming the basics, such as sensor polling and motor actuation using interrupts.  From there, I then programmed the basic PD controls for the motors of the mouse.  The PD control the drive so that the mouse would stay centered while traversing the maze and keep the mouse driving straight.  I also programmed basic algorithms used to solve the maze such as a right wall hugger and a left wall hugger algorithm.  From there I worked on a flood-fill algorithm to help the mouse track where it is in the maze, and to map the route it takes.  We finished with the fastest mouse who finished the maze within our college.

Here is some code that illustrates how we read values from the line sensors:

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

You can learn more at the [UH Micromouse Website](http://www-ee.eng.hawaii.edu/~mmouse/about.html).



