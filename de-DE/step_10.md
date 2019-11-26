## Bringe Tito bei, sich zu drehen!

Du kannst Deine Website **interaktiver** gestalten, indem du coole Sachen passieren lässt, wenn Du mit dem Mauszeiger über Dinge schwebst!

+ Suche Deine CSS-Regeln für die `img ` Elemente oder erstelle welche, falls Du keine hast. Füge einen Rand (border) hinzu und füge dann einen neuen Regelblock direkt darunter hinzu:

```css
  img {
    border: 2px solid White;
  }
  img:hover {
    border: 2px dashed Navy;
  }
```

Du hast gerade einen speziellen CSS-Block Typ verwendet, der **Pseudoklasse** genannt wird.

## \--- collapse \---

## title: Wie funktioniert das?

Eine **Pseudoklasse** ist ein bisschen anders, als eine **Klasse** die Du selbst erzeugst. Du kannst sie am `:` erkennen.

Pseudoklassen sind In HTML-Elementen schon integriert: Du kannst jedem Element, jeder Klasse oder jedem `id` Selektor in Deinem Stylesheet `:hover` (engl.: schweben) Stilregeln hinzufügen, ohne dass Du zusätzliche Elemente in Deinen HTML-Code einfügen musst.

\--- /collapse \---

+ Was glaubst du, wird passieren? Überprüfe, auf welchen Seiten Deiner Website Bilder angezeigt werden (füge ein Bild hinzu, falls es keine gibt!), bewege dann den Mauszeiger über ein Bild, um es herauszufinden!

+ Lass uns diese neue `:hover` Pseudoklasse zusammen mit einer CSS-Klasse verwenden, um Links leuchten zu lassen, wenn du über ihnen schwebst! Füge einen Link zu Deiner Webseite hinzu und füge ein Attribut hinzu, um den Klassennamen anzugeben. Denk daran, Links werden mit dem `<a>` Tag definiert, und zwar so:

```html
    <p>
      Besuche die <a class="niceLinks" href="https://de.wikipedia.org/wiki/Irland">Wikipedia-Seite</a> um noch mehr über Irland zu erfahren!
    </p>
```

+ Füge den folgenden Code zu Deinem Stylesheet hinzu und führe dann Deinen Code aus, um Deine schönen Links in Aktion zu sehen.

```css
  .niceLinks {
    text-decoration: none;
    color: #FFFAF0;
  }
  .niceLinks:hover {
    color: #00FF7F;
  }
```

+ Warum fügst Du das `class="niceLinks"` Attribut nicht auch gleich zu allen Links in Deiner Menüleiste hinzu?

Du kannst all diese Tricks auch mit Animationen kombinieren!

+ Such nochmal den CSS-Block für das Bild von Tito (oder für das Bild, an dem Du vorhin gearbeitet hast). Füge folgenden Code in dein Sylesheet ein:

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

+ Kannst Du dir vorstellen, was passieren wird?

+ Rufe jetzt "Roll dich!", während Du den Mauszeiger über das Bild bewegst!

\--- challenge \---

## Herausforderung: Erstelle leuchtende Regenbogen Links

+ Kannst du die `rainbowGlow` Animation von der vorherigen Karte verwenden, um zu bewirken, dass die Links in deinem Menü ihre Farben ändern, wenn sich der Mauszeiger darüber befindet?

\--- hints \---

\--- hint \---

Unten ist der Code für die `rainbowGlow` Animation. Es sind fünf Stufen definiert und in jeder Stufe wird eine andere Textfarbe festgelegt. Du kannst mehr hinzufügen oder sie ändern, wie Du willst!

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

\---/hint\---

\--- hint \---

Um etwas zu animieren, fügst Du die drei `animation` Eigenschaften zu den Stilregeln hinzu, wie Du es oben schon getan haben. Achte immer darauf, dass `animation-name` mit dem Namen der Animation übereinstimmt, die Du verwenden möchtest.

\---/hint\---

\--- hint \---

Du kannst `hover` Effekte direkt zum `nav` Menü wie folgt hinzufügen:

```css
  nav ul li a:hover {
    animation-name: rainbowGlow;
    animation-duration: 1.5s;
    animation-iteration-count: infinite;
  }
```

Oder, wenn Du auch andere Links auf Deiner Website in Regenbogenfarben blinken lassen möchtest, kannst Du die Animation, stattdessen der `.niceLinks` Klasse hinzufügen, wie folgt:

```css
  .niceLinks:hover {
    color: #00BFFF;
    animation-name: rainbowGlow;
    animation-duration: 1.5s;
    animation-iteration-count: infinite;
  }
```

\---/hint\---

\---/hints\---

\--- /challenge \---

![](images/badge-footer-image-html-intermed.png)