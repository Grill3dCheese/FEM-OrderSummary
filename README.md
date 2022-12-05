# Frontend Mentor - Order summary card solution

This is a solution to the [Order summary card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/order-summary-component-QlPmajDUj). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- See hover states for interactive elements

### Screenshot

![](images/order-card-screenshot.png)

### Links

- Solution URL: [https://github.com/Grill3dCheese/FEM-OrderSummary](https://github.com/Grill3dCheese/FEM-OrderSummary)
- Live Site URL: [https://grill3dcheese.github.io/FEM-OrderSummary/](https://grill3dcheese.github.io/FEM-OrderSummary/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties & animations
- Flexbox
- CSS Grid
- Mobile-first workflow
- Clamp (for font sizing based on viewport width)

### What I learned

- If I need to utilize the background css property AND background-image, background-repeat, background-size, etc. then the background shorthand needs to come FIRST! Before any of the other properties, otherwise the properties will cancel out and not work/display correctly.
- Used clamp function for the first time to resize text on card based on viewport size - this was super handy and helped to minimize the amount of media queries needed!
- Continued using Flexbox and CSS Grid to understand how they are best utilized
- Added custom animation, having text slide up on card and pulsing shadow around music note icon.

```css
.order-card__planType,
.order-card__planPrice,
.order-card__changePlan,
.order-card__cancelOrder,
button {
  font-size: clamp(0.9rem, calc(-0.25rem + 3vw), 1rem);
}

@keyframes scrollUp {
  0% {
    transform: translateY(435px);
  }

  100% {
    transform: translateY(0px);
  }
}
```

### Continued development

- Continue working with and learning clamp! It seems to be a very useful function!

### Useful resources

- [MDN - Clamp()](https://developer.mozilla.org/en-US/docs/Web/CSS/clamp) - This helped me understand the clamp function better, as I have never used it before.

## Author

- Website - [Keith McKenna](https://www.keithmckenna.com)
- Frontend Mentor - [@Grill3dCheese](https://www.frontendmentor.io/profile/grill3dcheese)
- Twitter - [@keithmckenna](https://www.twitter.com/keithmckenna)

## Acknowledgments

- As always, thank you to MDN and Google for always coming in clutch when I'm in a pinch!
