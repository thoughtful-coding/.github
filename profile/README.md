# Thoughtful Coding

This project is intended to be a configurable, customizable platform for Computer Science
teachers to augment their lessons with best-practice techniques to help students learn. It
focuses on using PRIMM, reflection (journaling), and active learning to constantly test,
reframe, and highlight the material.

The core differentiators between this project and other, existing teaching platforms is
that it's:

- Open Source
- Centered around PRIMM and Reflection
- Takes a "functions first" approach
- Makes it easy to customize/create your own lessons
- Has a debugger to provide students a step-by-step view of programs
- Has turtles and the ability to assess turtle programs
- Uses AI for structured feedback **prior to final assessment by the teacher**

The project can be broken down into three main pieces. All of these pieces can
either be used as is or cloned for greater control. The pieces are:

## Student Website

A website that walks students through learning Python with an iterative, experimental
approach. The core of the website is a series of "learning sections" that allow the material
to be presented and tested in a variety of ways:

- PRIMM: Shows students a snippet of code, asks them to predict what will happen, and then
    reflect on the difference between their prediction and the actual results.
- Reflection: Asks students to reflect on various new topics and provides iterative AI-based
    feedback to help them to improve their answers prior to submitting the entry for grading.
- Multiple Selection and Multiple Choice: Asks questions at key moments to clear up
    common misconceptions and highlight key points.
- Testing: Presents students with a particular problem and verifies their solution by
    running it through a series of input/output tests.
- Prediction: Gives students an input for a particular program and has them predict what
    the output will be.
- Coverage: Gives students a desired output for a particular program and has them predict
    what the input should be to reach that point in the program.

## Instructor Back-End

An easy to setup back-end (using AWS) that stores students progress, answers, reflections.
The server is front-end agnostic, meaning that the website can present _any_ type of
material and it will be stored without issues.

The server uses Google OAuth to map student's email addresses to their answers. Predicted
costs for running the server in a globally accessible environment is around 25-50 cents
per student.

## Instructor Website

A portal that allows instructors to track the progress of their students across various
dimensions. The portal provides easy access to high-level markers like "completion
percentage" of a particular unit/lesson but also the ability to dive deep and look at the
various iterations of a student's reflection prior to submitting it for grading.
