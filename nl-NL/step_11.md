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

+ Laten we deze nieuwe `:hover` pseudo-class samen met een CSS class gebruiken om links te laten gloeien als je eroverheen beweegt! Voeg een link toe aan je webpagina en voeg een attribuut toe om de klasse naam op te geven. Vergeet niet, koppelingen zijn gedefinieerd met behulp van de `<a>` tag, zoals:

```html
    <p>
      Bezoek de <a class="niceLinks" href="https://en.wikipedia.org/wiki/Ireland">Wikipedia-pagina</a> om nog meer te leren over Ierland!
    </p>
```

+ Voeg de volgende code toe aan je style sheet en voer vervolgens je code uit om je mooie links in actie te zien.

```css
  .niceLinks {
    text-decoration: none;
    color: #FFFAF0;
  }
  .niceLinks:hover {
    color: #00FF7F;
  }
```

+ Waarom zou je ook niet het attribuut `class="niceLinks"` aan alle links in je menubalk toevoegen?

Je kunt al deze trucs ook combineren met animaties!

+ Zoek opnieuw het CSS-blok op voor de afbeelding van Tito (of welke afbeelding je eerder aan het bewerken was). Voeg de volgende code aan je style sheet bestand toe:

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

+ Kun je raden wat er zal gebeuren?

+ Roep nu "Rol om!" terwijl je de cursor over de afbeelding beweegt!

\--- challenge \---

## Uitdaging: gloeiende regenboog links maken

+ Kun je de `rainbowGlow` animatie van de vorige kaart gebruiken om ervoor te zorgen dat de koppelingen in je menu de kleuren blijven veranderen wanneer de cursor eroverheen zweeft?

\--- hints \---

\--- hint \---

Hieronder staat de code voor de `rainbowGlow` animatie. Er zijn vijf fasen gedefinieerd en in elke fase wordt een andere tekstkleur ingesteld. Je kunt meer toevoegen of wijzigen als je wilt!

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

Als je iets wilt animeren, voeg je zoals je hierboven hebt gedaan de drie `animatie` eigenschappen toe aan de stijlregels. Zorg er altijd voor dat de `animatienaam` overeen komt met de naam van de animatie die je wilt gebruiken.

\--- /hint \---

\--- hint \---

Je kunt `hover` effecten direct toevoegen aan het `nav` menu zoals dit:

```css
  nav ul li a:hover {
    animation-name: rainbowGlow;
    animation-duration: 1.5s;
    animation-iteration-count: infinite;
  }
```

Of, als je wilt dat andere links op je website ook in regenboogkleuren flitsen, kun je in plaats daarvan de animatie toevoegen aan de `.niceLinks` class, zoals deze:

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