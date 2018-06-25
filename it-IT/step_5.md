## Organizzazione della tua pagina

Finora hai usato **titoli** e **paragrafi** per rendere il tuo contenuto **** ordinato e facile da leggere. Rendiamolo ancora più organizzato raggruppando le cose.

## \--- chiudi \---

## titolo: qual è il contenuto?

**contenuto** è tutto ciò che c'è nella tua pagina web, come testo e immagini.

\--- / chiudi \---

+ Vai `attractions.html` di file (o una delle tue pagine, se non si sta usando il progetto di esempio) e, nella parte superiore, appena **sotto** l'apertura `<main>` tag, digitare quanto segue in una nuova riga : 

```html
  <main>
    <article>
```

+ Se il tuo editor viene automaticamente aggiunto in un tag di chiusura `</article>` , eliminalo.

+ Nella parte inferiore del file, solo **sopra** il tag di chiusura `</main>` , aggiungi una nuova riga e chiudi l'elemento `article`:

```html
    </article>
  </main>
```

Il tuo `elemento principale` dovrebbe apparire come questo ora (potresti avere contenuti diversi tra i `tag dell'articolo` ovviamente):

```html
  <main>
    <article>
      <h1>I miei posti preferiti da vedere in Irlanda</h1>
        <h2>The Cliffs of Moher</h2>
        <p>
        Le Cliffs of Moher si trovano nella Contea di Clare, da dove vengo. Guarda quanto sono cool!</p>
        <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
        <h2>Achill Island</h2>
        <p>Questa è una grande isola al largo della contea di Mayo. Ha un paesaggio selvaggio e bellissimo di montagne, torbiere e scogliere.
        </p>
        <img src="achill.JPG" width="200px" />
    </article>
  </main>
```

+ Ora guarda il contenuto nel tuo `articolo` e prova a suddividerlo in sezioni. Metti questa nuova coppia di tag attorno ad ogni bit: `<section> </section>`. Ecco un esempio di come potrebbe essere:

```html
  <article>
    <h1>I miei posti preferiti da vedere in Irlanda</h1>
    <section>
      <h2>The Cliffs of Moher</h2>
      <p>
      Le Cliffs of Moher si trovano nella Contea di Clare, da dove vengo. Guarda quanto sono cool!</p>
      <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
    </section>
    <section>
      <h2>Achill Island</h2>
      <p>Questa è una grande isola al largo della contea di Mayo. Ha un paesaggio selvaggio e bellissimo di montagne, torbiere e scogliere.
      </p>
      <img src="achill.JPG" width="200px" />
    </section>
  </article>
```

## \--- chiudi \---

## titolo: quali sono i nuovi tag?

Pensa a questi nuovi elementi come **contenitori**. Sono usati per raggruppare le cose. È un po 'come organizzare le cose in scatole e scaffali nella tua casa!

Questo rende il tuo sito web amichevole per i lettori di schermo, ti dà un maggiore controllo sul layout e, come vedrai, ti permette di diventare davvero creativo con lo stile.

Qualsiasi cosa può andare tra i tag. Di solito sarà più di un elemento, ma non deve essere. Può essere elementi HTML di qualsiasi tipo. Quello che stai facendo è dire al browser che tutto ciò che sta tra questi tag appartiene insieme.

### Articolo

L'elemento `articolo` è un contenitore per un intero contenuto, in questo caso un insieme di informazioni sulle attrazioni in Irlanda. Se hai diversi bit di contenuto che non sono correlati, dovresti inserire ognuno nel proprio elemento articolo</code> `invece di mettere un set di tag attorno all'intero lotto.</p>

<h3>Sezione</h3>

<p>L'elemento <code>sezione` ti consente di suddividere il contenuto correlato in blocchi più piccoli e di inserire ciascun blocco nel proprio contenitore.

### Anche gli altri esistono!

Questi non sono gli unici elementi contenitore in HTML. Se hai mai creato un menu e poi lo hai inserito tra i tag `<nav> </nav>` , questo è un altro esempio di un tipo di contenitore. Quindi sono `<main> </main>` e `<header> </header>` - riesci a pensarci ancora?

\--- / chiudi \---

\--- sfida \---

La tua pagina web potrebbe non sembrare ancora diversa, ma una volta che il contenuto è stato organizzato in tag contenitore, sarai in grado di fare alcune cose interessanti con i CSS. Ricorda che HTML controlla in che modo è organizzato il tuo sito web e il CSS controlla come appare.

## Sfida: organizza il tuo sito web

+ Esegui l'organizzazione di tutti i contenuti del tuo sito web utilizzando i contenitori `articolo` e `sezione` in questo modo. 

\--- suggerimenti \---

\--- suggerimento \---

Guarda la pagina Cibo del progetto di esempio. Vedrai che ho aggiunto un `articolo` con un gruppo di `sezioni` tag nel file `food.html`:

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
          Una colazione "irlandese completa" composta da salsicce, fette di lardo (pancetta), uova, sanguinaccio, sanguinaccio e pane tostato.
        </p>
        <p>
          Spesso ci sarà un pomodoro grigliato e funghi e fagioli al forno.
        </p>
        <p>
          E, naturalmente, nessuna colazione è completa senza una bella tazza di tè!
        </p>
      </section>

      <section>
        <h2>Bangers and Mash</h2>
        <p>
          Questo classico di salsicce, purè di patate e sugo non è unico in Irlanda, ma ciò che lo rende speciale sono le salsicce irlandesi. La maggior parte dei paesi ha il proprio modo di fare le salsicce, e sono una cosa che mi manca da casa se sono fuori casa!
        </p>
      </section>

      <section>
        <h2>Pancetta e cavolo</h2>
        <p>
          Non potrei fare una lista di cibo irlandese senza includere questo piatto molto tradizionale!
        </p>
        <p>
          Potrebbe non sembrare molto interessante, ma questo abbondante pasto a base di prosciutto cotto, patate e cavolo verde è gustoso e abbondante.
          Adoro soffocare le patate nel burro e mi piace anche una piccola mostarda con la pancetta.
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

\--- / suggerimento \---

\--- / suggerimenti \---

Sulla prossima carta, disegnerai un tema diverso per ogni pagina che è organizzata in articoli e sezioni!

\--- / challenge \---