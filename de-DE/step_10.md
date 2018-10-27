## Animation

Wussten Sie, dass Sie CSS verwenden können, um Dinge in Bewegung zu bringen? Du wirst lernen, wie auf dieser Karte!

+ Bevor Sie beginnen, stellen Sie sicher, dass Sie ein Bild auf Ihrer Website mit einer `ID` und einem entsprechenden CSS-Block haben, der die `Breite` auf `100px`. Ich gehe mit dem Bild von Tito von vor, und mein CSS-Block sieht so aus:

```css
    #titoPicture {border-radius: 100%; Breite: 100px; }
```

+ Gehen Sie zum Ende Ihrer CSS-Datei und fügen Sie den folgenden Code hinzu:

```css
    @keyframes myFirstAnimation {von {width: 100px; } bis {Breite: 300px; }}
```

Dieser Code erstellt eine Animation mit dem Namen `myFirstAnimation` , die Sie zu einem beliebigen Element auf Ihrer Website hinzufügen können. Was denkst du wird es tun?

+ Suchen Sie Ihre CSS-Regeln für das Bild und fügen Sie die folgenden drei Eigenschaften hinzu:

```css
    Animationsname: myFirstAnimation; Animationsdauer: 2s; Animations-Iterationszählung: 1;
```

+ Jetzt schau dir an, was auf deiner Webseite passiert! Probieren Sie verschiedene Werte für `animation-iteration-count` zu sehen, was es tut.

+ Lass uns eine andere Animation ausprobieren! Fügen Sie am Ende Ihrer CSS-Datei den folgenden Code hinzu:

```css
    @keyframes rainbowGlow {0% {farbe: # FFD700; } 50% {Farbe: # 663399; } 100% {Farbe: # FFD700; }}
```

+ Finde jetzt die `#myCoolText` CSS-Regeln von früher und füge den Animationscode hinzu:

```css
    #myCoolText {Farbe: # 003366; Grenze: 2px Grat #ccffff; Auffüllen: 15px; Textausrichtung: Mitte; Animationsname: RainbowGlow; Animationsdauer: 1.5s; Animations-Iterationszählung: 1; }
```

Wenn Sie **Prozentwerte** statt `von` und `bis`, können Sie Zwischenwerte sowie Werte für Anfang und Ende festlegen. Sie können so viele Zwischenwerte einstellen, wie Sie möchten, indem Sie verschiedene Prozentwerte von `0` bis `100`.

+ Ändern Sie den Wert von `animation-iteration-count` in `infinite`. Sehen Sie, ob Sie erraten können, was passieren wird, bevor Sie es testen!

+ Probieren Sie verschiedene Werte für `Animationsdauer` , um Ihre Animation zu beschleunigen oder zu verlangsamen.

+ Ein letzter Trick! Fügen Sie diesen Animationscode hinzu:

```css
    @keyframes slide {0% {Hintergrundposition-x: 0; } 100% {Hintergrundposition-x: 600vw; }}
```

+ Finde nun die `# frontPage` CSS-Regeln, die du zuvor geschrieben hast, und ändere sie in:

```css
    #frontPage {Hintergrund: wiederholender linearer Gradient (-45 Grad, Rot 0%, Gelb 7,14%, Kalk 14,28%, Cyan 21,42%, Cyan 28,56%, Blau 35,7%, Magenta 42,84%, Rot 50%); Hintergrundgröße: 600vw 600vw; Animation: Folie 10s unendlich linear vorwärts; }
```

Mach dir keine Sorgen darüber, den gesamten obigen Code zu verstehen ... lehn dich einfach zurück und genieße !!

Um mehr über Dinge zu erfahren, die Sie mit Animation machen können, besuchen Sie [diese Webseite](http://dojo.soy/html2-css-animation){: target = "_ blank"}. Habe Spaß!

Auf der nächsten Karte lernst du, wie man coole Sachen macht, wenn man den Mauszeiger über Dinge bewegt!