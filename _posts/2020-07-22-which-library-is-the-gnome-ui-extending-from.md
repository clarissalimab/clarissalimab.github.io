---
layout: post
title:  "Which library is the GNOME UI extending from?"
date:   2020-07-27 20:00:0 -0300
tags: gnome personal gsoc
author: Clarissa Borges
---
About two weeks ago I did some research and learned about some libraries to choose one to extend from to use on my GSoC GNOME UI library project, and it turned out to be a very interesting topic that I'd like to share and take the opportunity to talk about how's the project going, as it's been a while since I don't blog :P

In case you don't know what my project is about, I recommend you to visit [my first post]({% post_url 2020-06-07-my-gsoc-project %}) where I provide an explanation of the project goals.

## The research
To choose a library to extend from, we had to find one that met the following requirements:

* **Customizable**: the developers need to be able to build elements and components fast and not to take too much work each of them while trying to make them look like our mockups. Considering this requirement, by choosing a library that already has elements and components, it's important to evaluate how close they are to how the GNOME UI library needs to look like, assuming this would take less time and work to adapt it.

* **Easy to learn**: make sure that contributors responsible for the GNOME websites don't need to make a huge effort to be able to use it. As a consequence of this, the adherence of the project will be improved.

* **Keeps GNOME web ecosystem looking consistent**: the library needs to provide possibilities for the project to set defaults up so that every website uses the same standards.

* **Extensible**: if some website needs an element or component that wasn't built in the library, the maintainer or some contributor can easily build on their own the component.

### Using a Library vs. Working with Vanilla CSS

Using a library saves a lot of time when it comes to styling. Many libraries provide a good set of predefined elements and components that can **ease the development**. The con to using a library can be that if the library diverges too much on what we want the GNOME UI library to look like, it will require a great effort to override existing components and elements to style them (maybe even more than just starting them from scratch).

Meanwhile, building a library from scratch allows you to build your design and define your style sheet as you wish, **keeping the markup clean**. It gives you full control of your code, and your project doesn't have unnecessary code. But as mentioned, it means having to build everything from scratch, and it's really difficult to build everything that is needed for a library in this way.

### Libraries
I considered some libraries that I heard of recently and that I think are very popular:

#### [Bootstrap](https://getbootstrap.com/)
Bootstrap is the most popular UI library, it's very easy to use and a lot of websites use it. It has lots of components ready to be used, which means you just have to add the classes to your HTML, and you are done. There are lots of themes that can be used to customize Bootstrap, this helps to find a better approach to start the GNOME UI library from, by choosing a theme that is closer to what we want the GNOME UI library to look like. On the other hand, when you need to customize it, it can be very painful.

#### [Materialize CSS](https://materializecss.com/)
Materialize is a library based on Google's Materialize Design. According to its website, the library speeds up the development by providing default stylings that incorporate its custom components, is user experienced focused, and easy to work with as they provide good documentation and support. Like Bootstrap, Materialize allows you to use themes to help to build designs that look different from others. As Bootstrap, when you need to customize it, it can take a lot of work.

#### [PureCSS](https://purecss.io/)
PureCSS is a set of small and responsive CSS modules that can be used in web projects. Pure is said to be extremely extensible by including Pure and writing some CSS on top of it, making sure that it works across browsers. You can import individual modules and start building the library just from the ones you need (like base or grids). Plus, Pure is very lightweight.

#### [Tailwind](https://tailwindcss.com/)
It's a utility-first CSS framework that doesn't provide pre-styled components like buttons, cards, and so on. Instead, it gives us low-level utility classes that add shadows, colors in a certain way that we can build components with the help of these utility classes. This means having to write less CSS and being able to use Tailwind combined with our styles.

It's hard to ensure consistency on every website if they eventually need an element or component that is not defined in the original UI library (which would be GNOME's), even using Tailwind. However, building components with Tailwind is very easy, because the naming of the classes is very consistent. Plus, as soon as someone builds a new component (even on their HTML), they can easily extract their code and submit a Merge Request for the GNOME UI library to include the new component. Anything can be easily changed.

#### [UIKit](https://getuikit.com/)
UIKit is a lightweight and modular framework for developing web interfaces, just like PureCSS, but it is more complete. Its very basic style can be extended with themes and is easy to create designs using it.

### Conclusion

In the end, Tailwind stays somewhere in the middle of using vanilla CSS and some other library: it's different from using a library that contains pre-built components, giving you the freedom to style yours, but it has utility classes that prevent you from spending too much time writing the base and also from struggling with accessibility classes, building a grid system, handling responsivity, etc. Compared to PureCSS and UIKit, it is a better approach to build a library because a complete CSS framework can be generated simply based on a configuration file that defines all the elements from the project. **Tailwind is the best use case for a complete custom design, in my opinion, so it was the chosen option for the project**.