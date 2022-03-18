# Frontend Mentor - 3-column preview card component solution

This is a solution to the [3-column preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/3column-preview-card-component-pH92eAR2-). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [The challenge](#the-challenge)
- [Screenshot](#screenshot)
- [Links](#links)

  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)


- [Author](#author)
- [Acknowledgments](#acknowledgments)

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![](./screenshot.jpg)

file path for the screenshot of my solution for the desktop view: screenshot of my solution/3 column preview-card compenent desktop-view.png

file path for the screenshot of my solution for the mobile view: screenshot of my solution/3 column preview-card compenent mobile-view.png

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [live site URL](https://aemrobe.github.io/3-column-preview-card-compenent/)

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

when I do this challenge I learn one new thing which is when we make an element a grid-container we can align the grid-items inside of the column and row they are spaning by using margin auto proeprty.
for example:-
I have article element with a class of car which have four elements. I gave it a min-height property of 497px and I made this element a grid-container with 4 rows and 1 columns. I gave a size of auto for my three elements which spans the first three rows and I gave 1fr to the fourth element which spans remaining space at the bottom (fourth row). so I can postion the last element inside the fourth row wherever I want by using margin auto property.

```
html
   <article class="car suvs">
        <img src="./images/icon-suvs.svg" alt="" class="logo">
        <h1 class="car-brand">SUVs</h1>

        <p class="description">Take an SUV for its spacious interior, power, and versatility. Perfect for your next
          family vacation
          and off-road adventures.
        </p>

        <a href="#" class="learn-btn">Learn More</a> <!--fourth item-->
      </article>
```

```
css
.car{
    display: grid;
    grid-template-rows: repeat(3, auto) 1fr;
    align-content: start;
}

  /* this element will be positioned at the bottom-left corner because it put the remaining space other than it's content at the top and right place from it. */
 .learn-btn {
    margin-top: auto;
    margin-right: auto;
  }


```

### Continued development

in the near feautre I want to focus on grid,flexbox,responsive design and css animation.

## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@aemrobe](https://www.frontendmentor.io/profile/aemrobe)
- Twitter - [@Aemro112](https://www.twitter.com/Aemro112)

## Acknowledgments

I want to say thanks to my team members who always give me feedback to improve my solutions.
