# Testimonials Grid Section

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![Desktop-version](./design/desktop-preview.jpg)
![Mobile-version](./design/mobile-design.jpg)


### Links

- [Live Site URL](https://mitp7.github.io/Testimonial-Grid/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid

### What I learned

From this challenge I learned more about CSS Grid and the various properties it has such as grid template columns, rows, and areas. Using these grid properties resulted in all of the components being very responsive further reducing the amount of time spend working with the media queries.

Sample of the CSS Grid code used for both desktpp and mobile:

```css
.testimonial {
    display: grid;
    margin: 5em;
    height: 100vh;
    grid-template-columns: repeat(4, 1.5fr);
    grid-template-rows:  repeat(2, 1fr);
    grid-template-areas: 
    "wide-purple wide-purple small-grey long-white"
    "small-white wide-black wide-black long-white";
    grid-gap: 1.8rem;
}
```

Mobile version has all the area components placed vertically: 
```css
@media (max-width: 800px) {
    .testimonial {
        margin: 1em;
        grid-template-columns: 1fr;
        grid-template-rows: 3fr 1.5fr 1.5fr 2.5fr 3fr;
        grid-template-areas:     
        "wide-purple" 
        "small-grey" 
        "small-white"
        "wide-black"
        "long-white";
        grid-gap: 1.5rem;
    }
}
```

