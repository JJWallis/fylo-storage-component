# Frontend Mentor - Fylo data storage component solution

This is a solution to the [Fylo data storage component challenge](https://www.frontendmentor.io/challenges/fylo-data-storage-component-1dZPRbV5n) on Frontend Mentor

## Table of contents

-  [Overview](#overview)
   -  [The challenge](#the-challenge)
   -  [Screenshot](#screenshot)
   -  [Links](#links)
-  [My process](#my-process)
   -  [Built with](#built-with)
   -  [What I learned](#what-i-learned)
   -  [Continued development](#continued-development)
   -  [Useful resources](#useful-resources)
-  [Author](#author)

## Overview

### The challenge

Your users should be able to:

-  View the optimal layout for the site depending on their device's screen size

### Screenshot

![](./Screenshot.png)

### Links

-  Live Site URL:

## My process

### Built with

-  Semantic HTML5 markup
-  Flexbox
-  Mobile-first workflow

### What I learned

```css
.data-container__meter::after {
   box-shadow: 0 0 3px 0 white;
   /* glow effect */
   clip-path: polygon(100% 0, 0 0, 100% 100%);
}
```

```css
:root {
   background: hsl(229, 57%, 11%) url('/images/bg-desktop.png') no-repeat bottom /
      100% 52.5%;
}
```

The background SVG for this project was at first difficult to control, since it would continue to scale either vertically or horizontally as the viewport increased. Yet while experimenting with the size of the asset, I discovered that providing a fixed vertical size in either px or at 100%, with a fluid horizontal size allowed the SVG to only scale along the x axis. In this instance it works quite nicely, but I am aware not all assets will look pleasant if they're continually stretched.

```css
.logo-container__icons-container {
   display: flex;
   flex-wrap: wrap;
}
```

Img icons with background/border around | flex to account for future content (wrap) vs inline-block + vertical-align (must apply style to each new img)

fluid position of 'data left' pseudo element - pinned to middle on mobile (translate trick) + fluid on wider (max-width on wrapper keeps all aligned)

Progress bar + circle pseudo el within (fixed % horizontally so responded with parent bar + didn't become mis-aligned) | box-shadow - glow effect (re-usable for other btn styles/usecases)

### Continued development

Further clip path uses - same use case past two projects (with Sunnyside Agency) although seems quite specific + niche use-cases

Further background img control - experimenting (always possible to control them - yet when first setup can seem very difficult)

### Useful resources

-  [Using CSS Clip Paths](https://teamtreehouse.com/library/css-clipping-paths) - This tutorial taught me all the basics about using clip paths, alongside some practical examples such as creating an effect where text can blend in with background images via 'clipping' certain shapes to hide the text at specific points.

## Author

-  Website - [Joshua Jameson-Wallis](https://joshuajamesonwallis.com)
-  Linkedin - [Joshua Jameson-Wallis]()
