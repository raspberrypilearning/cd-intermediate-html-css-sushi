## Passen Sie die Größe automatisch an

Bis jetzt haben Sie **Pixel** , um die Größe der Dinge festzulegen, zB `10px`. Auf dieser Karte erfahren Sie mehr über andere Messungen, die Sie verwenden können.

+ Gehe zu `index.html` und finde das `img` Element mit dem Bild von Tito, oder finde ein anderes `img` Tag auf deiner Webseite.

+ Löschen Sie das `width` Attribut, wenn es dort ist, und geben Sie dem Element eine `ID` wenn es nicht bereits eins hat.

```html
  <img src="tito.png" id="titoPicture" alt="Tito the dog" />
```

+ Definieren Sie in Ihrer CSS-Datei die Eigenschaft `width` für Ihr Bild, wie unten gezeigt (Sie müssen möglicherweise den CSS-Block mit dem Selektor `id` erstellen, falls Sie dies auf einer früheren Karte noch nicht getan haben).

```css
  #titoPicture {Breite: 50%; Rand-Radius: 100%; }
```

Hinweis: 50% (50 Prozent) ist **halb**.

+ Versuchen Sie, die Größe Ihres Browserfensters zu ändern und beobachten Sie, was mit dem Bild passiert.

Sie sollten sehen, dass das Bild größer und kleiner wird, wenn Sie das Fenster größer und kleiner machen. Dies liegt daran, dass es 50% der Breite des **Hauptelements** einnimmt (was ungefähr der Breite der Seite entspricht).

## \--- Einsturz \---

## Titel: Wie funktioniert es?

Wenn Sie die Größe eines Objekts in Pixeln festlegen, legen Sie eine genaue Größe fest, die sich nicht ändert. Dies wird als **absolute** Messung bezeichnet.

Eine weitere Möglichkeit, die Größe der Dinge festzulegen, ist die Verwendung von **relativen** Messungen, so dass die Größe davon abhängt, wie große Elemente miteinander verglichen werden. Immer dann, wenn eine Sache Größe ändert, alles andere wird automatisch Größe auch ändern , um die gleichen zu halten **Proportionen**.

Wenn Sie **relative** Messungen verwenden, ist es wichtig zu wissen, was die **Eltern** Ihres Elements sind. Der Elternteil ist die Sache, in der sich dein Element befindet, und darum geht es in Bezug auf die Messung. Zum Beispiel ist das übergeordnete Element des obigen Bildes das `Element von Artikel` , weil das Element `img` zwischen den Tags `<article></article>`.

Wenn Sie die `width` eines Elements auf `100%`, entspricht dies der Breite des übergeordneten Containers.

\--- / einklappen \---

+ Experimentiere mit verschiedenen Zahlen vor dem `%`.