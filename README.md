Here are the [@media Rules](https://www.w3schools.com/cssref/css3_pr_mediaquery.asp) that I personally use to fit all possible devices and screen sizes.

> Sizes from Chrome device toolbar.

``` css
/* ================ Desktop First ================ */

/* Any other bigger devices */

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

/* ================ Mobile First ================ */

/* Any other smaller devices */

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
