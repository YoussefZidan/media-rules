In this article I will share with you my experience with responsive design using css [@media Rules](https://www.w3schools.com/cssref/css3_pr_mediaquery.asp).

Before you start adding responsiveness into your app, You have to ask your self:
Am I going to design the app in **Mobile First**  or **Desktop First**?

Here are the @media rules that I personally use to fit all possible devices and screen sizes.

> Sizes from Chrome device toolbar.

## Desktop First

``` css
/* ================ Desktop First ================ */

/* Any other bigger devices */
body {
  background: brown;
}

/* Ultra HD */
@media (max-width: 3840px) {
  body {
    background: red;
  }
}
/* Full HD */
@media (max-width: 2560px) {
  body {
    background: blue;
  }
}
/* Labtop L*/
@media (max-width: 1440px) {
  body {
    background: green;
  }
}
/* Labtop */
@media (max-width: 1024px) {
  body {
    background: cyan;
  }
}
/* Tablet */
@media (max-width: 768px) {
  body {
    background: purple;
  }
}
/* Mobile */
@media (max-width: 425px) {
  body {
    background: yellow;
  }
}
```
With Desktop First we use `max-width` and the sizes order from bigger (at the top) and smaller (at the bottom).

## Mobile First

```css

/* ================ Mobile First ================ */

/* Any other smaller devices */
body {
  background: brown;
}

/* Mobile */
@media (min-width: 425px) {
  body {
    background: yellow;
  }
}
/* Tablet */
@media (min-width: 768px) {
  body {
    background: purple;
  }
}
/* Labtop */
@media (min-width: 1024px) {
  body {
    background: cyan;
  }
}
/* Labtop L*/
@media (min-width: 1440px) {
  body {
    background: green;
  }
}
/* Full HD */
@media (min-width: 2560px) {
  body {
    background: blue;
  }
}

/* Ultra HD */
@media (min-width: 3840px) {
  body {
    background: red;
  }
}
```
With Mobile First we use `min-width` and the sizes order from smaller (at the top) and bigger (at the bottom).
