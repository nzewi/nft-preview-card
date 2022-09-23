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
  
- [Author](#author)


## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![Screenshot](/images/sreenshot.png)

### Links

- Solution URL: [solution URL](https://github.com/nzewi/nft-preview-card)
- Live Site URL: [live site URL](https://nzewi.github.io/nft-preview-card)

## My process

### Built with

- Semantic HTML5 markup
- Flexbox
- Mobile-first workflow


### What I learned

I learnt how to add an overlay to an image on hover

```html
<div class="card__img-container">
        <img src="images/image-equilibrium.jpg" alt="Equilibrium cube" class="card__img">
        <div class="card__img-overlay">
          <svg class="card__img-overlay-icon" width="48" height="48" xmlns="http://www.w3.org/2000/svg"><g fill="none" fill-rule="evenodd"><path d="M0 0h48v48H0z"/><path d="M24 9C14 9 5.46 15.22 2 24c3.46 8.78 12 15 22 15 10.01 0 18.54-6.22 22-15-3.46-8.78-11.99-15-22-15Zm0 25c-5.52 0-10-4.48-10-10s4.48-10 10-10 10 4.48 10 10-4.48 10-10 10Zm0-16c-3.31 0-6 2.69-6 6s2.69 6 6 6 6-2.69 6-6-2.69-6-6-6Z" fill="#FFF" fill-rule="nonzero"/></g></svg>
        </div>
        
      </div>
```
```css

.card__img-container {
  position: relative;
  border-radius: 1.2rem;
  overflow: hidden;
}

.card__img-container:hover {
  cursor: pointer;
}

.card__img-overlay {
  height: 100%;
  width: 100%;
  opacity: 0;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);

  transition: .5s ease;
}

.card__img-overlay:hover {
  opacity: 1;
  background-color: hsla(178, 100%, 50%, 0.65) ;
}

.card__img-overlay-icon {
  position: absolute;
  top: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  
}
}
```

### Continued development

- I want to keep working on my flexbox and absolute positioning.


## Author

- Frontend Mentor - [@nzewi](https://www.frontendmentor.io/profile/nzewi)
- Twitter - [@nelson_nzewi](https://www.twitter.com/nelson_nzewi)

