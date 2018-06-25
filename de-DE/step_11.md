## Bringe Tito bei, sich umzudrehen!

Sie können Ihre Website mehr machen **interaktive** , indem sie coole Sachen passieren , wenn man über die Dinge mit dem Mauszeiger bewegen!

+ Finden Sie Ihre CSS-Regeln für die `Elemente img` oder erstellen Sie einige, wenn Sie keine haben. Fügen Sie einen Rahmen hinzu und fügen Sie anschließend einen neuen Block mit Regeln hinzu:

```css
  img {Grenze: 2px einfarbig weiß; } img: hover {border: 2px gestrichelt Navy; }
```

Sie haben gerade einen speziellen CSS-Block namens **Pseudo-Klasse**.

## \--- Einsturz \---

## Titel: Wie funktioniert es?

Eine **-Pseudoklasse** sich ein wenig von einer **Klasse** , die Sie selbst erstellen. Du kannst es am `:`.

Pseudoklassen werden in HTML-Elemente eingebaut: Sie können `:` Stilregeln zu jedem Element-, Klassen- oder `ID-` Selektor in Ihrem Stylesheet hinzufügen, ohne dass Sie etwas extra in Ihrem HTML-Code hinzufügen müssen.

\--- / einklappen \---

+ Was denkst du wird passieren? Überprüfen Sie, auf welchen Seiten Ihrer Website Bilder vorhanden sind (fügen Sie ein Bild hinzu, wenn es keine gibt!), Und bewegen Sie den Mauszeiger über ein Bild, um es herauszufinden!

+ Lassen Sie uns diese neue Pseudo-Klasse `: hover` zusammen mit einer CSS-Klasse verwenden, um Links zum Leuchten zu bringen, wenn Sie den Mauszeiger darüber bewegen! Fügen Sie einen Link zu Ihrer Webseite hinzu und fügen Sie ein Attribut hinzu, um den Klassennamen anzugeben. Denken Sie daran, Links werden wie folgt mit dem Tag `<a>` definiert:

```html
    <p>
      Besuchen Sie die <a class="niceLinks" href="https://en.wikipedia.org/wiki/Ireland">Wikipedia-Seite</a> , um noch mehr über Irland zu erfahren!
    </p>
```

+ Fügen Sie Ihrem Stylesheet den folgenden Code hinzu, und führen Sie dann Ihren Code aus, um Ihre schönen Links in Aktion zu sehen.

```css
  .niceLinks {Textdekoration: keine; Farbe: # FFFAF0; } .niceLinks: hover {color: # 00FF7F; }
```

+ Warum nicht das Attribut `class = "niceLinks"` zu allen Links in der Menüleiste hinzufügen?

Sie können alle diese Tricks auch mit Animationen kombinieren!

+ Suchen Sie erneut den CSS-Block für das Bild von Tito (oder das Bild, an dem Sie zuvor gearbeitet haben). Fügen Sie Ihrer Stylesheet-Datei den folgenden Code hinzu:

```css
  #titoPicture {border-radius: 100%; Breite: 100px; } #titoPicture: hover {animationsname: rollOver; Animationsdauer: 1s; Animations-Iterationszählung: 1; } @keyframes rollOver {0% {transform: rotieren (0deg); } 100% {transformiere: rotiere (-360deg); }}
```

+ Kannst du raten, was passieren wird?

+ Schreie jetzt "Roll over!" während du den Cursor über das Bild bewegst!

\--- Herausforderung \---

## Herausforderung: leuchtende Regenbogenlinks machen

+ Kannst du die `rainbowGlow` Animation von der vorherigen Karte verwenden, damit die Links in deinem Menü die Farben ändern, wenn der Cursor über ihnen schwebt?

\--- Hinweise \---

\--- Hinweis \---

Unten ist der Code für die Animation `rainbowGlow`. Es ist in fünf Stufen definiert und legt in jeder Phase eine andere Textfarbe fest. Sie können mehr hinzufügen oder sie ändern, wie Sie wollen!

```css
    @keyframes rainbowGlow {0% {farbe: # 00BFFF; } 25% {Farbe: # 00FF7F; } 50% {Farbe: #eeeeaf; } 75% {Farbe: #eeafee; } 100% {Farbe: # 00BFFF; }}
```

\--- /Hinweis \---

\--- Hinweis \---

Um etwas zu animieren, fügen Sie seinen Style-Regeln die drei `Animations-` Eigenschaften hinzu, wie Sie es oben getan haben. Stellen Sie immer sicher, dass der `Animationsname` mit dem Namen der Animation übereinstimmt, die Sie verwenden möchten.

\--- /Hinweis \---

\--- Hinweis \---

Sie können `hover` Effekte direkt zum `nav` Menü hinzufügen:

```css
  nav ul li a: schweben {animationsname: rainbowGlow; Animationsdauer: 1.5s; Animation-Iterationszählung: unendlich; }
```

Oder wenn Sie andere Links auf Ihrer Website auch mit Regenbogenfarben versehen möchten, können Sie die Animation stattdessen zur Klasse `.niceLinks` hinzufügen:

```css
  .niceLinks: hover {color: # 00BFFF; Animationsname: RainbowGlow; Animationsdauer: 1.5s; Animation-Iterationszählung: unendlich; }
```

\--- /Hinweis \---

\--- / Hinweise \---

\--- /Herausforderung \---

![](images/badge-footer-image-html-intermed.png)