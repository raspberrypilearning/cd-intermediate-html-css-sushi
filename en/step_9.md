## Sizing it up

Up until now you've been using **pixels** to set the size of things, e.g. `10px`. This is called an **absolute** measurement. It means you set an exact size and it doesn't change. Another way to set the size of things is using **relative** measurements. That means how big elements are in relation to each other. So when one thing changes size, everything else will automatically change as well to keep the same **proportions**. 

+ Go to `index.html` and find the `img` element with the picture of Tito. Delete the width attribute if `width="100px"` if it's there, and give the element an `id` of `imgTito`.

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

+ 50% (50 percent) is **half**. Try a few different percentages and see if you can work out what it's doing.

When you're using **relative** measurements it's important to know what the **parent** of your element is. The **parent** is the thing that your element is inside, and that's what the measurement will be in relation to. For example, **parent** of the image above is the `article` element because the `img` element is in between the `<article></article>` tags.

+ Now in your html file, put the image inside a `section` element with `id` `titoSection`. Include some text in the section too. 

```html
  <section id="titoSection">
    <img id="imgTito" src="tito.png" alt="Tito the dog" />  		
    <p>
      This is Tito. He will be your tourguide! As you can see, Tito loves CoderDojo.
    </p>
  </section>
```

+ Add the following code to your stylesheet, so you can see what's going on more clearly

```css
  #titoSection {
    width: 200px;
    background-color: white;
  }
```

If you don't give **section** elements a width, they fill up all the space available, which is usually a good thing!

+ You should notice that the picture is much smaller now. That is because it is taking up 50% of the width of the **section** element instead of the **article** element \(which is roughly the width of the page\).

+ Experiment with different `%` values for the size of the picture.

+ Before moving onto the next card, delete the `section` tags you added around the image and also delete the `#titoSection` CSS block! Set the size of the Tito picture back to `100px` as well.
