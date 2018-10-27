## Entwerfen Sie einige Themen

Schreiben von CSS-Regeln für Elemente wie `Abschnitt` und `p` ist großartig, aber was ist, wenn Sie möchten, dass einige von ihnen anders aussehen als andere? Auf dieser Karte erfahren Sie, wie Sie verschiedene Arten von Stilregeln auf Elemente desselben Typs anwenden und für jede Seite Ihrer Website ein anderes Thema erstellen können!

+ Gehen Sie zu Ihrer Stylesheet-Datei und fügen Sie Folgendes hinzu: Achten Sie darauf, dass der Punkt davor steht!

```css
  .topDivider {border-top-style: fest; border-top-width: 2px; border-top-color: # F5FFFA; padding-bottom: 10px; }
```

+ Gehen Sie jetzt zu `attractions.html` (oder der HTML-Datei, an der Sie gerade arbeiten, wenn Sie Ihr eigenes Projekt verwenden) und fügen Sie jedem `Section-` Tag die folgenden **Attribute**:

```html
  <section class="topDivider">
```

Über jedem Abschnitt auf der Seite sollte eine Linie angezeigt werden. Herzlichen Glückwunsch - Sie haben gerade Ihr erstes verwendet **CSS - Klasse**!

![Seite mit Linien zwischen den Abschnitten](images/sectionsWithTopBorder.png)

+ Schau dir an, wie deine Webseite jetzt aussieht und vergleiche sie mit den anderen Seiten, die `Sektion` Elemente haben. Sie werden sehen, dass nur diejenigen, bei denen Sie das Attribut `class = "topDivider"` hinzugefügt haben, die Zeile oben haben.

## \--- Einsturz \---

## Titel: Wie funktioniert es?

Denken Sie daran , dass , wenn Sie einen CSS **Selektor** wie `Abschnitt` oder `p` oder `nav ul`gelten die Stilregeln zu **alle** die Elemente dieses Typs auf Ihrer Webseite ein .

Mit CSS **classes**können Sie den Stil von nur **** Elementen ändern.

Wenn Sie einen Punkt vor Ihren Selektor setzen, wird dieser zu einem **Klassen-Selektor**. Eine Klasse kann einen beliebigen Namen haben, also muss sie nicht der Name eines HTML-Elements sein. Beispielsweise:

```css
  .myAwesomeClass {/ * Meine coolen Style-Regeln gehen hier * /}
```

Um auszuwählen, auf welche Elemente die Stilregeln angewendet werden, fügen Sie das `Klasse` **-Attribut** zu diesen Elementen im HTML-Code hinzu: Setzen Sie den Namen der Klasse als Wert für das Attribut ein, **ohne** den Punkt, so:

```html
  class = "meineAwesomeClass"
```

\--- / einklappen \---

+ Bereit, eine andere Klasse auszuprobieren? Fügen Sie den folgenden CSS-Code zu `styles.css`:

```css
  .stylishBox {Hintergrundfarbe: # 87CEFA; Farbe: # A52A2A; Rand-Stil: fest; Rahmenbreite: 2px; Rahmenfarbe: # F5FFFA; Rand-Radius: 10px; }
```

+ Fügen Sie dann auf einer anderen Seite Ihrer Website die Klasse einigen Elementen hinzu. Ich füge es zu den `Section` Elementen auf der Food Seite meiner Website hinzu, so: `<section class="stylishBox">`.

Es sieht gut aus, aber jetzt sind meine Abschnitte alle zusammen gequetscht.

![Schön aussehende Abschnitte zusammengequetscht](images/squashedSections.png)

Sie können so viele CSS-Klassen auf ein Element anwenden, wie Sie möchten. Schreiben Sie einfach die Namen aller Klassen, die Sie verwenden möchten, in das `Klasse-` Attribut (denken Sie daran, ohne den Punkt!) Und trennen Sie sie durch Leerzeichen.

+ Lassen Sie uns eine weitere CSS-Klasse erstellen, um den Abschnitten einen gewissen Spielraum zu geben. Erstellen Sie in der Datei `styles.css` die folgende CSS-Klasse:

```css
  .someSpacing {Auffüllen: 10px; Rand oben: 20px; }
```

+ Fügen Sie in Ihrem `html` Code die neue Klasse zu jedem der Elemente hinzu, an denen Sie gerade gearbeitet haben:

```html
  <section class="stylishBox someSpacing">
```

![Abschnitte mit Rand und Abstand hinzugefügt](images/sectionsWithSpacing.png)

So CSS - Klassen können Sie **wählen** , welche Elemente zu Stil, und sie lassen Sie **Wiederverwendung** der gleiche Satz von Stilregeln auf alle Elemente , die Sie wollen.

+ Gehe zu `index.html` und füge die `stylishBox` Klasse den `wichtigsten` Elementen oder einem anderen Element auf der Seite hinzu. Sie können es danach wieder entfernen!

```html
    <main class="stylishBox">   
```

So sieht meine Homepage mit der CSS-Klasse aus. Ich habe auch die Klasse `topDivider` zum Tag `img` mit dem Bild von Tito hinzugefügt.

![CSS-Klassen werden auf der Startseite verwendet](images/homePageWithClasses.png)

\--- Herausforderung \---

## Herausforderung: Mach ein paar neue Klassen

+ Verwenden Sie CSS **classes** , um einige verschiedene Bildgrößen für Ihre Website zu definieren, z. B. `.smallPictures` und `.mediumPictures`. Entfernen Sie dann das Attribut `width` von jedem Ihrer `Elemente img` und fügen Sie stattdessen die entsprechende Klasse hinzu.

\--- Hinweise \---

\--- Hinweis \---

Sie können eine CSS-Klasse erstellen, die nur die Breite eines Elements definiert:

```css
  .smallPictures {Breite: 100px; }
```

\--- /Hinweis \---

\--- Hinweis \---

Hier ist ein `img` -Tag mit einem `width` -Attribut:

```html
  <img src="tito.png" alt="Tito the dog" width="100px" />       
```

Wenn Sie das Attribut `width` entfernen und stattdessen die Größe mit der CSS-Klasse steuern, sieht es folgendermaßen aus:

```html
  <img src="tito.png" class="smallPictures" alt="Tito the dog" />       
```

Wenn Sie eine CSS-Klasse verwenden, können Sie die Breite aller Bilder auf einmal ändern, indem Sie nur eine Zeile Code in Ihrem Stylesheet ändern.

\--- /Hinweis \---

\--- / Hinweise \---

\--- /Herausforderung \---