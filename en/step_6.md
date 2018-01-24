## Design some themes

On this card you will learn how to apply different sets of style rules to elements of the same type and create a different theme for each page on your website!

+ Go to your stylesheet file and add the following. Be sure to include the dot in front!
  
```css
  .greenBackground {
      background-color: #48D1CC;
  }
```

+ Now go to `attractions.html` \(or the page you're working on if you're using your own project\) and add the following **attribute** to each `section` tag:

```html
  <section class="greenBackground">
```

You should see the background change around the text on the page. Congratulations – you've just used your first **CSS class**!

+ Look at how your web page looks now and compare it to the other pages that have `section` elements.

--- collapse ---
---
title: How does it work?
---

Remember that when you use a CSS **selector** such as `section` or `p` or `nav ul`, the style rules apply to **all** the elements of that type on your website. That's not always what you want.

With CSS **classes** you're able to just change **some** of them. 

Putting a dot in front of your selector makes it into a **class selector**. A class can have any name, it doesn't have to be the name of a HTML element.

```css
  .myAwesomeClass {
    /* my cool style rules go here */
  }
```

You choose which elements the style rules apply to by adding the `class` **attribute** to those elements, in the HTML code. You put the name of the class in as the value for the attribute, **without** the dot, like this:

```html
  class="myAwesomeClass"
```

--- /collapse ---

--- collapse ---
---
title: Stuff to rewrite or cut out
---

The class can contain any rules you like. Sometimes you might make a bunch of CSS classes that each do only one or two things.

You can add more than one class to an element too; in fact, you can add as many CSS CSS classes to an element as you like. Just write the names of all the classes you want to use inside the `class` attribute, and separate them with spaces.

Sometimes you might make a CSS class that does only one thing. For example, you might want to easily apply the same borders to several different elements. On some of those elements, maybe you also want to make the text stand out, but not on others. In that case you would make one CSS class that defines the border styling, and another that defines the text styling. You can apply any or both of the classes to whichever elements you like on your website.

- note about using them to separate different parts of the styling? don't have to define **all** the rules for an element, just a particular set that you might want to reuse on other elements ???

--- /collapse ---

+ Let's make another CSS **class** to give the sections some margin and padding. In `styles.css`, add the following code:

```css
  .sectionSpacing {
    padding: 10px;
    margin-top: 20px;
  }
```

+ In the `html` page you were working on, add the new class to each of the sections like this:

```html
  <section class="greenBackground sectionSpacing">
```

You can apply as many CSS classes to an element as you like. Just write the names of all the classes you want to use inside the `class` attribute (remember, without the dot!), separating them with spaces.

+ Let's give another page a makeover! Add the following classes to your stylesheet:

```css
  .yellowBackground {
    background-color: #FFFFCC;
    color: #A52A2A;
  }

  .solidRoundBorders {
    border-style: solid;
    border-width: 2px;
    border-color: #F5FFFA;
    border-radius: 10px;
  }
```

+ Go to the `food.html` file \(or, if you're using your own website, you'll need another `html` file with some **sections** on it\) and add the new classes as well as the `.sectionSpacing` class to each section:

```html
  <section class="yellowBackground sectionSpacing solidRoundBorders">
```

Using CSS classes lets you **reuse** the same set of style rules on lots of elements. They don't even have to be the same type of element: you can apply the same class to any element that has the properties you've set in that class. 

+ Go to `index.html` and add the `solidRoundBorders` class to the picture of Tito, or another picture on your website.

```html
    <img class="solidRoundBorders" src="tito.png" alt="Tito the dog" width="100px" />
```

--- challenge ---

## Challenge: Make some new classes


Choose another page and design some different styles for the elements on that page. You could use some of the same CSS classes 

+ Why not experiment with some more CSS classes to make the other pages have their own themes? You can name a CSS class anything you like. It's common to give it a name that describes what it does or what it's for!

+ Try applying the classes to other elements too, such as `<article>` or `<p>`.

+ As an extra challenge, use CSS **classes** to define a few different picture sizes for your website, for example `.smallPictures` and `.mediumPictures`. Then remove the `width` attribute from each of your `img` elements and add the appropriate class instead.

--- /challenge ---