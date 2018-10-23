## Disegna alcuni temi

Scrivere regole CSS per elementi come `section` e `p` è grandioso, ma cosa succede se si desidera che alcune di esse siano diverse dalle altre? In questa card imparerai come applicare diversi set di regole di stile a elementi dello stesso tipo e creare un tema diverso per ogni pagina del tuo sito web!

+ Vai al tuo foglio di stile e aggiungi quanto segue: assicurati di includere il punto davanti!

```css
  .topDivider {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #F5FFFA;
  padding-bottom: 10px;
}
```

+ Ora vai al file `attractions.html` (o al file HTML su cui stai lavorando se stai utilizzando il tuo progetto) e aggiungi il seguente **attributo** a ogni tag `section`:

```html
  <section class="topDivider">
```

Dovresti vedere apparire una linea sopra ogni sezione della pagina. Congratulazioni: hai appena usato la tua prima **classe CSS**!

![Pagina con linee tra le sezioni](images/sectionsWithTopBorder.png)

+ Guarda come appare la tua pagina web ora e confrontala con le altre pagine che hanno elementi `section`. Vedrai che solo quelli in cui hai aggiunto l'attributo `class="topDivider"` avranno la riga sopra.

## \--- collapse \---

## title: Come funziona?

Ricorda che quando usi un **selettore** CSS come `section` o `p` o `nav ul`, le regole di stile si applicano a **tutti** gli elementi di quel tipo nel tuo sito web.

Con le **classi** CSS, puoi modificare lo stile di solo **alcuni** elementi.

Mettere un punto davanti al tuo selettore lo trasforma in un **selettore di classe**. Una classe può avere qualsiasi nome, quindi non deve essere il nome di un elemento HTML. Per esempio:

```css
  .laMiaFantasticaClasse {
/ * le mie fantastiche regole di stile vanno qui * /
}
```

Per scegliere a quali elementi si applicano le regole di stile, devi aggiungere l'**attributo** `class` a quegli elementi nel codice HTML: inserisci il nome della classe come valore dell'attributo, **senza** il punto, in questo modo:

```html
  class="laMiaFantasticaClasse"
```

\--- /collapse \---

+ Pronto a provare un'altra lezione? Aggiungi il seguente codice CSS a `styles.css`:

```css
  .stylishBox {
background-color: #87CEFA;
color: #A52A2A;
border-style: solid;
border-width: 2px;
border-color: #F5FFFA;
border-radius: 10px;
}
```

+ Quindi, su una pagina diversa del tuo sito web, aggiungi la classe ad alcuni elementi presenti. Ho intenzione di aggiungerlo agli elementi `section` nella pagina Cibo del mio sito, in questo modo: `<section class="stylishBox">`.

Sembra fantastico, ma ora le mie sezioni sono tutte schiacciate insieme.

![Sezioni dall'aspetto piacevole schiacciate insieme](images/squashedSections.png)

Puoi applicare ad un elemento tutte le classi CSS che vuoi. Basta scrivere i nomi di tutte le classi che vuoi usare all'interno dell'attributo `class` (ricorda, senza il punto!), separandole con spazi.

+ Facciamo un'altra classe CSS per dare alle sezioni un margine (margin) e un riempimento (padding). Nel file `styles.css`, crea la seguente classe CSS:

```css
  .someSpacing {
padding: 10px;
margin-top: 20px;
}
```

+ Nel tuo codice `html`, aggiungi la nuova classe a ciascuno degli elementi su cui stavi lavorando, in questo modo:

```html
  <section class="stylishBox someSpacing">
```

![Sezioni con margine e padding aggiunti](images/sectionsWithSpacing.png)

Quindi, le classi CSS consentono di **scegliere** quali elementi stilizzare, e ti lasciano **riutilizzare** lo stesso insieme di regole di stile su tutti gli elementi che desideri.

+ Vai al file `index.html` e aggiungi la classe `stylishBox` all'elemento `main`, o ad un altro elemento della pagina. Puoi rimuoverlo di nuovo in seguito!

```html
    <main class="stylishBox">   
```

Ecco come appare la mia home page con la classe CSS. Ho anche aggiunto la classe `topDivider` al tag `img` con l'immagine di Tito.

![Classi CSS utilizzate nella home page](images/homePageWithClasses.png)

\--- challenge \---

## Sfida: crea nuove classi

+ Utilizza le **classi** CSS per definire alcune dimensioni di immagine diverse per il tuo sito Web, ad esempio `.smallPictures` e `.mediumPictures`. Quindi rimuovi l'attributo `width` da ciascuno dei tuoi elementi `img` e aggiungi invece la classe appropriata.

\--- hints \---

\--- hint \---

Puoi creare una classe CSS che definisca solo la larghezza di un elemento come questo:

```css
  .smallPictures {width: 100px; }
```

\--- /hint \---

\--- hint \---

Ecco un tag `img` con un attributo `width`:

```html
  <img src="tito.png" alt="Tito the dog" width="100px" />       
```

Quando rimuovi l'attributo `width` e controlli invece la dimensione con la classe CSS, assomiglia a questo:

```html
  <img src="tito.png" class="smallPictures" alt="Tito the dog" />       
```

Usando una classe CSS, puoi modificare facilmente la larghezza di tutte le immagini contemporaneamente cambiando solo una riga di codice nel tuo foglio di stile!

\--- /hint \---

\--- /hints \---

\--- /challenge \---