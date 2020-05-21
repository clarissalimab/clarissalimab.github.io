---
layout: post
title:  "Types of Usability Testing"
date:   2018-12-11 15:00:0 -0300
tags: outreachy gnome usability research
author: Clarissa Borges
---

There are many different ways of testing usability, and this is because every test has a main objective and a context where it is better to be applied on. Deciding on which kind of test you are going to use depends on what do you have of your product and what are you trying to find out about it.

As most of the tests I’m going to perform along this internship are from designs that haven’t gone live yet, I’ll give an approach about two types of usability testing that fit better to this context: Paper Prototype Test and Prototype Test.

To illustrate the explanations about the types of testing, I’ll be using the following articles:

* [Usability testing for early-stage software prototypes](https://opensource.com/article/17/9/paper-based-usability-testing)
* [Paper Prototyping As A Usability Testing Technique](https://usabilitygeek.com/paper-prototyping-as-a-usability-testing-technique/)
* [GNOME Usability Testing Report](https://medium.com/gnome-usability-testing-report/gnome-usability-testing-report-93320514ea86)
* [Usability testing through prototypes](https://opensource-usability.blogspot.com/2014/05/usability-testing-through-prototypes.html)

# Paper Prototyping tests vs. Prototyping tests
Those two kind of tests are very similar, as they are not the real software working, they are prototypes of screens that we want to test. So, in both kinds of tests, we need to simulate the software behavior as the testers perform the tasks.

To prepare a paper prototyping test, we need to have some screens designed in papers to let the users interact with them. As the testers perform the tasks, the conductor is responsible for changing between screens and reproducing other software behaviors (screen alerts, dropdowns, etc).

The difference to a prototype test now is just where the screens are showed to the tester. To proceed with this test, the screens must be designed on the computer (not necessarily they have to be perfect or so much similar to the final design, they just need to be comprehensible to the tester and contain the main components) and there are some ways the test conductor can reproduce the test behavior:

* The test conductor can use images of the screens and switch manually between them as the tester goes through the tasks

* The designers who prepared the screens can add behaviors by using some software (there are some software that allow the designer to add behavior)

* The designers who prepared the screens can add behaviors to them simply by using web pages with html and switching through them using the html `<area>` tag

![Image from [Usability Geek](https://usabilitygeek.com/paper-prototyping-as-a-usability-testing-technique/)](/assets/images/paper-prototyping-usability-illustration-1.jpg)

# How to run a Usability Testing?
As most usability testing methods do, during the tests execution, we need first to collect some information about our testers that may be interesting to what we expect to find out about our design usability (e.g. gender, age, computer usage, familiarity with the kind of software we want to test, etc). I like to use Google Forms for this part because it already generates by itself the charts I need to use in the report.

We should give the testers some tasks to complete, and as they go, we reproduce the software behavior as if they were using a real software. For each task to be completed, we give them a brief context before asking them to complete the task, so that they can think as they were really using the software.

While the testers complete the tasks, the test conductor can use a heat map to summarize the results, where we can imagine a scale of colors to represent the ease or difficulty to complete the tasks (I see sometimes the colors are not exact the same in the tests I saw, so I guess the colors may mean different results in each context and it’s O.K. to change them if needed).

![The heatmap I got from my usability testing results](/assets/images/heatmap-example-1.png)

A heat map helps us to summarize the results and gives us an overview about the testers performances. We can know from it what were the tasks that the testers could execute with no difficult and the ones that should be worked on better designs to have better results. Heat maps also can be compared through iterations to see the improvements working.

It is important to take notes about what is happening during the tests, as the heat map is not enough to assume many details that are important to observe. Having a section saying what worked well is nice to show what the designers can maintain or maybe reproduce on another screens. Also, having a section saying what were the difficulties, the challenges and so on is crucial to track what were the design issues and to identify what changes will be needed for the next iterations.

# Some tips to follow while applying the tests
1. **Ask testers to think out loud** helps us to follow their rationales while they perform the tasks. This is useful to identify not only where they may have difficult, but also why they are having trouble.
2. **Consider showing testers the current environment (if one exists) prior to performing the usability test** helps the testers to know better how some parts of the system work previously.
3. **Let testers preview the material beforehand** helps the testers to know all the options they have so that they won’t loose their time looking for the options during the tests or click the wrong option because they didn’t see all of them.