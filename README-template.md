# Frontend Mentor - Recipe page solution

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Solution Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

## Overview

### Solution Screenshot

![](./assets/images/SolutionScreenShoot/Screenshot.svg)


### Links

- Solution URL: [Solution URL](https://github.com/hussaindev94/frontend-mentor-challenges-recipe-page)
- Live Site URL: [Live site URL](https://hussaindev94.github.io/frontend-mentor-challenges-recipe-page/)

## My process
I had taken mobile first approach do layout the desing and html layout, then I noted the differences between the three approaches mobile, tablet and desktop and change the properties by using media queiries.
### Built with

- Semantic HTML5 markup
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned


1. The hierarchy of a list make differences in designing it.
    * here are different layouts of a list:

      ```html
      <!-- 1 -->
      <ul>
        <li><span>Time: </span> about 10 mins</li>
      </ul>

      <!-- 2 -->
      <ul>
        <li><strong>Time: </strong> about 10 mins</li>
      </ul>

      <!-- 3 -->
      <ul>
        <li><div><span>Time: </span> about 10 mins<div></li>
      </ul>

      <!-- 4 -->
      <ul>
        <li><p><span>Time: </span> about 10 mins</p></li>
      </ul>
      ```
2. If the CSS file is constructed in a neasted approach, the media queries need to have the same level of cascading inorder to work and compete with the properties to decide which property will win.

3. The width value provided to the media query must be in px.
    ```css
    /*Padding inside the media will compete with the one in card-wrapper*/
    html{
      body{
        .section{
          .card-wrapper{
            padding: 40px
            @media (min-width: 768px){
              padding: 0;
            }
          }
        }
      }
    }
    /*This media will not work if the code nested*/
        html{
      body{
        .section{
          .card-wrapper{
            padding: 40px
          }
        }
      }
    }
    @media (min-width: 768px){
      padding: 0;
    }
    ```

### Continued development

I am not completely comfortable with the following:
1. Styling a list. I do not knew how to align the marker of a list with the design.
2. Styling tables. I am not comfortable with designing tables.


## Author

- Website - [Hussain Al-shaer](https://hussaindev94.github.io/Portfolio/)
- Frontend Mentor - [@hussaindev94](https://www.frontendmentor.io/profile/hussaindev94)
- Twitter - [@hussaindev94](https://x.com/hussaindev94)
