## Organisiere Deine Seite

Bisher hast Du **Überschriften** und **Absätze** verwendet, damit Deine **Inhalte** übersichtlich aussehen und leicht lesbar sind. Lass sie uns noch übersichtlicher gestalten, indem wir Dinge zu Gruppen zusammenfassen.

## \--- collapse \---

## title: Was ist Inhalt?

**Inhalt** ist all das Zeug auf Deiner Webseite, wie Texte und Bilder.

\--- /collapse \---

+ Wechsle zur Datei `attractions.html` (oder zu einer Deiner eigenen Seiten, falls Du das Beispielprojekt nicht verwendest), und gib oben, direkt **unter** dem öffnenden `<main>` Tag, Folgendes in eine neue Zeile ein: 

```html
  <main>
    <article>
```

+ Falls Dein Editor automatisch ein schließendes `</article>` Tag für dich eingefügt hat, lösch es wieder.

+ Am Ende der Datei, direkt **über** dem schließenden `</main>` Tag, fügst Du eine neue Zeile hinzu und schließt das `article` Element:

```html
    </article>
  </main>
```

Dein `main` Element sollte jetzt ungefähr so aussehen (natürlich kann es sein, dass du andere Inhalte zwischen den `article` Tags hast):

```html
  <main>
    <article>
      <h1>Meine Lieblingsorte in Irland</h1>
        <h2>Die Klippen von Moher</h2>
        <p>
        Die Klippen von Moher befinden sich in der Grafschaft Clare, wo ich herkomme. Schau wie cool sie sind!</p>
        <img src="cliffs.JPG" alt="Die Klippen von Moher" height="200px" />
        <h2>Achill Insel</h2>
        <p>Das ist eine große Insel vor der Küste der Grafschaft Mayo. Sie hat eine wilde und
        wunderschöne Landschaft mit Bergen, Mooren und Klippen.
        </p>
        <img src="achill.JPG" width="200px" />
    </article>
  </main>
```

+ Schau Dir jetzt den Inhalt in deinem Artikel (engl.: `article`) an und versuch ihn in Abschnitte aufzuteilen. Setze dieses neue Tag-Paar um jeden Teil: `<section></section>` (section ist englisch für Sektion/Abschnitt). Hier ist ein Beispiel, wie das aussehen könnte:

```html
  <article>
    <h1>Meine Lieblingsorte in Irland</h1>
    <section>
      <h2>Die Klippen von Moher</h2>
      <p>
      Die Klippen von Moher befinden sich in der Grafschaft Clare, wo ich herkomme. Schau wie cool sie sind!</p>
      <img src="cliffs.JPG" alt="Die Klippen von Moher" height="200px" />
    </section>
    <section>
      <h2>Achill Insel</h2>
      <p>Das ist eine große Insel vor der Küste der Grafschaft Mayo. Sie hat eine
        wunderschöne und wilde Landschaft mit Bergen, Mooren und Klippen.
      </p>
      <img src="achill.JPG" width="200px" />
    </section>
  </article>
```

## \--- collapse \---

## title: Worum geht es bei den neuen Tags?

Stelle Dir diese neuen Elemente als **Container** (engl.: Behälter) vor. Sie werden verwendet, um Dinge zu gruppieren. Es ist ein bisschen so, als würde man Dinge in Kisten und Regalen bei sich zu Hause organisieren!

Das macht Deine Website benutzerfreundlich für Screenreader (das sind Programme die den Bildschirminhalt vorlesen), gibt Dir mehr Kontrolle über das Layout und ermöglicht es Dir, wie Du noch sehen wirst, wirklich kreativ mit der Gestaltung zu werden.

Zwischen den Tags kann alles stehen. Normalerweise sind es mehr als ein Element, aber das muss nicht sein. Es können beliebige HTML-Elemente sein. Was Du machst ist, dem Browser mitzuteilen, dass alles zwischen diesen Tags zusammengehört.

### Artikel

Das `article` (engl.: Artikel) Element ist ein Container für ein ganzes Stück Inhalt, in diesem Fall eine Reihe von Informationen über Sehenswürdigkeiten in Irland. Wenn Du verschiedene Arten von Inhalten hast, die nicht zueinander gehören, solltest Du jeden in sein eigenes `article` Element stecken, anstatt nur einen Satz von Tags um das Ganze zu legen.

### Section

Das `section` (engl.: Sektion/Abschnitt) Element lässt dich verwandte Inhalte in kleinere Blöcke aufteilen und jeden Block in seinen eigenen Container packen.

### Es gibt auch Andere!

Das sind nicht die einzigen Containerelemente in HTML. Hast Du schon mal ein Menü erstellt hast und das dann zwischen `<nav></nav>` Tags gesetzt, das ist ein weiteres Beispiel für einen Containertyp. Ebenso wie `<main></main>` und `<header></header>`. Fallen Dir noch mehr ein?

\--- /collapse \---

\--- challenge \---

Deine Webseite sieht vielleicht noch nicht anders aus, aber sobald der Inhalt in Container-Tags organisiert wurde, kannst Du mit CSS einige coole Dinge tun. Erinnere Dich, HTML steuert wie deine Website organisiert ist und CSS steuert wie sie aussieht.

## Herausforderung: Organisiere Deine Website

+ Versuche den gesamten Inhalt Deiner Website mithilfe von `article`- und `section`-Containern zu organisieren. 

\--- hints \---

\--- hint \---

Schau Dir die "Essen" Seite aus dem Beispielprojekt an. Du wirst sehen, dass ich einen `article` mit einigen `section` Tags in die Datei `food.html` eingefügt habe:

```html
  <main>
    <article>
      <h1>Essen in Irland</h1>
      <p>
        Dies sind einige meiner Lieblingsspeisen aus Irland!
      </p>  
      <section>
        <h2>Traditionelles irisches Frühstück</h2>
        <p>
         Ein "richtiges irisches" Frühstück besteht aus Würstchen, Speck,
          Eiern, Blutwurst, Weißwurst und Toast.
        </p>
        <p>
          Oft gibt es eine gegrillte Tomate sowie Pilze,
    	  und gebackene Bohnen.
        </p>
        <p>
          Und natürlich ist es kein Frühstück ohne eine schöne Kanne
          Tee!
        </p>
      </section>

      <section>
        <h2>Würstchen und Pürree</h2>
        <p>
          Diesen Klassiker aus Würstchen, Kartoffelpürre und Soße gibt es zwar nicht 
          nur in Irland aber was es besonders macht sind die irischen 
          Würstchen. Die meisten Länder haben ihre eigene Art Würstchen zu machen,
          und sie sind eine Sache, die ich von zu Hause vermisse, wenn ich unterwegs bin!
        </p>
      </section>

      <section>
        <h2>Speck und Kohl</h2>
        <p>
          Ich könnte keine Liste irischer Speisen erstellen, ohne
  	  dieses sehr traditionelle Gericht einzubeziehen!
        </p>
        <p>
         Es mag nicht sehr interessant klingen, aber diese herzhafte Mahlzeit aus
  	gekochtem Schinken, Kartoffeln und Grünkohl ist lecker und sättigend.
          Ich liebe es, die Kartoffeln in Butter zu ersticken, und ein
        wenig Senf mit dem Speck darf nicht fehlen.
        </p>
        <p>
          Meine Mutter hatte ihre eigene Art den Grünkohl 
          in dem Wasser vom Schinken zu kochen.
        </p>
        <p>
          Sollte es Reste geben, kannst du noch eines meiner Lieblingsgerichte 
          kochen: <strong>frittierten Kohl</strong>!
        </p>
      </section>
    </article>     
  </main>
```

\---/hint\---

\---/hints \---

Auf der nächsten Karte wirst Du für jede Seite, die in Artikel und Sektionen organisiert ist, ein anderes Design erstellen!

\--- /challenge \---