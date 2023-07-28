# Frontend Mentor - 3-column preview card component solution

This is a solution to the [3-column preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/3column-preview-card-component-pH92eAR2-). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

![Screenshot1](/images/Screenshot1.png)
![Screenshot2](/images/Screenshot%202023-07-28%20at%2013-11-52%20Frontend%20Mentor%203-column%20preview%20card%20component.png)
![Screenshot3](/images/Screenshot%203-column-preview%20button%20hover.png)


### Links

- Solution URL: [https://github.com/jeeheezy/FEM-3-Column-Preview-Card-Component](https://github.com/jeeheezy/FEM-3-Column-Preview-Card-Component)
- Live Site URL: [https://jeeheezy.github.io/FEM-3-Column-Preview-Card-Component/](https://jeeheezy.github.io/FEM-3-Column-Preview-Card-Component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow


### What I learned

I learned how to make use of CSS custom properties, as well as how CSS applies when there's multiple classes applied on one element. 

Specifically for the button (not on hover), the background color is white while the text color is the same as the background color of the element behind it (the boxes). I didn't want to 
create a new class for each of the button to specify different colors, but applying multiple classes didn't work well here either since contradictory properties resulted in ways I didn't want
(e.g. background-color property of the class "sedan" would conflict with the white background-color of class "button"). My friend taught me about custom properties which then could be inherited 
and applied to different properties with var(), so that I could use the classes I had already without introducing conflicting properties.
Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge.

```html
<div class="flex-container">
    <div class="sedans box">
      <button class="button">Learn More</button>
    </div>
</div>
```
```css
/* Thought about using mask for transparency effect but seems overkill here*/
.button {
    margin-top: 50px;
    background-color: hsl(0, 0%, 95%);
    padding: 10px 20px;
    border-radius: 25px;
    border: none;
    font-family: 'Lexend Deca', sans-serif;
    font-weight: 400;
    /*Handy trick by inherting a custom property to set as the color*/
    color: var(--sectioncolor);
    cursor: pointer;
}

.sedans {
    background-color: hsl(31, 77%, 52%);
    --sectioncolor: hsl(31, 77%, 52%);
}
```

### Continued development

Flexbox and the general way CSS are applied are things I need more practice with. I also want to see what other ways there are to using CSS custom properties since it seems like a very powerful tool.


## Author

- LinkedIn - [https://www.linkedin.com/in/jeeho-lee-719852182/](https://www.linkedin.com/in/jeeho-lee-719852182/)
- Frontend Mentor - [@jeeheezy](https://www.frontendmentor.io/profile/jeeheezy)

