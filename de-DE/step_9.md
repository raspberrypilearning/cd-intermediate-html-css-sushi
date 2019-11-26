## Animationen

Wusstest du, dass du CSS verwenden kannst, um Dinge zu bewegen? Auf dieser Karte lernst du wie!

+ Bevor Du loslegst, stelle sicher, dass Du ein Bild auf Deiner Webseite, mit einer `ID` und einen entsprechenden CSS Block, hast, der die `Breite` auf `100px` setzt. Ich nehme das Bild von Tito von zuvor, und mein CSS-Block sieht so aus:

```css
    #titoPicture {
        border-radius: 100%;
        width: 100px;
    }
```

+ Gehe zum Ende deiner CSS-Datei und füge folgenden Code hinzu:

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

Dieser Code erstellt eine Animation mit dem Namen `myFirstAnimation`, die Du zu jedem Element auf Deiner Website hinzufügen kannst. Was glaubst du, wird es tun?

+ Suche Deine CSS-Regeln für das Bild und füge die folgenden drei Eigenschaften hinzu:

```css
    animation-name: myFirstAnimation;
    animation-duration: 2s;
    animation-iteration-count: 1;
```

+ Schau Dir an, was auf Deiner Webseite passiert! Probiere verschiedene Werte für `animation-iteration-count` (engl.: Anzahl der Animationsiterationen) aus, um zu sehen, was es tut.

+ Lass uns eine weitere Animation versuchen! Füge den folgenden Code am Ende deiner CSS-Datei hinzu:

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

+ Such jetzt die `#myCoolText` CSS-Regeln von vorhin und füge den Animationscode hinzu:

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

Wenn Du **Prozentwerte** anstelle von `from` (engl:: von) und `to` (engl.: bis) verwendest, kannst Du sowohl Zwischenwerte als auch Start- und Endwerte festlegen. Du kannst so viele Zwischenwerte, mit verschiedenen Prozentwerten von `0` bis `100`, wie Du möchtest einstellen.

+ Ändere den Wert von `animation-iteration-count` zu `infinite` (engl.: unendlich). Überlege dir, was wohl passieren wird, bevor Du es ausprobierst!

+ Probiere verschiedene Werte für `animation-duration` (engl.: Animationsdauer) aus, um Deine Animation zu beschleunigen oder zu verlangsamen.

+ Ein letzter Trick! Füge diesen Animationscode hinzu:

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

+ Suche jetzt die `#frontPage` CSS-Regeln, die du zuvor geschrieben hast und ändere sie zu:

```css
    #frontPage {
        background: repeating-linear-gradient(-45deg, red 0%, yellow 7.14%, lime 14.28%, cyan 21.42%, cyan 28.56%, blue 35.7%, magenta 42.84%, red 50%);
        background-size: 600vw 600vw;
        animation: slide 10s infinite linear forwards;
    }
```

Mach dir keine Sorgen, den gesamten obigen Code zu verstehen... lehn dich einfach zurück und genieße es!!

Um mehr über Dinge zu erfahren, die Du mit Animationen tun kannst, besuche [diese Webseite](http://dojo.soy/html2-css-animation){:target="_blank"}. Habe Spaß!

Auf der nächsten Karte wirst du lernen, wie du coole Dinge passieren lassen kannst, wenn du den Mauszeiger über Dinge bewegst!