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
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

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

**html**
<!-- changing image on orientation -->
<picture class="product__image">
          <source
            srcset="images/image-product-desktop.jpg"
            media="(min-width: 600px)"
          />
          <img
            src="images/image-product-mobile.jpg"
            alt="perfume bottle surrounded by green leaves"
          />
        </picture>

<!-- sr-only class -->
<p class="product__current-price">
  <span class="sr-only">Current price:</span>
  $149.99
</p>

<!-- data element for buttons -->

<button class="button" data-icon ="shopping-cart"> Add to Cart</button>

**css**

<!-- centering content on the body -->

body {
min-width: 100vw;
display: grid;
place-content: center;
}

<!-- sr-only class css -->

.sr-only:not(:focus):not(:active) {
clip: rect(0 0 0 0);
clip-path: inset(50%);
height: 1px;
overflow: hidden;
position: absolute;
white-space: nowrap;
width: 1px;
}

<!-- data element for buttons -->

.button[data-icon="shopping-cart"]::before {
content: "";
background-image: url(images/icon-cart.svg);
width: 15px;
height: 16px;
}

### Useful resources

- [Scott O Hara](https://www.scottohara.me/blog/2017/04/14/inclusively-hidden.html) - This helped me with the code for the sr-only class that improved accessibility.

- [Josh Comeau CSS Reset](https://www.joshwcomeau.com/css/custom-css-reset/)

- [Kevin Powell] (https://www.youtube.com/channel/UCJZv4d5rbIKd4QHMPkcABCw) - I highly recommend his channel for anyone interested in getting a deeper understanding of CSS, responsive design and web accessibility.

## Author

Name: Christopher Zimbizi
