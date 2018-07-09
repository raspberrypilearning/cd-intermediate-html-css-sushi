## Leer Tito om te rollen!

Je kunt je website **interactiever** maken door coole dingen te laten gebeuren wanneer je met de muiscursor over dingen beweegt!

+ Zoek je CSS-regels voor de `img` elementen, of maak er een paar als je er geen hebt. Voeg een rand toe en voeg dan de hieronder staande nieuwe blok regels toe:

```css
  img {
    border: 2px solid White;
  }
  img:hover {
    border: 2px dashed Navy;
  }
```

Je hebt zojuist een speciaal type CSS-blok gebruikt dat een **pseudo-class** wordt genoemd.

## \--- collapse \---

## title: Hoe werkt het?

Een **pseudo-class** is een beetje anders dan een **class** die je zelf maakt. Je kunt het herkennen aan de `:`.

Pseudo-klassen zijn ingebouwde HTML-elementen: je kunt `:hover` stijlregels voor elk element, klasse of `id` selector toevoegen in je stylesheet zonder iets toe te voegen in je HTML-code.

\--- /collapse \---

+ Wat denk je dat het zal doen? Controleer welke pagina's op je website afbeeldingen bevatten (voeg een afbeelding toe als die er niet zijn!) En beweeg je cursor over een afbeelding om erachter te komen!

+ Laten we deze nieuwe `:hover` pseudo-class samen met een CSS class gebruiken om links te laten gloeien als je eroverheen beweegt! Add a link to your web page and include an attribute to specify the class name. Remember, links are defined using the `<a>` tag, like so:

```html
    <p>
      Visit the <a class="niceLinks" href="https://en.wikipedia.org/wiki/Ireland">Wikipedia page</a> to learn even more about Ireland!
    </p>
```

+ Add the following code to your style sheet, then run your code to see your lovely links in action.

```css
  .niceLinks {
    text-decoration: none;
    color: #FFFAF0;
  }
  .niceLinks:hover {
    color: #00FF7F;
  }
```

+ Why not add the attribute `class="niceLinks"` to all of the links in your menu bar as well?

You can combine all of these tricks with animations too!

+ Find the CSS block for the picture of Tito again (or whatever picture you were working on earlier). Add the following code to your style sheet file:

```css
  #titoPicture {
    border-radius: 100%;
    width: 100px;
  }
  #titoPicture:hover {
    animation-name: rollOver;
    animation-duration: 1s;
    animation-iteration-count: 1;
  }
  @keyframes rollOver {
    0% {
      transform: rotate(0deg);
    }
    100% {
      transform: rotate(-360deg);
    }
  }
```

+ Can you guess what will happen?

+ Now shout "Roll over!" as you move the cursor over the picture!

\--- challenge \---

## Challenge: make glowing rainbow links

+ Can you use the `rainbowGlow` animation from the previous card to make the links in your menu keep changing colours when the cursor is hovering over them?

\--- hints \---

\--- hint \---

Below is the code for the `rainbowGlow` animation. It has five stages defined, and it sets a different text colour at each stage. You can add more or change them however you want!

```css
    @keyframes rainbowGlow {
        0% {
            color: #00BFFF;
        }
        25% {
            color: #00FF7F;
        }
        50% {
            color: #eeeeaf;
        }
        75% {
            color: #eeafee;
        }
        100% {
            color: #00BFFF;
        }
    }
```

\--- /hint \---

\--- hint \---

To animate something, you add the three `animation` properties to its style rules as you've done above. Always make sure the `animation-name` matches the name of the animation you wish to use.

\--- /hint \---

\--- hint \---

You can add `hover` effects directly to the `nav` menu like this:

```css
  nav ul li a:hover {
    animation-name: rainbowGlow;
    animation-duration: 1.5s;
    animation-iteration-count: infinite;
  }
```

Or, if you want to make other links on your website flash rainbow colours too, you can add the animation to the `.niceLinks` class instead, like this:

```css
  .niceLinks:hover {
    color: #00BFFF;
    animation-name: rainbowGlow;
    animation-duration: 1.5s;
    animation-iteration-count: infinite;
  }
```

\--- /hint \---

\--- /hints \---

\--- /challenge \---

![](images/badge-footer-image-html-intermed.png)