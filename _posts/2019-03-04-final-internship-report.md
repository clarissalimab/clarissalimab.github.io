---
layout: post
title:  "Final internship report"
date:   2019-03-04 20:00:0 -0300
tags: outreachy gnome personal
---

Today is my last day as an Outreachy intern for GNOME. My mentor, Jim Hall, encouraged me to write some topics about the work I developed during the internship and I will add some more that may be useful for readers who may want to apply on next rounds.

![Outreachy](/assets/images/outreachy-logo.png)

# How many usability tests did I do? And what did each usability test look like?
I did three rounds of usability testing with different programs. To run the tests, I used the program’s development versions downloaded with [flatpak](https://flatpak.org/).

# What and how was a round of test?
A round of test was the complete cycle of preparing, running and reporting test results. It started when the design team asked me to prepare tests for one or more program and told me what functionalities they need to get tested.

Based on what the design team asked, I downloaded a new design of the program using [flatpak](https://flatpak.org/) and did a walk through along the program to find out myself how did it work, specially through the tasks the design team required.

When I already knew the program, I did not need to see all the functionalities working to write the tasks. I could just write them before and after I wrote, I tried to complete them to see if the program was working and to imagine how the scenarios for the tasks could be. Sometimes only this process was enough to find some bugs and report them to the design team (as happened with Contacts, which I ended up not testing because of that).

After that, I showed the tasks and scenarios to Jim and Allan Day (who was representing the design team) and received feedbacks from them to improve my tests and add or remove tasks. In the second round, Jim helped me to write tasks and scenarios for some programs, but they were not used because the tests changed. Even though they were not used, doing that with him helped me a lot to write the next tasks and scenarios more easily.

When the tasks and scenarios were ready, I tried to complete the tasks as if I was a user to figure out if the volunteers would be able to run the tests. After that, the tests were ready to be translated to my native language and to be shot with my volunteers.

Some tests need environment preparations, such as creating sample files, changing program’s configurations and stuff like this. I always had a note with that so as not to forget.

After I ran the tests, I listened to their recordings and took notes about what I heard and what I saw them seeing. The recordings helped a lot to be able to watch the testers to complete their tasks without loosing time writing during the tests.

When I was reporting the results, I tried to be direct and to write suggestions of better designs based on what I was watching the users doing, even if they were able to complete the tasks. I always tried to be clear if the users could or not complete their tasks, how did they manage to do that and why did they follow their steps. Sometimes it is important to ask them what did they think and how it would be easier to complete some task in their opinion, it helps to give the design team some improvement suggestions.

# What did each usability test focus on?
## Round#1
![Sound Settings](/assets/images/round-1-sound-settings.png)

On the first round, I tested a design for sound settings. I tested some basic configurations for sounds, such as changing the volume of applications, muting them, changing output devices and applications’ sound balance. You can see the test plan [here]({% post_url 2018-12-25-round-1-test-plan %}) and the test results [here]({% post_url 2019-01-03-round-1-test-results %}).

## Round#2
![Files](/assets/images/round-2-files.png)

![Notes](/assets/images/round-2-notes.png)

This round I tested two programs: Files and Notes. Allan wanted me to test their menus and I also tested some of the program’s functionalities. On this round I was supposed to test Contacts too, but the program was not working properly, so unfortunately I wasn’t able to run the tests on it. You can see the tests plan [here]({% post_url 2019-01-30-round-2-test-plan %}) and the test results [here]({% post_url 2019-02-08-round-2-test-results %}).

## Round#3
![Gedit](/assets/images/round-3-gedit.png)

On the last round I tested GNOME’s text editor. I tested some of its most important functionalities, such as saving and editing notes, customizing the program’s exhibition and the window’s size. You can see the test plan [here]({% post_url 2019-02-15-round-3-test-plan %}) and the test results [here]({% post_url 2019-03-04-round-3-test-results %}).

# What did I learn about usability testing by the end of the internship?
1. How to prepare and run tests, and from them, how to filter the results to improve the designs. I had many ideas of improvement suggestions while I watched the users trying to complete the tasks.

2. A bigger number of testers does not always give you more precise results. When I applied to the internship, I tried to look for the bigger amount of volunteers as I could because I thought it would bring me better results and I would have a better contribution, and, consequently, I would be chosen for the internship (hehe :P). On the first week of the internship I studied with the help of some articles that Jim sent me and I discovered that the time you spend running tests with more testers than you actually need can be spent with writing results faster and giving the design team more time to work on new designs. I discovered that it was true on the first round, when I ran tests with 7 volunteers, when I needed only 5.

3. Language is very important while testing, you have to choose well your words so that understanding what the task means does not become an obstacle for the user. Also, you have to be careful with that because what you say can change the way testers complete the tasks.

4. Always ask the users to speak aloud what they are thinking while they are trying to complete a task, you can get a lot of information from how the user’s mind tries to “solve” the task by that. If the user is shy and not speaking very much, you can induce him to speak by asking questions like “What are you trying to do?” or “What are you looking for?”.

5. Usability testing in general is an easy contribution to make when you learn about it, and we need to make it easier for active users to become contributors if they want to help our community with usability tests.

# How was this internship cycle?
On this round of Outreachy, the mentors were asked to leave the intern more independent and let him work quickly. Personally, I think it is very important for the intern to learn how to research and learn by himself, even though knowing that he had the mentor’s support if needed.

I learned how to research for study materials alone and sometimes I had to hurry because the internship timeline did not always work as we wished, as we depended from other people to run the tests and we were subject to various contingencies (for example, I got sick for a week on the last round and I had to run with the tests to finish the round on time before the internship ended).

The internship demands that you be proactive and do not depend so much on the mentor’s instructions. You can research for yourself if you have doubts and study alone, sometimes you get results faster and you don’t have to take your mentor’s time by asking him something that you can do by yourself.

Overall, I guess that’s what I recall for now. I’d like to thank the Outreachy organizers that made this internship possible for so many people and opened doors for this opportunity. I’d like to thank Allan Day too for all the attention and for providing me help to run the tests and special thanks for Jim Hall for being such a good mentor, for helping me to grow and for being so helpful and patient, I couldn’t have a better mentor.

If you are trying to apply for the internship and need help with something, you can comment this post or e-mail me on [clarissalimab08@gmail.com](mailto:clarissalimab08@gmail.com), I’ll be happy to help you. You can find my first contribution for the project [here](https://medium.com/gnome-usability-testing-report/gnome-usability-testing-report-93320514ea86).