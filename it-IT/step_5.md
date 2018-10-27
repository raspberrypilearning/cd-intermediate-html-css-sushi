## Organizzare la tua pagina

Finora hai usato **titoli (headings)** e **paragrafi (paragraphs)** per rendere il tuo **contenuto** ordinato e facile da leggere. Rendiamolo ancora più organizzato raggruppando le cose.

## \--- collapse \---

## title: Cosa è il contenuto?

**Contenuto** è tutto ciò che c'è nella tua pagina web, come testo e immagini.

\--- /collapse \---

+ Vai al file `attractions.html` (o una delle tue pagine, se non stai usando il progetto di esempio) e, nella parte superiore, appena **sotto** il tag `<main>` di apertura, digita quanto segue in una nuova riga: 

```html
  <main>
    <article>
```

+ Se il tuo editor ha aggiunto automaticamente un tag di chiusura `</article>`, eliminalo.

+ Nella parte inferiore del file, subito **sopra** al tag di chiusura `</main>`, aggiungi una nuova riga e chiudi l'elemento `article`:

```html
    </article>
</main>
```

Il tuo elemento `main (principale)` dovrebbe apparire ora simile a questo (ovviamente potrai avere contenuti diversi tra i tag `article`):

```html
  <main>
    <article>
      <h1>I miei posti preferiti da vedere in Irlanda</h1>
        <h2>The Cliffs of Moher</h2>
        <p>
        Le Scogliere, o Cliffs of Moher si trovano nella Contea di Clare, da dove vengo. Guarda che spettacolo!</p>
        <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
        <h2>Achill Island</h2>
        <p>È una grande isola al largo della contea di Mayo. Ha un bellissimo paesaggio selvaggio di montagne, torbiere e scogliere.
        </p>
        <img src="achill.JPG" width="200px" />
    </article>
  </main>
```

+ Ora guarda il contenuto del tuo `article` e prova a suddividerlo in sezioni. Metti questa nuova coppia di tag attorno ad ogni contenuto: `<section> </section>`. Ecco un esempio di come potrebbe apparire:

```html
  <article>
    <h1>I miei posti preferiti da vedere in Irlanda</h1>
    <section>
      <h2>The Cliffs of Moher</h2>
      <p>
      Le Scogliere, o Cliffs of Moher si trovano nella Contea di Clare, da dove vengo. Guarda che spettacolo!</p>
      <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
    </section>
    <section>
      <h2>Achill Island</h2>
      <p>È una grande isola al largo della contea di Mayo. Ha un bellissimo paesaggio selvaggio di montagne, torbiere e scogliere.
      </p>
      <img src="achill.JPG" width="200px" />
    </section>
  </article>
```

## \--- collapse \---

## title: A cosa servono i nuovi tag?

Pensa a questi nuovi elementi come **contenitori**. Sono usati per raggruppare le cose. È un po' come organizzare le cose in scatole e scaffali nella tua casa!

Questo rende il tuo sito web adatto ai lettori dello schermo, ti dà un maggiore controllo sul layout e, come vedrai, ti permette di diventare davvero creativo con lo stile.

Qualsiasi cosa può andare tra i tag. Di solito sarà più di un elemento, ma non deve esserlo necessariamente. Può essere qualsiasi tipo di elemento HTML. Quello che stai facendo è dire al browser che tutto ciò che sta tra questi tag sta bene insieme.

### Article

L'elemento `article` è un contenitore per un intero contenuto, in questo caso un insieme di informazioni sulle attrazioni in Irlanda. Se hai diversi blocchi di contenuto che non sono correlati, dovresti inserire ognuno nel proprio elemento `article` invece di mettere un set di tag attorno all'intera area.

### Section

L'elemento `section` ti consente di suddividere il contenuto correlato in blocchi più piccoli e di inserire ciascun blocco nel proprio contenitore.

### Ne esistono anche altri!

Questi non sono gli unici elementi contenitore in HTML. Se hai mai creato un menu e poi lo hai inserito tra i tag `<nav> </nav>`, questo è un altro esempio di un tipo di contenitore. Lo sono anche `<main> </main>` e `<header> </header>` - te ne vengono in mente altri?

\--- /collapse \---

\--- challenge \---

La tua pagina web potrebbe non sembrare ancora diversa, ma una volta che il contenuto è stato organizzato in tag contenitore, sarai in grado di fare alcune cose interessanti con i CSS. Ricorda che HTML controlla in che modo è organizzato il tuo sito web e il CSS controlla come appare.

## Sfida: organizza il tuo sito web

+ Prova ad organizzare in questo modo tutti i contenuti del tuo sito web, utilizzando i contenitori `article` e `section`. 

\--- hints \---

\--- hint \---

Guarda la pagina Cibo del progetto di esempio. Vedrai che ho aggiunto un `article` con un gruppo di tag `section` nel file `food.html`:

```html
  <main>
    <article>
      <h1>Cibo in Irlanda</h1>
      <p>
        Questi sono alcuni dei miei cibi irlandesi preferiti!
      </p>  
      <section>
        <h2>Colazione irlandese tradizionale</h2>
        <p>
         Una colazione "Full Irish" è costituita da salsicce, fette di bacon, uova, sanguinaccio, pudding e toast.
        </p>
        <p>
          Spesso ci saranno anche un pomodoro alla griglia, funghi e fagioli stufati.
        </p>
        <p>
          E, naturalmente, nessuna colazione è completa senza una bella tazza di tè!
        </p>
      </section>

      <section>
        <h2>Bangers and Mash</h2>
        <p>
          Questo classico di salsicce, patate schiacciate e sugo non è unico dell'Irlanda, ma ciò che lo rende speciale sono le salsicce irlandesi. La maggior parte dei Paesi ha il suo modo di fare le salsicce e queste sono una delle cose che mi manca di casa quando sono in viaggio!
        </p>
      </section>

      <section>
        <h2>Bacon e Cavolo</h2>
        <p>
         Non potrei fare un elenco di cibo irlandese senza includere questo piatto veramente tradizionale!
        </p>
        <p>
         Potrebbe non sembrare molto interessante, ma questo lauto piatto a base di prosciutto bollito, patate e cavolo verde è gustoso e saziante.
          Amo affogare le patate nel burro e mi piace anche un po' di senape con il bacon.
        </p>
        <p>
          Mia mamma lo rendeva sempre speciale cucinando il cavolo nell'acqua in cui il prosciutto era bollito.
        </p>
        <p>
          Se ci sono avanzi si può fare un altro dei miei preferiti: <strong>cavolo fritto</strong>!
        </p>
      </section>
    </article>     
  </main>
```

\--- /hint \---

\--- /hints \---

Nella prossima card, disegnerai un tema diverso per ogni pagina che è organizzata in articoli e sezioni!

\--- /challenge \---