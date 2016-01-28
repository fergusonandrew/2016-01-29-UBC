---
layout: page
title: The Unix Shell
subtitle: Introducing the Shell
minutes: 5
---
> ## Learning Objectives
>
> *   Explain how the shell relates to the keyboard, the screen, the operating system, and users' programs.
> *   Explain when and why command-line interfaces should be used instead of graphical interfaces.

At a high level, computers do four things:

-   run programs
-   store data
-   communicate with each other
-   interact with us

They can do the last of these in many different ways,
including direct brain-computer links and speech interfaces.
Since these are still in their infancy,
most of us use windows, icons, mice, and pointers.
These technologies didn't become widespread until the 1980s,
but their roots go back to Doug Engelbart's work in the 1960s,
which you can see in what has been called
"[The Mother of All Demos](http://www.youtube.com/watch?v=a11JDLBXtPQ)".

From the 1950s to the 1980s,
most people used devices that only allowed input and output of the letters, numbers, and punctuation found on a standard keyboard,
so programming languages and interfaces had to be designed around that constraint.

This kind of interface is called a
**command-line interface**, or CLI,
to distinguish it from a
**graphical user interface**, or GUI,
which most people now use.
The heart of a CLI is a **read-evaluate-print loop**:
when the user types a command and then presses the enter (or return) key,
the computer reads it,
executes it,
and prints its output.
The user then types another command,
and so on until the user logs off.

So we can try this now. In your terminal type 'ls', and then hit enter.

This description makes it sound as though the user sends commands directly to the computer,
and the computer sends output directly to the user.
In fact,
there is usually a program in between called a
**command shell**.
What the user types goes into the shell,
which then figures out what commands to run and orders the computer to execute them. Note, the shell is called *the shell* because it encloses the operating system in order to hide some of its complexity and make it simpler to interact with.

A shell is a program like any other.
What's special about it is that its job is to run other programs
rather than to do calculations itself.
The most popular Unix shell is Bash, you may have heard of it before.
Bash is the default shell on most modern implementations of unix, including OS X and most Linux distros,
and in most packages that provide Unix-like tools for Windows.

Using Bash or any other shell
sometimes feels more like programming than like using a mouse.
Commands are terse (often only a couple of characters long),
their names are frequently cryptic,
and their output is lines of text rather than something visual like a graph.

On the other hand,
the shell is powerful because it allows us to combine existing tools in as many ways as we can imagine with only a few keystrokes
and to set up pipelines to handle large volumes of data automatically. When doing computational research this is crucial for productivity and reproducibility.

In addition to all of that, familiarity with the shell is near essential to run a variety of specialised tools and resources using remote, high-performance computing systems. 

As clusters and cloud computing systems become more popular for scientific data crunching,
being able to efficiently interact with them is becoming a necessary skill. We can build on the command-line skills covered here to tackle a wide range of scientific questions and computational challenges.

## Nelle's Data
Today, we're going to be working with some example data from Nelle Nemo, a marine biologist who
has just returned from a six-month trip to the field with lots of data to process. 

We are going to use her data to learn some basics of data processing. More specifically,
we'll learn how to use the shell
to automate the most repetitive steps Nelle might need to  perform.

