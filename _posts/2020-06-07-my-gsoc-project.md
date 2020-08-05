---
layout: post
title:  "My GSoC Project with GNOME"
date:   2020-06-07 20:00:0 -0300
tags: gnome personal gsoc
author: Clarissa Borges
---
This was my last chance to try to be a GSoC student as I am on my last undergrad period. For this summer, I was lucky that GNOME had a web development project, and this project has everything to do with what I am more familiar with. I want to begin thanking my mentors, Claudio Wunder and Caroline Henriksen, who chose me as alumn, I am very grateful for the opportunity to learn more about front end development and to contribute to GNOME, and deeply excited to work on my project.

## What is the project about?
The motivation behind my project was the need for a refresh on the [main GNOME website](https://gnome.org) design. Although we don’t sell the GNOME desktop environment itself, nor GNOME’s programs, we want that more people feel interested about GNOME and give it a try, and we want to encourage people to contribute and be part of the community as well. GNOME's website is the first place a user or a possible contributor visits when they want to learn more about it, and the more attractive and friendly it looks, the closer to what GNOME represents it is.

At some point, my project turned out to be a UI library for all the GNOME websites - currently, they don't follow a common style guide between them, and they don't look exactly consistent with each other. In terms of technical benefits, having GNOME’s library will ease keeping UI patterns or changing them in the entire website whenever needed. It will help to maintain and evolve the website with more frequent updates and will ensure good web development practices, as it provides consistency in the design by setting defaults in the development to be followed and making the code more understandable.

The library should take in consideration the current design-wise needs of the GNOME websites, such as components, elements, assets and etc. For that, I'm running an assessment on the current state of:
* [Main GNOME website](https://gnome.org);
* [Planet](https://planet.gnome.org);
* [Surveys](https://surveys.gnome.org);
* [Events](https://events.gnome.org);
* [Developer Center](https://developer.gnome.org);
* [Discourse](https://discourse.gnome.org);
* [Extensions](https://extensions.gnome.org).

After the assessment, I'll design some new elements and components to get started with the library development :)