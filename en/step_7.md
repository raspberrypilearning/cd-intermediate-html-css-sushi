## Individual style

 Let's jazz up the homepage a bit! With another kind of CSS selector, you can apply a unique set of CSS rules to just **one specific element**.
 
+ Go to `index.html` and add the following **attribute** to the first paragraph tag:

```html
    <p id="myCoolText">
        My website is about Ireland.
    </p> 
```

The `id` is a name you give to **identify** this particular element. No two elements on a page should ever have the same `id`.

+ Now go to your stylesheet and add the following code

```css
    #myCoolText {
        color: rgb(0, 51, 102);
        border: 2px ridge rgb(204, 255, 255);
        padding: 15px;
        text-align: center;
    }
```
    
Here you're using an **ID selector**. You can tell because of the `#` in front of it.

Your text should look like this now:

![](images/paragraphIdStyle.png)

By giving an element an `id` and using an **ID selector** in your stylesheet, you can make **unique** CSS rules that just apply to that one specific thing on your website. 

+ Let's do one for the `body` of the homepage. Go to `index.html` and add an `id` to the `body` tag and one the `article` tag.

```html
    <body id="frontPage">
```

```html
    <article id="frontPageArticle">
```

+ In the stylesheet, add CSS rules for the body of the homepage.

```css
    #frontPage {
        background: #48D1CC;
        background: linear-gradient(#fea3aa, #f8b88b, #faf884, #baed91, #baed91, #b2cefe, #f2a2e8, #fea3aa);
    }
```

![Rainbow gradient background](images/frontPageIdStyles.png)
    
You just used a **gradient**! Note: The first `background` property sets a default colour for browsers that don't support gradients.

You can make lots of different effects with gradients. If you want to learn more, go to [dojo.soy/html2-css-gradients](http://dojo.soy/html2-css-gradients).


--- challenge ---

## Challenge: Style some more elements

+ Try giving another element an `id` and styling that element using the id selector with `#` as above. How about making one picture have a `border-radius` of `100%` so that it's fully rounded? Any other pictures on the website will stay the same as they are. 

Note that just like with CSS classes, the name you type in front of the CSS rules should **exactly** match the name you put in the element's `id` attribute.

--- hints ---

--- hint ---

You give an element an `id` by adding the `id` attribute to the HTML tag, like this: can make a CSS class that defines just the width of an element like this:

```html
  <img src="tito.png" id="titoPicture" alt="Tito the dog" />  		
```

Choose any name you like.

--- /hint ---

--- hint ---

To define style rules for a specific element, you use the `#` symbol, and the name that you gave the element for its `id`.

```css
  .titoPicture {
    border-radius: 100%;
    border: solid 1px white;
  }
```

--- /hint ---

--- /hints ---

![A round picture of Tito with a white border](images/frontPageStyleAll.png)

--- /challenge ---

