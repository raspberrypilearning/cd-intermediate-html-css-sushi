## Insegna a Tito di girarsi!

È possibile rendere il vostro sito web più **interattivo** facendo cose interessanti accadere quando si passa sopra le cose con il cursore del mouse!

+ Trova le tue regole CSS per gli elementi `img` o creane alcune se non ne hai. Aggiungi un bordo e aggiungi un nuovo blocco di regole subito sotto:

```css
  img {border: 2px solid White; } img: hover {border: 2px dashed Navy; }
```

Hai appena usato un tipo speciale di blocco CSS chiamato **pseudo-classe**.

## \--- chiudi \---

## titolo: come funziona?

A **pseudo-classe** è un po 'diverso da un **di classe** che si crea da soli. Puoi riconoscerlo con `:`.

Le pseudo-classi sono incorporate in elementi HTML: puoi aggiungere `: regole di stile hover` a qualsiasi elemento, classe o `selettore id` nel tuo foglio di stile senza aggiungere nulla di extra nel tuo codice HTML.

\--- / chiudi \---

+ Cosa pensi che succederà? Verifica quali pagine del tuo sito web contengono immagini (aggiungi una foto se non ce ne sono!), Quindi sposta il cursore su un'immagine per scoprirlo!

+ Usiamo questo nuovo `: pseudo-classe hover` insieme a una classe CSS per far risplendere i link quando passi il mouse su di loro! Aggiungi un link alla tua pagina web e includi un attributo per specificare il nome della classe. Ricorda, i collegamenti sono definiti usando il tag `<a>` , in questo modo:

```html
    <p>
      Visita la pagina <a class="niceLinks" href="https://en.wikipedia.org/wiki/Ireland">Wikipedia</a> per saperne di più sull'Irlanda!
    </p>
```

+ Aggiungi il seguente codice al tuo foglio di stile, quindi esegui il codice per vedere i tuoi link adorabili in azione.

```css
  .niceLinks {text-decoration: none; colore: # FFFAF0; } .niceLinks: hover {color: # 00FF7F; }
```

+ Perché non aggiungere l'attributo `class = "niceLinks"` a tutti i link nella barra dei menu?

Puoi anche combinare tutti questi trucchi con le animazioni!

+ Trova di nuovo il blocco CSS per l'immagine di Tito (o qualsiasi altra immagine a cui stavi lavorando in precedenza). Aggiungi il seguente codice al tuo foglio di stile:

```css
  #titoPicture {border-radius: 100%; larghezza: 100 px; } #titoPicture: hover {nome-animazione: rollOver; durata animazione: 1s; animazione-iterazione: 1; } @keyframes rollOver {0% {transform: rotate (0deg); } 100% {transform: ruotare (-360 gradi); }}
```

+ Riesci a indovinare cosa accadrà?

+ Ora urla "Roll over!" mentre muovi il cursore sull'immagine!

\--- sfida \---

## Sfida: crea collegamenti arcobaleno luminosi

+ Puoi usare l'animazione `rainbowGlow` dalla scheda precedente per far sì che i collegamenti nel tuo menu continuino a cambiare colore quando il cursore passa sopra di loro?

\--- suggerimenti \---

\--- suggerimento \---

Di seguito è riportato il codice per l'animazione `rainbowGlow`. Ha cinque livelli definiti e imposta un diverso colore del testo in ogni fase. Puoi aggiungerne altri o cambiarli come preferisci!

```css
    @keyframes rainbowGlow {0% {color: # 00BFFF; } 25% {color: # 00FF7F; } 50% {color: #eeeeaf; } 75% {color: #eeafee; } 100% {color: # 00BFFF; }}
```

\--- / suggerimento \---

\--- suggerimento \---

Per animare qualcosa, aggiungi le tre `proprietà dell'animazione` alle sue regole di stile come hai fatto sopra. Assicurati sempre che il nome dell'animazione `` corrisponda al nome dell'animazione che desideri utilizzare.

\--- / suggerimento \---

\--- suggerimento \---

Puoi aggiungere `effetti hover` direttamente al menu `nav` questo modo:

```css
  nav ul li a: hover {nome-animazione: rainbowGlow; durata dell'animazione: 1,5 s; animazione-iterazione-conteggio: infinito; }
```

Oppure, se desideri creare altri collegamenti sul tuo sito Web anche con i colori dell'arcobaleno, puoi aggiungere l'animazione alla classe `.niceLinks` , in questo modo:

```css
  .niceLinks: hover {color: # 00BFFF; nome-animazione: rainbowGlow; durata dell'animazione: 1,5 s; animazione-iterazione-conteggio: infinito; }
```

\--- / suggerimento \---

\--- / suggerimenti \---

\--- / challenge \---

![](images/badge-footer-image-html-intermed.png)