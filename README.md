# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow
- SASS

### What I learned

I don't know if that is the correct way, but I managed to do the hover effect like this.

```html
<div class="img">
    <div class="transparency">
         <svg width="48" height="48" xmlns="http://www.w3.org/2000/svg"><g fill="none" fill-rule="evenodd"><path d="M0 0h48v48H0z"/><path d="M24 9C14 9 5.46 15.22 2 24c3.46 8.78 12 15 22 15 10.01 0 18.54-6.22 22-15-3.46-8.78-11.99-15-22-15Zm0 25c-5.52 0-10-4.48-10-10s4.48-10 10-10 10 4.48 10 10-4.48 10-10 10Zm0-16c-3.31 0-6 2.69-6 6s2.69 6 6 6 6-2.69 6-6-2.69-6-6-6Z" fill="#FFF" fill-rule="nonzero"/></g></svg>
    </div>
</div>
```
```scss
.img {
        background-image: url(../img/image-equilibrium.jpg);
        height: 30rem;
        width: 100%;
        background-size: cover;
        background-position: center center;
        border-radius: 1rem;

        .transparency {
            width: 100%;
            height: 100%;
            display: flex;
            justify-content: center;
            align-items: center;

            svg {
                visibility: hidden;
            }
            
            &:hover {
                cursor: pointer;
                background-color: rgba(0, 255, 247,0.5);
                border-radius: 1rem;

                svg {
                    visibility: visible;
                }
            }
        }
    }
```

## Author

- Frontend Mentor - [@lucasscattolin](https://www.frontendmentor.io/profile/lucasscattolin)
- Twitter - [@lucasscattolin](https://www.twitter.com/lucasscattolin)
