## Alle Farben!

Wie Du bereits gesehen hast, kannst Du viele verschiedene Farbnamen als Wörter eingeben und der Browser erkennt diese. Aber eine geläufigere Methode Farben festzulegen ist sogenannte **Hex-Codes** zu verwenden ("Hex" ist eine Abkürzung für **Hexadezimal**, das ist eine besondere Art zu zählen).

+ Schau Dir Dein **Style Sheet** an. Das ist die Datei, die `.css` im Namen hat.

+ Setze die Hintergrundfarbe (engl.: backgroundcolor), innerhalb der CSS-Regel für `body`, auf den Hex-Code `#7B68EE`:

```html
  background-color: #7B68EE;
```

Hinweis: Falls Du einen Mac verwendest, kannst Du `#` durch gleichzeitiges Drücken der <kbd>Alt</kbd> und der <kbd>3</kbd> Taste eingeben.

Deine Website sollte jetzt einen lila Hintergrund haben.

![](images/HexColourFirst.png) ![](images/HexColourFirstResult.png)

+ Kein Fan von Lila? Gehe auf [diese Webseite](http://dojo.soy/html2-colors){:target="_blank"} und wähle eine andere Farbe für Dein Stylesheet aus. Anstatt den Namen der Farbe einzugeben, gib den Hex-Code ein. 

![](images/ColorNamesHex.png)

Farbcodes erlauben es Dir jede Farbe zu erzeugen, auch wenn sie auf keiner Liste von Farbnamen steht.

+ Versuch Deinen eigenen Farbcode zu erstellen. Er muss mit einer `#` beginnen. Das sagt dem Browser, dass es sich um einen Hex-Code, statt eines Farbnammen, handelt. Der Rest des Codes besteht aus sechs Zeichen. Das kann eine beliebige Zahl von **0 bis 9** und ein beliebiger Buchstabe von **A bis F** sein.

## \--- collapse \---

## title: Wie funktioniert das?

Jede Farbe wird durch Mischen verschiedener Mengen von **Rot**, **Grün** und **Blau** erzeugt. Manchmal wird das als **RGB** geschrieben. Jede dieser Farben wird durch zwei der sechs Ziffern in Deinem HEX-Code dargestellt. `00` ist das Minimum und `FF` ist das Maximum.

**Hexadezimal** ist eine Methode zum Zählen, mit der Zahlen kürzer geschrieben werden können, indem die Buchstaben A-F als zusätzliche Ziffern verwendet werden. Die Zahl `255` wird hexadezimal als `FF` geschrieben. Du musst dir keine Gedanken darüber machen, zu lernen wie man mit hexadezimalen Zahlen zählt. Experimentiere stattdessen mit verschiedenen Hex-Codes, um dich daran zu gewöhnen, wie man sie benutzt.

+ Hier sind einige Grundfarben, die Du auf Deiner Website ausprobieren kannst. Versuche kleinere Zahlen anstelle von `FF` einzufügen, um zu sehen, wie sich die Schattierungen ändern.

|      | R  | G  | B  |    Ergebnis    |
| ---- | -- | -- | -- |:--------------:|
| \# | FF | 00 | 00 |      Rot       |
| \# | 00 | FF | 00 |      Grün      |
| \# | 00 | 00 | FF |      Blau      |
| \# | FF | FF | 00 |      Gelb      |
| \# | FF | 00 | FF |    Magenta     |
| \# | 00 | FF | FF |     Türkis     |
| \# | FF | 8c | 00 | Dunkles Orange |

\--- /collapse \---

Das Mischen der perfekten Farbe kann viel Experimentieren erfordern. Glücklicherweise gibt es viele Online-Farbauswahlwerkzeuge, die Dir helfen, den Hex-Code für jede gewünschte Farbe zu bekommen.

![](images/W3ColorPicker.png)

+ Probiere [diesen Farbwähler](http://dojo.soy/html2-color-picker){:target="_blank"} aus, um einige hexadezimale Farbcodes für den Rest der Stile auf Deiner Website auszuwählen.