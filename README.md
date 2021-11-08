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

:root {
   background: hsl(229, 57%, 11%) url('/images/bg-desktop.png') no-repeat bottom /
      100% 52.5%;
   /* fluid bg-img */
}
```

### Continued development

Further clip path uses - same use case past two projects (with Sunnyside Agency)

Further background img control - experimenting (always possible to control them - keeping important parts in focus or changing layout in mqs)

### Useful resources

-  [Using CSS Clip Paths](https://teamtreehouse.com/library/css-clipping-paths) - This tutorial taught me all the basics about using clip paths, alongside some practical exampls such as creating an effect where text can blend in with background images via 'clipping' certain shapes to hide the text at specific points.

## Author

-  Website - [Joshua Jameson-Wallis](https://joshuajamesonwallis.com)
-  Linkedin - [Joshua Jameson-Wallis]()

###### TODO

HTML:

Wrapping <img> in <a> for icons - thinking about what's interactive (with further potential purpose)

CSS:

Fluid background img - fixed vs fluid values (for both size + position) | this specific SVG ok to keep growing - not all are

Img icons with background/border around | flex to center within - grid + place-items: center (less code)

Clip path for triangle/speech bubble effect on 'data left' pseudo element | fluid position of pseudo el - pinned to middle on mobile (translate trick) + fluid on wider (max-width on wrapper keeps all aligned)

Progress bar + circle pseudo el within (fixed % horizontally so responded with parent bar + didn't become mis-aligned) | box-shadow - glow effect (re-usable for other btn styles/usecases)
