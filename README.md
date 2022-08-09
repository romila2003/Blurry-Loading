# Blurry-Loading

This is apart of the 50 projects in 50 days challenge and is the fifth project.

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

- To create a blurry loading page that changes from blurry to normal whilst the percentage increases to 100%. The challenge involves HTML, CSS and Javascript.

### Screenshot

# Mobile Preview 

![screenshot](https://github.com/romila2003/Blurry-Loading/blob/main/Mobile%20preview.PNG)


# Desktop Preview 

![screenshot](https://github.com/romila2003/Blurry-Loading/blob/main/Desktop%20previe.PNG)


### Links

 - Source code: [https://github.com/romila2003/Blurry-Loading](https://github.com/romila2003/Blurry-Loading)
 - Live website: [https://blurry-loading-main.netlify.app/](https://blurry-loading-main.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- Plain CSS
- Vanilla Javascript
- Flexbox

### What I learned

I worked with the blurring effect and incremented the numbers so that the blur fades as the number gets closer to 100%. I also learned a new concept of `scale`.

Javascript - scale:

```javascript

function blurring() {
    load++;

    if(load > 99) {
        clearInterval(int)
    }

    loadText.innerText = `${load}%`;
    loadText.style.opacity = scale(load, 0, 100, 1, 0);
    bg.style.filter = `blur(${scale(load, 0, 100, 30, 0)}px)`
}

const scale = (num, in_min, in_max, out_min, out_max) => {
    return ((num - in_min) * (out_max - out_min)) / (in_max - in_min) + out_min
}

```

### Continued development

For future developments, I should learn more concepts of javascript and implement those within new projects.


## Author

- Twitter - [@romila003](https://www.twitter.com/romila003)
- Frontend Mentor - [@romila2003](https://www.frontendmentor.io/profile/romila2003)
