# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![](./![alt text](image.png))

### Links

- Solution URL: (https://github.com/korcakSEA/nft-preview-card-component-main.git)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow


### What I learned

My major learnings while working through this project is the hover effects together with different images/ elements.

You can see code snippets below:


```css
.card__image{
    border-radius: 1rem;
    overflow: hidden;
    position: relative;
    background-color: transparent;
    transition: background-color 0.3s ease;
}   

/* Base Image */
.main__image{
    transition: opacity 0.3s ease;
}


/* Hover Image (Initially Hidden) */
.hover__image{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
    opacity: 0;
    transition: opacity 0.3s ease;
    pointer-events: none; /* ensures hover passes through */
}

.card__image:hover{
    background-color: var(--Cyan-400);
    cursor: pointer;
}

.card__image:hover .main__image{
    opacity: 0.5;
}

.card__image:hover .hover__image{
    opacity: 1;
}
```

## Author

- Frontend Mentor - [@korcakSEA](https://www.frontendmentor.io/profile/korcakSEA)
