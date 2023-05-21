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
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![Solution Screenshot](dist/images/solution-screenshot.jpg)

### Links

- Solution URL: [Frontend Mentor Solution](https://www.frontendmentor.io/solutions/nft-preview-card-component-solution-using-flexbox-grid-and-sass-2eG2KEBEe6)
- Live Site URL: [https://carekajzex.github.io/NFT-preview-card-component/](https://carekajzex.github.io/NFT-preview-card-component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- [Sass](https://sass-lang.com/) - CSS Preprocessor
- Variables
- Nesting
- Partials

### What I learned

I learned how to do overlay effect on hover. I basically changed alpha channel of the background color to zero and opacity of the icon to zero as well. Then on hover made them visible.

I used Grid to center the div inside of a parent element and transition for the smooth changing of states.

Below is the code used:

```css
&-hover-overlay {
  background: hsla(178, 100%, 50%, 0%);
  display: grid;
  place-items: center;
  position: absolute;
  top: 0;
  left: 0;
  width: 19rem;
  height: 19rem;
  border-radius: 3%;
  transition: background 0.3s $cubic-bezier;

  &:hover {
    background: hsla(178, 100%, 50%, 50%);

    .nft-card-image-hover-overlay-icon {
      opacity: 1;
    }
  }

  &-icon {
    width: 3rem;
    height: 3rem;
    opacity: 0;
    transition: opacity 0.3s $cubic-bezier;
  }
}
```

I continue to learn Markdown. Which is not that hard at all, especially with the live preview which makes it super easy to write.

### Continued development

I need to take a closer look to hover effect and if it can be done differently.

### Useful resources

- [Traversy Media](https://www.youtube.com/@TraversyMedia) - Place where I learn everything.
- [Flexbox Crash Course](https://www.youtube.com/watch?v=3YW65K6LcIA) - Great resource for flexbox
- [Grid Crash Course](https://www.youtube.com/watch?v=0xMQfnTU6oo) - Great resource for grid
- [Markdown Crash Course](https://www.youtube.com/watch?v=HUBNt18RFbo) - Helped me to get my feet wet with Markdown

## Author

- Github - [@CareKajzeX](https://github.com/CareKajzeX/)
- Frontend Mentor - [@CareKajzeX](https://www.frontendmentor.io/profile/CareKajzeX)
- Twitter - [@CareKajze](https://twitter.com/CareKajze)