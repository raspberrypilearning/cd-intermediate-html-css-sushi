## Animation

+ Go to the bottom of your CSS file and add the following code

```css
    @keyframes myFirstAnimation {
        from {
            width: 100px;
        }
        to {
            width: 300px;
        }
    }
```

This code creates an animation called `myFirstAnimation` that you can add to any element on your website. What do you think it will do?

+ Find your CSS rules for the ID `#imgTito` and add the following three properties:

```css
    animation-name: myFirstAnimation;
    animation-duration: 2s;
    animation-iteration-count: 1;
```

+ Watch what happens on your web page! Try different values for `animation-iteration-count` to see what it does.

+ Let's try another animation! Add the following code to the end of your CSS file:

```css
    @keyframes glowPulse {
        0% {
            color: DeepSkyBlue;
        }
        50% {
            color: LightGreen;
        }
        100% {
            color: DeepSkyBlue;
        }
    }
```
   
+ Now find the `#myCoolText` CSS rules from earlier and add in the animation code:

```css
    #myCoolText {
            animation-name: glowPulse;
            animation-duration: 1.5s;
            animation-iteration-count: 1;
    }
```

When you use **percentages** instead of `from` and `to`, you're able to set in between values as well as just start and end values. You can set as many in between values as you like using different percentages. 

+ Try adding in more colours to the glowing sequence above, for example at `25%` and `75%`!



+ Change the value of `animation-iteration-count` to `infinite`. What do you think will happen? 

+ You can also play with different values for `animation-duration` to speed up or slow down your animation.

+ One final trick! Add this animation code:

```css
    @keyframes slide {
    0% {
        background-position-x: 0;
    }
    100% {
        background-position-x: 600vw;
    }
    }
```

+ Now find the `#frontPage` CSS rules from earlier and change them to:

```css
    #frontPage {
        background: repeating-linear-gradient(-45deg, red 0%, yellow 7.14%, lime 14.28%, cyan 21.42%, cyan 28.56%, blue 35.7%, magenta 42.84%, red 50%);
        background-size: 600vw 600vw;
        animation: slide 10s infinite linear forwards;
    }
```

Don't worry about understanding all of the code above... just sit back and enjoy!!

+ Try making your own new animation using the `@keyframes` keyword and a name that you choose. How about animating your nav menu? To learn about more things you can do with animation, visit [dojo.soy/html2-css-animation](http://dojo.soy/html2-css-animation). Have fun!


--- hints ---

--- hint ---

You create an animation using the `@keyframes` keyword. Choose a name for your animation and then create a bunch of style rules for each different stage of the animation using the `from` and `to` keywords or using `%` values as above.

This example has five different stages defined, and it sets a different text colour at each stage:

```css
    @keyframes rainbowGlow {
        0% {
            color: DeepSkyBlue;
        }
        25% {
            color: LightGreen;
        }
        50% {
            color: #eeeeaf;
        }
        75% {
            color: #eeafee;
        }
        100% {
            color: DeepSkyBlue;
        }
    }
```
   
--- /hint ---


--- hint ---

To animate something, you add the three `animation` properties to the style rules of it as you've done above, making sure the `animation-name` matches the name of the animation you wish to use.

--- /hint ---

--- hint ---

You can add hover effects directly to the nav menu like this:

```css
    nav ul li a:hover {
    animation-name: rainbowGlow;
    animation-duration: 1.5s;
    animation-iteration-count: infinite;
    }
```

--- /hint ---

--- /hints ---

