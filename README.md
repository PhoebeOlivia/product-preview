# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)


**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![](./images/Screenshot%20Desktop.png);
![](./images/image-product-mobile.jpg);

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

### I learn't how to use custome properties to make code in larger projects than this easier to managed. 

:root {
  --clr-primary-400: hsl(158, 36%, 37%);
  --clr-primary-800: hsl(158, 36%, 16%);
  --clr-secondary-200: hsl(30, 38%, 92%);

  --clr-neutral-900: hsl(212, 21%, 14%);
  --clr-neutral-400: hsl(228, 12%, 48%);
  --clr-neutral-100: hsl(0, 0%, 100%);

  --ff-accent: 'Fraunces', serif;
  --ff-base: 'Montserrat', sans-serif;

  --fw-regular: 500;
  --fw-bold: 700;
}

.button {
  background-color: var(--clr-primary-400);
  color: var(--clr-neutral-100);
  border: none;
}

### I learn't how to use visually hidden to help with acessibilty. 

<div class="flex-group">
  <p class="product__sale-price">
    <span class="visually-hidden">Sale Price:</span>
    $149.99
  </p>
  <p class="product__original-price">
    <span class="visually-hidden">Original Price:</span>
    $169.99
  </p>
</div>

.visually-hidden:not(:focus):not(:active){
  clip: rect(0 0 0 0 );
  clip-path: inset(50%);
  height: 1px;
  overflow: hidden;
  position: absolute;
  white-space: nowrap;
  width: 1px;
}


