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
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![](./screenshot.jpg)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

**Note: These are just examples. Delete this note and replace the list above with your own choices**

### What I learned

Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge.

For this project I mainly focused on application of CSS layout concepts such as flexbox and positioning, this also marks my first time working directly with SVGs and learning how to insert them into a page. My biggest hurdle was completing the hover over active state for the main image and creating an overlay.

Specifically learning how to use the z-index property to order elements on top of each other and the transition and transform properties to create nice hover animations:
```css
.img-overlay {
  position: absolute;
  top: 0;
  width: 100%;
  height: calc(100% - 4px);
  background-color: hsl(178, 100%, 50%, 50%);
  border-radius: 15px;
  z-index: 1;
  opacity: 0;
  transition: opacity 0.3s ease-in-out;
}

.img-overlay img {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
```

I also encountered a bug that was creating an extra empty <li> element on the page and it took me a couple of days why this was occurring just to figure out (as I was typing a cry for help on stack overflow) that I simply didn't properly close the last <li> element. So I definitely learned the importance of closing tags correctly and double checking my code for typos or spelling mistakes when debugging haha! 

### Continued development

Moving into future projects I would definitely like to learn more about CSS animations and the different transform properties. I felt like my understanding on how positioning could also improve, as I did take me a couple of hours to properly align the <img> element with the overlay <div>. 

### Useful resources

- [CSS Tricks](https://css-tricks.com/almanac/properties/t/transition/) - This really helped me understand the transition property. I also took a look at the pages for Tranform and Flexbox as well. 


## Author

- Frontend Mentor - [@wshelt21](https://www.frontendmentor.io/profile/wshelt21)
- Twitter - [@will_shelton21](https://twitter.com/will_shelton21)


## Acknowledgments

Would also like to shout out tsbsankara's YouTube channel and they video on this project for helping with identifying how to solve the image overlay problem here's a link the video for anyone who might get stuck on a particular section:
(https://www.youtube.com/watch?v=9bGbykdR4T8&t=1579s&ab_channel=tsbsankara)

