---
layout: post
title:  "GSoC final report!"
date:   2020-08-30 20:00:0 -0300
tags: gnome personal gsoc
author: Clarissa Borges
---
## My project
My project consisted of building a UI library for the GNOME web ecosystem. GNOME has many websites ([gnome.org](gnome.org), [extensions.gnome.org](extensions.gnome.org/), [discourse.gnome.org](discourse.gnome.org/), [planet.gnome.org](planet.gnome.org/), [developer.gnome.org](developer.gnome.org/), [surveys.gnome.org](surveys.gnome.org/) and many others, but, currently, they don't have a consistent design between each other. The GNOME UI library then comes with those main following goals:

* Keep a consistent look between the GNOME websites;
* Ease the development and increase the maintainability of the websites, once the developers responsible for them won't have to spend a lot of time designing;
* Refresh the GNOME websites look.

I started the project with an assessment of the current state of GNOME. I worked on an inventory of the main GNOME websites, where I had to find and research, for each website:

* Who is responsible for it;
* In which platform it runs;
* Theme information (does it use a theme? Is it extended from some framework like bootstrap?);
* Who is the website target audience;
* What are the website goals;
* Which visual elements draw more of the attention.

I wrote the inventory on issues so it is documented to be used as a reference later on the project. [Inventories](https://gitlab.gnome.org/Teams/Engagement/websites/general-website-resources/-/issues?scope=all&utf8=%E2%9C%93&state=closed&label_name[]=Inventory):

* [Main GNOME Website](https://gitlab.gnome.org/Teams/Engagement/websites/general-website-resources/-/issues/1)
* [GNOME Extensions](https://gitlab.gnome.org/Teams/Engagement/websites/general-website-resources/-/issues/2)
* [Events Portal](https://gitlab.gnome.org/Teams/Engagement/websites/general-website-resources/-/issues/3)
* [Planet](https://gitlab.gnome.org/Teams/Engagement/websites/general-website-resources/-/issues/4)
* [Discourse](https://gitlab.gnome.org/Teams/Engagement/websites/general-website-resources/-/issues/5)
* [Developer Center](https://gitlab.gnome.org/Teams/Engagement/websites/general-website-resources/-/issues/6)
* [Surveys](https://gitlab.gnome.org/Teams/Engagement/websites/general-website-resources/-/issues/7)
* [Wiki](https://gitlab.gnome.org/Teams/Engagement/websites/general-website-resources/-/issues/8)

After the inventory, I started working on an evaluation of the website components and elements: how do they look like now, how should they look like, fonts, spaces, and, meanwhile, I created some mockups for them on [Figma](https://www.figma.com/files/project/10093619/WWW) to help me build the project. The Figma project is not an official source, I used it as a tool for helping me with the designs.

Just like the inventory, the evaluations are placed on [issues](https://gitlab.gnome.org/Teams/Engagement/websites/general-website-resources/-/issues?scope=all&utf8=%E2%9C%93&state=all&label_name[]=Evaluation) as well. Between the evaluation issues, there is one especially describing the research I worked on to [decide on which library the project would extend from](https://gitlab.gnome.org/Teams/Engagement/websites/general-website-resources/-/issues/15). In conclusion, I chose the [Tailwind](https://tailwindcss.com/) utility-first CSS framework. In parallel with the evaluation and design, I created with my mentor, Claudio Wunder, the project configuration for the library.

I coded preflight setups: typography and colors and basic components/ elements: inputs, buttons, and cards. Tailwind helps a lot with spacing, accessibility classes, flex, grid, and other basics :D To place the project documentation, I configured a Jekyll project and my mentor helped me to configure a GitLab CI to have the project documentation placed at [Gitlab Pages](https://teams.pages.gitlab.gnome.org/Engagement/websites/general-website-resources/), which holds every component, configuration, element, etc that is already merged to master. The work I did is on the [GNOME General Website Resources repository](https://gitlab.gnome.org/Teams/Engagement/websites/general-website-resources) (on issues, MRs and code as well, me and my mentor were the only authors in the project).

Last but not least, during the project the GSoC and Outreachy interns had the opportunity to give a small talk on GUADEC - the main GNOME conference - and it was an enthusiastic way of sharing about our projects and contributions!

## What were the challenges
* **Project requirements**: Besides having some knowledge about usability, that diverges a lot from knowing how to design stuff and what I should look at on the current design to improve on the UI library. I struggled very much with the inventory and the evaluation parts, and my lack of knowledge about this messed up with my confidence in the project.
* **Project set up**: It was very hard to find references about how to proceed to create a UI library extended from Tailwind. It took me a few days (maybe more than a week) experimenting stuff and project configurations to find the best approach, and yet, I couldn't find it myself. Thankfully, Claudio helped me with that and the project was now moving forward.

## Work in progress and future steps
The whole GNOME UI library project is still is far from over. I'm happy to continue the project and count on other contributors interested in helping the project to happen! For now, those are some of the missing parts of the project:
* Finishing the basic library elements and components, like
    * Tables
    * Lists
    * Alerts
* Publishing it into a CDN to be used on the websites
* Create Platform-Specific Frameworks

## Conclusion
I'm very happy to be given the opportunity of working with GNOME once again. Even having a lot of work to be done before using the project in real life, I feel fulfilled with the work I've done, and I want very much to continue in the project as much and as often as I can.

I want to thank my mentors, Claudio Wunder, Caroline Henriksen and Britt Yazel, for being so patient to me and for their help whenever I needed. I hope we can still work together on this project and other opportunities!