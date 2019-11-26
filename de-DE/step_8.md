## Passe die Größe automatisch an

Bisher hast Du **Pixel** verwendet, um die Größe von Objekten festzulegen, z.B. `10px`. Auf dieser Karte wirst Du mehr über andere Maßeinheiten erfahren, die Du verwenden kannst.

+ Gehe zu `index.html` und finde das `img` Element mit dem Bild von Tito oder ein anderes `img` Tag auf deiner Website.

+ Lösche das `width` Attribut falls es vorhanden ist, und gib dem Element eine `ID`, falls es noch keine hat.

```html
  <img src="tito.png" id="titoPicture" alt="Tito der Hund" />
```

+ In Deiner CSS-Datei definiere die `width` Eigenschaft für Dein Bild wie unten gezeigt (Du musst den CSS Block mit dem `ID` Selektor möglicherweise erstellen, falls Du das noch nicht auf einer früheren Karte getan hast).

```css
  #titoPicture {
    width: 50%;
    border-radius: 100%;
  }
```

Hinweis: 50% (50 Prozent) ist die **Hälfte**.

+ Verändere die Größe deines Browser-Fensters und schau, was mit dem Bild passiert.

Du solltest sehen, dass das Bild größer und kleiner wird, wenn Du das Fenster größer und kleiner machst. Das liegt daran, dass es 50% der Breite des **main** Elements einnimmt (was ungefähr der Breite der Seite entspricht).

## \--- collapse \---

## title: Wie funktioniert das?

Wenn Du die Größe eines Objekts in Pixel festlegst, legst Du eine genaue Größe fest, die sich nicht ändert. Das wird als **absolute** Abmessung bezeichnet.

Eine andere Möglichkeit, die Größe von Dingen festzulegen, ist die Verwendung von **relativen** Messungen, sodass die Größe davon abhängt, wie groß Elemente im Vergleich zueinander sind. Wenn dann eine Sache die Größe ändert, wird alles andere automatisch die Größe ändern, um die gleichen **Proportionen** zu behalten.

Wenn Du **relative** Messungen verwendest, ist es wichtig zu wissen, was das **"Elter"** Deines Elements ist. Das "Elter" (Einzahl von Eltern) ist das Objekt, in dem sich Dein Element befindet und das wird das sein auf das sich die Abmessungen beziehen. Zum Beispiel ist das Elter des obigen Bildes das `article` Element, da das `img` Element zwischen den `<article></article>` Tags liegt.

Wenn Du die Breite (also `width`) eines Elements auf `100%` setzt, wird es die gleiche Breite haben, wie der übergeordnete Container.

\--- /collapse \---

+ Experimentiere mit verschiedenen Zahlen vor `%`.