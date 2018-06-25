## Regola automaticamente le dimensioni

Fino ad ora hai usato **pixel** per impostare la dimensione delle cose, ad esempio `10px`. Su questa carta imparerai altre misurazioni che puoi usare.

+ Vai a `index.html` e trova l'elemento `img` con l'immagine di Tito o trova un altro tag `img` sul tuo sito web.

+ Elimina l'attributo `larghezza` se è lì e assegna all'elemento un `id` se non ne ha già uno.

```html
  <img src="tito.png" id="titoPicture" alt="Tito the dog" />
```

+ Nel tuo file CSS, definisci la proprietà `width` per la tua immagine come mostrato di seguito (potresti aver bisogno di creare il blocco CSS con il `selettore id` se non lo hai già fatto su una scheda precedente).

```css
  #titoPicture {width: 50%; border-radius: 100%; }
```

Nota: il 50% (50%) è **metà**.

+ Prova a ridimensionare la finestra del browser e guarda cosa succede alla foto.

Dovresti vedere che l'immagine diventa sempre più piccola quando ingrandisci e riduci la finestra. Questo perché occupa il 50% della larghezza dell'elemento **principale** (che è approssimativamente la larghezza della pagina).

## \--- chiudi \---

## titolo: come funziona?

Quando si imposta la dimensione di qualcosa in pixel, si imposta una dimensione esatta e non cambia. Questa è chiamata una misura **assoluta**.

Un altro modo per impostare la dimensione delle cose consiste nell'utilizzare **misurazioni relative** , in modo che la dimensione dipenda da quanto sono grandi gli elementi confrontati l'uno con l'altro. Quindi, ogni volta che una cosa cambia dimensione, tutto il resto cambierà automaticamente anche le dimensioni per mantenere le stesse proporzioni ****.

Quando utilizzi **misurazioni relative** , è importante sapere qual è il **genitore** del tuo elemento. Il genitore è la cosa in cui si trova il tuo elemento, ed è a questo che la misura sarà in relazione. Ad esempio, il genitore dell'immagine sopra è l'elemento `articolo` , perché l'elemento `img` è tra i `<article></article>` tag.

Se si imposta la larghezza `` di un elemento su `100%`, ciò lo renderà della stessa larghezza del contenitore genitore in cui si trova.

\--- / chiudi \---

+ Sperimenta con numeri diversi di fronte allo `%`.