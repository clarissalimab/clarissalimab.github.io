---
layout: post
title:  "Round#2: Test Results"
date:   2019-02-08 15:00:0 -0300
tags: [outreachy, gnome, usability, test-plan, files, nautilus, notes]
---

For the second round of tests, I tested new designs for Files and Notes GNOME’s programs. I’ve written tasks and scenarios for some important features from both programs I found interesting, but the most important things to be tested that Allan Day required me to test were the programs’ menus.

You can see the test plan I prepared for the results presented here on [this post]({% post_url 2019-01-30-round-2-test-plan %}).

# User Profile
I ran the tests with 5 users this time, and used the same users for both programs. In that case there was no problem using the same users because the kind of tasks were very different, as the menu types too.

![User Profile Age](/assets/images/round-2-user-profile-age.png)

![User Profile Gender](/assets/images/round-2-user-profile-gender.png)

![User Profile Computer Usage](/assets/images/round-2-user-profile-computer-usage.png)

![User Profile GNOME/ Linux Usage](/assets/images/round-2-user-profile-computer-gnome-linux-usage.png)

# Files
![Files](/assets/images/round-2-files.png)

## Tasks
* Search for files
* Move files through folders
* Select all files
* Copy and paste files
* Create new folders
* Change exhibition

## Results
### Search for files
> 1. Yesterday, you re-organized your files and you don’t remember where you saved the copy of one of the articles you were working on. Please search for a file named “The Hobbit”.

All of the users could finish the task with no big issue, but some of the testers had a little problem when they were looking for the search bar, they were confused by the color of the program’s bar, as they thought it was a search field. So, before they clicked on the search icon, they tried to click on the bar to start typing.

![Files top bar](/assets/images/round-2-files-nav-bar.png)

### Move files through folders
> 2. You don’t think a text file should be placed at “Pictures” folder. Move “The Hobbit.txt” from the “Pictures” folder to the “Documents” folder.

They had no issue on this one. Some of them tried to drag and drop and some of them right-clicked and chose “Move to” option.

### Copy and paste files
> 3. You want to make a copy of all your documents that are inside your Documents folder to your USB drive. Please, choose the documents files that are inside the folder and paste them in your USB drive.

The testers had no idea they could select all of the files. All of them tried to select the files using the mouse and holding shift or using only the mouse. After they completed the task, I tried to ask them to do that in another way to see if they could figure out they had a better way to do so, two of them didn’t realize how to do it, the other two right clicked and chose “Select all”. Most of them used “Ctrl – C” and “Ctrl – V” shortcuts to copy the files, only one of them right-clicked and copied.

### Create new folders
> 4. To help you to find your “The Hobbit” article, you find it better to create a folder called “Movies” to put it on. Do so and move your article to your new folder, inside the “Documents” folder.

They had no issue in this one. All of them created a folder, dragged and dropped the file inside the folder.

### Change exhibition
> 5. Files and folders are usually displayed as icons, but you can display them in other ways too. Change how the file manager displays the files and folders, to show them as a list.

They didn’t realize very quick about the icon, they looked for options on the menu. One of them almost gave up until I asked him if he could find an icon that looked like what he was looking for. Maybe an additional option in the menu like “view > list” would help.

![Dropdown Menu](/assets/images/round-2-files-menu.png)

# Notes
## Tasks
* Create a new note
* Look for a shortcut that helps you to change the text style
* Put notes inside a notebook
* Search for a note
* Change the view of your notes

## Results
### Create a new note
> 1. You want to take a note of what you have to do for today so as not to forget. Please, create a note called “To-do list for today” and place there your tasks for today. *[Some tasks will be provided so that the tester doesn’t have to think of tasks to write]*

It was easy for them to create a new note, but I noticed it was not very clear how the title and the body of the note worked, as they have no apparent difference until the user starts to type.

![New blank note](/assets/images/round-2-notes-new-blank-note.png)

![New note with some text](/assets/images/round-2-notes-new-note.png)

### Look for a shortcut that helps you to change the text style
> 2. It might be annoying to change the text style by clicking on their buttons all the time. Please, look for the keyboard shortcuts to change the text style.

It was hard to tell them what I wanted, I had to be specific because they didn’t know there could be a place that contained all the shortcuts they could use. As the shortcuts were about text styling, they looked for it in the menu with the note opened. They didn’t get that the menu would change in a different screen, some of them took a while to find because of that too.

![Note menu view](/assets/images/round-2-notes-note-menu.png)

![Menu that appears when the user is at the first screen of the program](/assets/images/round-2-notes-main-menu.png)

### Put notes inside a notebook
> 3. Your notes look messy and you want to keep them separated from each other. Please, create a notebook called “To-dos” and a notebook called “Grocery lists” and place the correspondent lists inside them.

I think the steps to do that are a bit confusing for the users (even for me, I didn’t understand very well how they worked).

![Notes inside a notebook](/assets/images/round-2-notes-notebook.png)

For creating a notebook, I noticed they took very long to find the option. They had to select one or more notes and then create notebooks and select in which of them the notes should be placed. I noticed they tried several times to click on “New” to create a Notebook, so I guess maybe if we had a dropdown to create a notebook or a note would help. They looked for the option on the menu where there is a list of all notes, and there is no “notebook” there unless they select some notes, it was hard for them to find the option on an specific view of a note. One of them tried to drag and drop two notes to see if they joined and created a notebook together.

![The dropdown menu with the options “Notebook” or “Note” could show up when clicking this “New” button](/assets/images/round-2-notes-new-button.png)

Placing notes inside notebooks was difficult too because they had to follow the same first steps to create a notebook, but they had to check the notebooks where they wanted to place the note. After they created notebooks, they tried to place the notes inside the notebooks by dragging and dropping the notes inside the notebook icon. Two of the users couldn’t complete this task. Those steps seem to be very confusing.

The users who could finish the task were confused if they did complete the task because the notes still appear outside the notebooks. I think it makes sense to show them outside the notebooks as they can belong to many notebooks, but I think it would make sense too if they could belong to only a single notebook and maybe add a “tags” functionality to do this same function.

### Search for a note
> 4. You want to find your to-do list you’ve just created. Please, search for it.

All of them could figure out how to do it. 

### Change the view of your notes
> 5. Notes can be displayed in different ways. Change how the program shows the notes to display them as lists.

As they knew how to do it from the previous test, they didn’t find it any hard. 