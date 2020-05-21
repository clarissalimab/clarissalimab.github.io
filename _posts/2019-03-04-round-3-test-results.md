---
layout: post
title:  "Round#3: Test Results"
date:   2019-03-04 15:00:0 -0300
tags: outreachy gnome usability test-results gedit
author: Clarissa Borges
---

For the last round of tests, I tested GNOME’s Text Editor (gedit) design. As I already tested gedit once (you can see the first test plan and results [here](https://medium.com/gnome-usability-testing-report/gnome-usability-testing-report-93320514ea86)), I used the same test plan with two additional tasks.

You can also check the test plan for this round on [this post]({% post_url 2019-02-15-round-3-test-plan %}).

# User Profile

![User Profile Age](/assets/images/round-3-user-profile-age.png)

![User Profile Gender](/assets/images/round-2-user-profile-gender.png)

![User Profile Computer Usage](/assets/images/round-3-user-profile-computer-usage.png)

![User Profile GNOME/ Linux usage](/assets/images/round-3-user-profile-computer-gnome-linux-usage.png)

# Tasks
* Create and save a text file
* Edit a text file
* Find and replace words
* Create a copy of a text file
* Customize the program’s presentation
* Change the window to full screen exhibition
* Print a text file

# Results
## Create and save a text file
> **1.** Type a quick note for yourself, describing something that you want to remember later.
> Please type the following short paragraphs into the text editor:
> [I prepared a note for the user to type]
> Save this note as party reminder.txt in the Documents folder.

![Party Reminder](/assets/images/round-3-gedit-party-reminder.png)

The users didn’t find any difficult doing that, as they are familiarized with this task in other programs. None of them had to think very much to complete the task.

## Edit a text file

> **2.** After typing the note, you realize that you got a few details wrong. Please make these edits:
> * In the first paragraph, change “Friday” to “Thursday”.
> * Change “17:30” to “17:00”.
> * Move the entire sentence “Teresa arranged for João’s roommate to keep him away until 7:00PM.” to the end of the second paragraph.
>
> When you are done, please save the file. You can use the same filename.

The users didn’t find any difficult doing that, as they are familiarized with this task in other programs. None of them had to think very much to complete the task.

## Find and replace words

> **3.** Actually, João prefers to go by George, and Teresa prefers Júlia. Please, replace every occurence of João with George, and all instances of Teresa with Júlia.
>
> When you are done, please save the file. You can use the same filename.

Most of them looked for the words to change and replaced them manually. Two of them realized that there must be an easier way to change every occurrence I asked, but only one figured out the “Find and replace” option. To find this option, she first tried to hit the “Ctrl – F” shortcut, but she only had the option to find words, and then she found the option in the menu.

![Gedit dropdown menu](/assets/images/round-3-gedit-dropdown-menu.png)

I guess it would be nice to show the replace option when the user tries to look for a word using the “Find” shortcut, I think I’ve seen this in other editors and would work nice. In that way, if the user only wants to find where a word is, he just needs to fill the search field and hit enter, but if he wants to replace the occurrences by other word, he can fill a second field and click “Replace all” or “Replace” to replace just the current word.

![How the “Find” option looks now](/assets/images/round-3-gedit-find.png)

![A simple prototype I made of how the “Find” option would look with the “Replace” option](/assets/images/round-3-gedit-find-and-replace.png)

## Create a copy of a text file
> **4.** You’d like to make a copy of the note, using a different name that you can find more easily later. Please, save a copy of this note as George surprise party.txt.

The users could complete this task very easily, although two of them first clicked on “Save All…” before clicking on “Save As”, but my guess is that they didn’t pay attention and were trying to complete the task faster.

## Customize the program’s presentation

> **5.** You notice without your glasses you can’t read very well, and you would prefer to use a different font. Please change the font to DejaVu Sans Mono, 12 point.
>
> **6.** You decide the black-on-white text is too bright for your eyes, and you would prefer to use different colors. Please change the color to the Oblivion color scheme.

I’ve had issues with this task because of the “Preferences” button. When I ran the tests with the 2 first testers, this button was placed in the in-window menu, but on the next three tests, two days after, the button was no longer there and was on the superior menu, outside the window.

![In the two first tests, the “Preferences” button was placed under the “Tools” button](/assets/images/round-3-gedit-dropdown-menu.png)

When the “Preferences” option was placed in the in-window menu, the testers were able to find it, but not as easily as I thought they were. I asked them why “Preferences” was not an option for them at first look and they said that they thought that they wouldn’t find “fonts” options there.

All of the testers first tried to change the font by clicking on “Plain text” (on the bottom of the window, where you can change the text highlights) and they took a while to realize they couldn’t change the font there, as none of them are familiarized with this kind of feature. They suggested that the font options would be more easy to access if these options were placed on the bottom of the window, just like the text highlight options. I disagree, because I think as a note program, the user won’t be stylizing the text all the time as if he would be when writing a document on a different kind of program, maybe it would look very full.

![Blank document](/assets/images/round-3-gedit.png)

The last three testers, when the “Preferences” button was placed on the menu outside the window, couldn’t finish the task. 

Even though not all of them found the option, I showed them where the “Preferences” option is to see if they were able to change the font. All of the testers had a little issue to change the font because the select input of the font is not enabled until the user uncheck the “Use the system fixed width font (Monospace 11)” checkbox, and their first attempt was to click on the select input several times until they stopped and read the checkbox.

![Font & Colors Preferences](/assets/images/round-3-gedit-font-preferences.png)

I think it would be better if the font option was not disabled at first, because if the user is clicking there, probably he does not want to leave the system’s default font anyway, and then leave a button to reset to editor’s default Font & Colors preferences would help to let the user go back to the system’s font.

After changing the font, the users could easily change the editor’s color scheme as the option to change it is on the same screen as the font options.

## Change the window to full screen exhibition
> **7.** You want to see the window bigger than the default size to see more text in the screen. Please, change the window exhibition to full screen.

They were a little bit confused, I guess because they are more used to other OSs and looked for a maximize button on the top of the window. Three of them found and expand icon on the menu inside the window and clicked it to see the window bigger, and two of them right clicked on the top of the window and clicked on “Maximize”, but I think the result was not the same, maybe the ones who clicked on “Maximize” did not achieve the expected result.

![The maximize button](/assets/images/round-3-gedit-maximize-screen.png)

## Print a text file
> **8.** After you finished your work, you want to print it to deliver the note to Júlia. Please, print this note.

They found this option easily as at this point they were used to the menu inside the window, the print icon was very clear for them.

