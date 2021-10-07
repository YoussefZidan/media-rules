In this shot, I will share my experience with responsive design using css @media Rules.

Before you start adding responsiveness into your app, you have to ask yourself
"am I going to design the app in **Mobile-First Approach**  or **Desktop-First Approach**?"

> Mobile-First Approach is designing or developing an app for **Mobile** before designing for desktop web or any other device.

> Desktop-First Approach is designing or developing an app for **Dekstop** before designing for Mobiles or any other device.

Here are the **@media rules** that I personally use to fit all possible devices and screen sizes.
> Sizes from [Chrome device toolbar](https://developer.chrome.com/docs/devtools/device-mode/). 

## Desktop-first

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
With Desktop-first we use `max-width` and the order of the sizes from **larger** (at the top) to **smaller** (at the bottom).

## Mobile-first

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
With mobile-first, we use `min-width`, and the order of the sizes from **smaller** (at the top) to **larger** (at the bottom).
