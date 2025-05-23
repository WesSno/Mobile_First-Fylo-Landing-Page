# Frontend Mentor - Fylo landing page with two column layout solution

This is a solution to the [Fylo landing page with two column layout challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/fylo-landing-page-with-two-column-layout-5ca5ef041e82137ec91a50f5). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size
- See hover states for all interactive elements on the page

### Links

- Solution URL: [View Solution](https://github.com/WesSno/Mobile_First-Fylo-Landing-Page)
- Live Site URL: [View Site](https://kwatia-fylo-landing-page.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

I learnt a new way to validate emails using vanilla JavaScript

To see how you can add code snippets, see below:

```js
function emailValidation(email) {
  const emailRegex = /^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$/;
  return emailRegex.test(email);
}

function checkEmail() {
  event.preventDefault();

  const form = event.target;
  const input = form.querySelector("input[type='text']");
  const errorMsg = form.querySelector(".err-msg");
  const email = input.value;

  if (emailValidation(email)) {
    errorMsg.style.display = "none";
    input.classList.remove("border-color");
  } else {
    errorMsg.style.display = "block";
    input.classList.add("border-color");
  }
}
```

## Author

- Website - [Kofi Baafi Kwatia](https://github.com/WesSno)
- Frontend Mentor - [@WesSno](https://www.frontendmentor.io/profile/WesSno)
