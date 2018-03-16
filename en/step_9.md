## Sizing it up

Up until now you've been using **pixels** to set the size of things, e.g. `10px`. On this card you will learn about other measurements you can use.

+ Go to `index.html` and find the `img` element with the picture of Tito, or find another `img` tag on your website.

+ Delete the `width` attribute if it's there, and give the element an `id` of `imgTito`.

```html
  <img id="imgTito" src="tito.png" alt="Tito the dog" />
``` 

+ In your CSS file find the `#imgTito` code block and add the `width` property below:

```css
  #imgTito {
    border-radius: 100%;
    width: 50%;
  }
```

Note: 50% (50 percent) is **half**. 

+ Try resizing your browser window and watch what happens to the picture.

+ You should notice that the picture gets bigger and smaller when you make the window bigger and smaller. is much smaller now. That is because it is taking up `50%` (or **half**) of the width of the **main** element \(which is roughly the width of the page\).


--- collapse ---
---
title: How does it work?
---

When you set the size of something in pixels, you are setting an exact size and it doesn't change. This is called an **absolute** measurement. 

Another way to set the size of things is using **relative** measurements. That means how big elements are in relation to each other. So when one thing changes size, everything else will automatically change as well to keep the same **proportions**. 

If you set the `width` of an element to `100%`, that will make it be the same width as the container it's in.

When you're using **relative** measurements it's important to know what the **parent** of your element is. The **parent** is the thing that your element is inside, and that's what the measurement will be in relation to. For example, **parent** of the image above is the `article` element because the `img` element is in between the `<article></article>` tags.


--- /collapse ---

+ Experiment with different numbers in front of the `%`.

+ Before moving onto the next card, set the size of the Tito picture back to `100px` as well.
