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
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- Recreate the card design and layout
- Optional modifications

**Actual Design: Desktop**

![Desktop design image](design/desktop-design.jpg)

**Actual Design: Mobile**

![Mobile design image](design/mobile-design.jpg)

### Screenshot

Final solution for desktop and mobile.

![](./screenshots/desktop-screenshot.png)

![](./screenshots/mobile-screenshot.png)

### Links

- Code Solution URL: [GitHub](https://your-solution-url.com)
- Live Site URL: [Hosted on Vercel](https://your-live-site-url.com)

## My process

### Built with

- HTML5 markup
- CSS3 Columns
- Mobile-first workflow
- CSS Media Queries

No external 3rd party libraries or frameworks were used. Fully custom, vanilla HTML5 and CSS3.

### What I learned

**CSS Columns**
The use of CSS columns to quickly create a multi-column layout with equal width was suprisingly quite easy and simple than I thought. It was not a complex task, but it was something that I would struggle with to correctly implement, especially as I am just starting out.

Adding the following code to a parent element, and then adding the corresponding number of `div`s as children that act as columns is very simple.

```
<style>
  .parent {
    columns: 3;
    column-gap: 3px;
  }
</style>

<div class="parent">
  <div id="1"></div>
  <div id="2"></div>
  <div id="3"></div>
</div>
```

**Media Queries**
To make the website/card/component responsive - to render correctly when the screen size changes, I used CSS Media Queries to set breakpoints, at which I hide/display the correct card component. I created two separate cards (one for mobile, and another for desktop) as I felt that the given design was quite different, and I was not able to convert it just by changing the column widths to 100%.

```
@media screen and (max-width: 1010px) {
  .card {
    display: none;
  }
}

@media screen and (min-width: 1010px) {
  .card2 {
    display: none;
  }
}

```

---

The most important learning experience for me, was to try and cut down all duplicate code, which was especially tough for me in CSS. I still think there is room for improvement, and I would love to here from anyone who has suggestions.

### Continued development

This repository and project will remain active as I try to improve the code, make changes, and review any possible changes made by other contributors. Feel free to add issues, or make pull requests.

### Useful resources

- [CSS-Tricks](https://css-tricks.com) - This website has many helpful blog posts, examples and tutorials. I used this for learning the CSS Columns implementation, and was very happy with the explanation.
- [W3 Schools](https://www.w3schools.com) - This is an amazing resource for references when I get stuck or forget something at any point of time during development.

## Author

- Website - [Aditya](https://yo.adityaone.com)
- Frontend Mentor - [@adityavinodh](https://www.frontendmentor.io/profile/adityavinodh)
- Twitter - [@THEadityavinodh](https://www.twitter.com/THEadityavinodh)

## Acknowledgments

I would like to thank Frontend Mentor for providing this experience and platform, as well as the author for creating this challenge.
