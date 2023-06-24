# Frontend Mentor - Results summary component solution

This is a solution to the [Results summary component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/results-summary-component-CE_K6s0maV). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page

### Screenshot

![Result in desktop](./screen/result-desk.png)
![Result in mobile](./screen/result-mobile.png)

### Links

- Solution URL: [Netlify]()

## My process

I did the project with sass, so I began to prepare the environment for its compilation with gulp, once ready I began to organize the sass folders, creating a base for general styles, I created the variables with the colors that will be used and fonts, I create mixins for the media queries with the necessary sizes and use normalize. once ready I start to layout the HTML of the site once ready I create the layout folder inside sass to start giving styles to the layout with HTML following the guidelines of the challenge in the style guide, the scss code is compiled in the css folder in the app.css file and you're done.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- SASS
- Gulp
- Normalize

### What I learned

In this challenge reinforce knowledge of HTML layout, apply gradients and layout with grid

```scss
.contenedor {
    max-width: 60rem;
    min-width: 50rem;
    margin: 5rem auto;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    box-shadow: 10px 10px 23px -5px rgba(0,0,0,0.2);
    border-radius: 3rem;
    // height: 50rem;
    @include m.telefono {
        grid-template-columns: 1fr;
        height: auto;
        margin: 0 0 5rem 0;
        border-radius: 0 0 3rem 3rem;
        min-width: 100%;
    }

    .result {
        background: linear-gradient(to bottom, v.$violeta-claro 0%, v.$azul-medio 70%);
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        padding: 2rem 5%;
        border-radius: inherit;
        min-width: 25rem;
        @include m.telefono {
            border-radius: inherit;
            padding: 2rem 15%;
        }
    }
}
```

## Author

- Name - [Jonathan Tovar]
- Frontend Mentor - [@Nathantvr](https://www.frontendmentor.io/profile/Nathantvr)
