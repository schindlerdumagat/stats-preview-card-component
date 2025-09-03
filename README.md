# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

This is a responsive stats preview card component. It allows you to practice the basics which are HTML and CSS as well as responsive design techniques.

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

![](./screenshot.png)

### Links

- Solution URL: [https://www.frontendmentor.io/solutions/responsive-stats-preview-card-component-using-flexbox-and-bem-FCzOLkA-nD](https://www.frontendmentor.io/solutions/responsive-stats-preview-card-component-using-flexbox-and-bem-FCzOLkA-nD)
- Live Site URL: [https://schindlerdumagat.github.io/stats-preview-card-component/](https://schindlerdumagat.github.io/stats-preview-card-component/)

## My process

1. Inspect the figma design
2. Create a Github repository for the project
3. Download the necessary fonts, add CSS resets and create custom variables based on the design system in figma.
4. Build the structure of the HTML according to the design.
5. Add styling to the HTML elements starting from the layout all the way to the elements within that layout.
6. Compare the output from the design and polish the solution.
7. Publish it to Github, create a live site and test the live site as well.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow
- [BEM](https://getbem.com/) - Block, Element, Modifier

### What I learned

I was able to implement responsive images using the picture element.
```html
<picture class="stats__img-container">
          <source
            srcset="./images/image-header-desktop.jpg"
            media="(min-width: 48em)"
          />
          <img
            class="stats__img"
            src="./images/image-header-mobile.jpg"
            width="654"
            height="480"
            role="presentation"
            aria-hidden="true"
            alt=""
          />
        </picture>
```

I learned that you can use blend modes to add color overlays to images.
```css
.stats__img-container {
  background: var(--clr-purple);
}

.stats__img {
  mix-blend-mode: multiply;
  opacity: 0.7511;
  background-color: var(--clr-purple);
  max-height: clamp(15rem, 2.9532rem + 51.3995vw, 27.625rem);
  height: 100%;
}
```

### Useful resources

- [Responsive Images](https://web.dev/learn/design/responsive-images) - This gave me some techniques on how to implement responsive images.
- [Responsive Images - Picture Element](https://web.dev/learn/design/picture-element) - This gave me an alternative way to implement responsive images with more control.

## Author

- Website - [Schindler Dumagat](https://schindlerdumagat.github.io/webportfolio/)
- Frontend Mentor - [@schindlerdumagat](https://www.frontendmentor.io/profile/schindlerdumagat)
- LinkedIn - [@schindler-dumagat-015238230](https://www.linkedin.com/in/schindler-dumagat-015238230/)
