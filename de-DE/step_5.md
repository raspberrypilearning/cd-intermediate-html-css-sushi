## Organisieren Sie Ihre Seite

Bisher haben Sie **Überschriften** und **Absätze** , um Ihre **Inhalte** ordentlich und leicht lesbar zu machen. Machen wir es noch organisierter, indem wir Dinge zusammenfassen.

## \--- Einsturz \---

## Titel: Was ist Inhalt?

**Inhalt** alle Inhalte auf Ihrer Webseite, z. B. Text und Bilder.

\--- / einklappen \---

+ Gehen Sie zur Datei `attractions.html` (oder zu einer Ihrer eigenen Seiten, wenn Sie das Beispielprojekt nicht verwenden) und geben Sie in der oberen Zeile nur **unter** das öffnende `<main>` -Tag ein und geben Sie Folgendes in eine neue Zeile ein : 

```html
  <main>
    <article>
```

+ Wenn Ihr Editor automatisch ein abschließendes `</article>` -Tag für Sie hinzugefügt hat, löschen Sie es.

+ Fügen Sie am Ende der Datei, nur **über** dem schließenden `</main>` -Tag, eine neue Zeile hinzu und schließen Sie das Element `artikel`:

```html
    </article>
  </main>
```

Ihr `main` Element sollte jetzt ungefähr so ​​aussehen (Sie könnten zwischen den `Tags des Artikels` natürlich unterschiedliche Inhalte haben):

```html
  <main>
    <article>
      <h1>Meine Lieblingsorte in Irland</h1>
        <h2>Die Klippen von Moher</h2>
        <p>
        Die Klippen von Moher sind in der Grafschaft Clare, wo ich bin. Schau, wie cool sie sind!</p>
        <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
        <h2>Achill Island</h2>
        <p>Dies ist eine große Insel vor der Küste der Grafschaft Mayo. Es hat eine wilde und schöne Landschaft mit Bergen, Mooren und Klippen.
        </p>
        <img src="achill.JPG" width="200px" />
    </article>
  </main>
```

+ Schauen Sie sich nun den Inhalt in Ihrem `Artikel` und versuchen Sie ihn in Abschnitte aufzuteilen. Legen Sie dieses neue Paar Tags um jedes Bit: `<section> </section>`. Hier ist ein Beispiel dafür, wie es aussehen könnte:

```html
  <article>
    <h1>Meine Lieblingsorte in Irland zu sehen</h1>
    <section>
      <h2>Die Klippen von Moher</h2>
      <p>
      Die Klippen von Moher sind in der Grafschaft Clare, wo ich bin. Schau, wie cool sie sind!</p>
      <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
    </section>
    <section>
      <h2>Achill Island</h2>
      <p>Dies ist eine große Insel vor der Küste der Grafschaft Mayo. Es hat eine wilde und schöne Landschaft mit Bergen, Mooren und Klippen.
      </p>
      <img src="achill.JPG" width="200px" />
    </section>
  </article>
```

## \--- Einsturz \---

## Titel: Worum geht es bei den neuen Tags?

Stellen Sie sich diese neuen Elemente als **Container**. Sie werden verwendet, um Dinge zusammen zu gruppieren. Es ist ein bisschen so, als würde man Dinge in Kisten und Regalen in deinem Haus organisieren!

Dies macht Ihre Website für Bildschirmleser freundlich, gibt Ihnen mehr Kontrolle über das Layout und, wie Sie sehen werden, ermöglicht es Ihnen, wirklich kreativ mit dem Styling zu werden.

Alles kann zwischen den Tags eingefügt werden. Normalerweise wird es mehr als ein Element sein, aber es muss nicht sein. Es können HTML-Elemente jeglicher Art sein. Sie sagen dem Browser, dass alles zwischen diesen Tags zusammen gehört.

### Artikel

Das Element `Artikel` ist ein Container für ein ganzes Stück Inhalt, in diesem Fall eine Reihe von Informationen über Attraktionen in Irland. Wenn Sie verschiedene Teile des Inhalts haben, die nicht verwandt sind, sollten Sie jedes in sein eigenes `Artikel` Element setzen, anstatt einen Satz der Tags um das ganze Los zu legen.

### Sektion

Mit dem Element `section` können Sie verwandte Inhalte in kleinere Abschnitte aufteilen und jeden Abschnitt in einen eigenen Container einfügen.

### Andere existieren auch!

Dies sind nicht die einzigen Containerelemente in HTML. Wenn Sie jemals ein Menü erstellt und es dann zwischen `<nav> </nav>` Tags eingefügt haben, ist dies ein weiteres Beispiel für einen Containertyp. So sind `<main> </main>` und `<header> </header>` - können Sie noch mehr denken?

\--- / einklappen \---

\--- Herausforderung \---

Ihre Webseite sieht vielleicht noch nicht anders aus, aber sobald der Inhalt in Containertags organisiert ist, können Sie mit CSS einige coole Dinge tun. Denken Sie daran, dass HTML steuert, wie Ihre Website organisiert ist, und CSS steuert, wie es aussieht.

## Herausforderung: Organisieren Sie Ihre Website

+ Organisieren Sie auf diese Weise alle Inhalte auf Ihrer Website mit den Containern `Artikel` und `Abschnitt`. 

\--- Hinweise \---

\--- Hinweis \---

Sehen Sie sich die Seite "Essen" des Beispielprojekts an. Sie werden sehen, dass ich einen `Artikel` mit einer Reihe von `Abschnitt` Tags in die Datei `food.html`hinzugefügt habe:

```html
  <main>
    <article>
      <h1>Essen in Irland</h1>
      <p>
        Dies sind einige meiner Lieblingsspeisen in Irland!
      </p>  
      <section>
        <h2>Traditionelles irisches Frühstück</h2>
        <p>
          Ein "komplettes irisches" Frühstück besteht aus Würstchen, Speckscheiben, Eiern, Blutwurst, Blutwurst und Toast.
        </p>
        <p>
          Oft gibt es eine gegrillte Tomate sowie Pilze und gebackene Bohnen.
        </p>
        <p>
          Und natürlich ist kein Frühstück ohne eine schöne Kanne Tee komplett!
        </p>
      </section>

      <section>
        <h2>Bangers and Mash</h2>
        <p>
          Dieser Klassiker aus Würstchen, Kartoffelpüree und Soße ist nicht nur in Irland zu finden. Die meisten Länder haben ihre eigene Art, Würste zu machen, und sie sind eine Sache, die ich von zuhause vermisse, wenn ich auf Reisen bin!
        </p>
      </section>

      <section>
        <h2>Bacon and Cabbage</h2>
        <p>
          Ich könnte unmöglich eine Liste von irischem Essen machen, ohne dieses sehr traditionelle Gericht einzubeziehen!
        </p>
        <p>
          Es klingt vielleicht nicht sehr interessant, aber diese herzhafte Mahlzeit aus gekochtem Schinken, Kartoffeln und Grünkohl ist lecker und sättigend.
          Ich liebe es, die Kartoffeln in Butter zu ersticken, und ich mag auch ein wenig Senf mit dem Speck.
        </p>
        <p>
          Meine Mutter machte es immer besonders, indem sie den Kohl im Wasser kochte, in dem der Schinken gekocht wurde.
        </p>
        <p>
          Wenn es irgendwelche Reste gibt, kannst du noch einen meiner Favoriten machen: <strong>gebratener Kohl</strong>!
        </p>
      </section>
    </article>     
  </main>
```

\--- /Hinweis \---

\--- / Hinweise \---

Auf der nächsten Karte entwerfen Sie ein anderes Thema für jede Seite, die in Artikeln und Abschnitten organisiert ist!

\--- /Herausforderung \---