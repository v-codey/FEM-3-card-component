# Frontend Mentor - 3-column preview card component solution

This is a solution to the [3-column preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/3column-preview-card-component-pH92eAR2-). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

If you can suggest any improvements or have seen any thing I should know then feel free to let me know.

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
  In this challenge we have to code the given design of what frontend mentor named as 3 column preview card components. These are comparatively easy challanges in newbie section. The screenshot below shows you my take on this challenge.

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![](/design/screenshot.jpg)

This is the screenshot of the challenge solution by me.
### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

The design output is as asked, however I have take a different approach on this to make the border-radius work in both horizontal and on vertical view card (or desktop view or mobile view) by a wrapping individual card inside a main div and then applying the border-radius on the main div, and then overflow hidden will cover the extra visible corners. 

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid

### What I learned

I got to know about the min/max width & height importance while coding the cards and I learned about a new thing which I haven't used untill now that is the `mix-blend-mode`.
- `mix-blend-mode` property of an element is used to specify the blending of an element’s background with the element’s parent. 
This property I used on the button "Learn More", which enabled the button text color to blend with their respective parent cards background-colors. 
To see code snippets, see below:

```html
<a href="#" class="btn"> Learn More </a>
```
```css
.btn{
  display: inline-block;
  margin-top: 1.625rem;
  text-decoration: none;
  border: 2px solid white;
  border-radius: 100vw;
  font-size: 1rem;
  font-family: 'Lexend Deca', sans-serif;
  font-weight: 400;
  background-color: var(--very-light-gray);
  mix-blend-mode: screen;    /* <--  this is where is used the mode */
  padding: 0.75rem 1.5rem;
  transition: background-color 0.3s ease-in;
}
```

### Useful resources

- [mix-blend-mode](https://www.geeksforgeeks.org/css-mix-blend-mode-property/) - This helped me for blending button color. I really liked this pattern and will use it going forward.


## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@v-codey](https://www.frontendmentor.io/profile/v-codey)


