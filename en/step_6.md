## Design some themes

Let's design a theme for the Attractions page that's different from the other pages. 

+ Go to your stylesheet file and add the following. Be sure to include the dot in front!
  
```css
  .greenBackground {
      background-color: #48D1CC;
  }
```

The dot makes this into a **class selector**. With a CSS **class** you can apply a set of CSS rules to any element on your website by adding an **attribute** to the element.

+ Now go to `attractions.html` \(or the page you're working on if you're using your own project\) and add the following **attribute** to each `section` tag:

```html
  <section class="greenBackground">
```

You should see the background change around the text on the page.

+ Look at how your web page looks now and compare it to the other pages that have `section` elements.

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

--- collapse ---
---
title: How does it work?
---

When you use a CSS **element selector** such as `section`, the style rules apply to **all** the elements of that type on your website. With CSS **classes** you're able to just change **some** of them. 

You can add more than one class to an element too; in fact, you can add as many CSS CSS classes to an element as you like. Just write the names of all the classes you want to use inside the **class attribute**, and separate them with spaces.

--- /collapse ---

+ Let's give the Food page a makeover! \(If you're using your own website, you'll need another page with some **sections** on it\) Add the following classes to your stylesheet:

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

+ Go to the `food.html` file \(or your own file\) and add the new classes as well as the `.sectionSpacing` class to each section:

```html
  <section class="yellowBackground sectionSpacing solidRoundBorders">
```

Notice how you can mix and match the classes in your element's `class` attribute? Using CSS classes lets you **reuse** the same set of style rules on lots of elements. You can apply them to any element that has the properties you've set. 

+ Go to `index.html` and add the `solidRoundBorders` class to the picture of Tito, or another picture on your website.

```html
    <img class="solidRoundBorders" src="tito.png" alt="Tito the dog" width="100px" />
```

--- challenge ---

## Challenge: Make some new classes

+ Why not experiment with some more CSS classes to make the other pages have their own themes? You can name a CSS class anything you like. It's common to give it a name that describes what it does or what it's for!

+ As an extra challenge, use CSS **classes** to define a few different picture sizes for your website, for example `.smallPictures` and `.mediumPictures`. Then remove the `width` attribute from each of your `img` elements and add the appropriate class instead.

--- /challenge ---