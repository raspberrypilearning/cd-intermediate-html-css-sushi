## Animatie

Wist je dat je CSS kunt gebruiken om dingen te laten bewegen? Hoe zul je leren op deze kaart!

+ Voordat je begint, zorg ervoor dat je een afbeelding op je website hebt met een `id` en een bijbehorende CSS blok welke de `with` instelt op `100 pixels`. Ik gebruik het beeld van Tito van hiervoor, en mijn CSS blok ziet er als volgt uit:

```css
    #titoPicture {
        border-radius: 100%;
        width: 100px;
    }
```

+ Ga naar de onderkant van je CSS bestand en voeg de volgende code toe:

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

Deze code maakt een animatie met de naam `myFirstAnimation` (mijnEertseAnimatie) aan die je aan elk element op je website kunt toevoegen. Wat denk je dat het zal doen?

+ Zoek je CSS regels voor de afbeelding en voeg de volgende drie eigenschappen toe:

```css
    animation-name: myFirstAnimation;
    animation-duration: 2s;
    animation-iteration-count: 1;
```

+ Bekijk nu wat er gebeurt op je webpagina! Try different values for `animation-iteration-count` to see what it does.

+ Let's try another animation! Add the following code to the end of your CSS file:

```css
    @keyframes rainbowGlow {
        0% {
            color: #FFD700;
        }
        50% {
            color: #663399;
        }
        100% {
            color: #FFD700;
        }
    }
```

+ Now find the `#myCoolText` CSS rules from earlier and add in the animation code:

```css
    #myCoolText {        
        color: #003366;
        border: 2px ridge #ccffff;
        padding: 15px;
        text-align: center;
        animation-name: rainbowGlow;
        animation-duration: 1.5s;
        animation-iteration-count: 1;
    }
```

When you use **percentage values** instead of `from` and `to`, you're able to set in-between values as well as just start and end values. You can set as many in-between values as you like using different percentage values from `0` all the way up to `100`.

+ Change the value of `animation-iteration-count` to `infinite`. See if you can guess what will happen before you test it!

+ Try out different values for `animation-duration` to speed up or slow down your animation.

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

+ Now find the `#frontPage` CSS rules you wrote earlier and change them to:

```css
    #frontPage {
        background: repeating-linear-gradient(-45deg, red 0%, yellow 7.14%, lime 14.28%, cyan 21.42%, cyan 28.56%, blue 35.7%, magenta 42.84%, red 50%);
        background-size: 600vw 600vw;
        animation: slide 10s infinite linear forwards;
    }
```

Don't worry about understanding all of the code above... just sit back and enjoy!!

To learn about more things you can do with animation, visit [this web page](http://dojo.soy/html2-css-animation){:target="_blank"}. Have fun!

On the next card you'll learn how to make cool things happen when you hover the mouse cursor over things!