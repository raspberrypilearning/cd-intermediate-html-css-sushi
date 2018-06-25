## Animazione

Sapevi che puoi usare i CSS per far muovere le cose? Imparerai come su questa carta!

+ Prima di iniziare, assicurati di avere un'immagine sul tuo sito Web con `id` e un blocco CSS corrispondente che imposta la larghezza `` a `100px`. Vado con l'immagine di Tito di prima, e il mio blocco CSS assomiglia a questo:

```css
    #titoPicture {border-radius: 100%; larghezza: 100 px; }
```

+ Vai in fondo al tuo file CSS e aggiungi il seguente codice:

```css
    @keyframes myFirstAnimation {from {width: 100px; } a {width: 300px; }}
```

Questo codice crea un'animazione chiamata `myFirstAnimation` che puoi aggiungere a qualsiasi elemento sul tuo sito web. Cosa pensi che farà?

+ Trova le tue regole CSS per l'immagine e aggiungi le seguenti tre proprietà:

```css
    nome-animazione: myFirstAnimation; durata dell'animazione: 2 secondi; animazione-iterazione: 1;
```

+ Ora guarda cosa succede sulla tua pagina web! Prova diversi valori per `animazione-iteration-count` per vedere cosa fa.

+ Proviamo un'altra animazione! Aggiungi il seguente codice alla fine del tuo file CSS:

```css
    @keyframes rainbowGlow {0% {color: # FFD700; } 50% {color: # 663399; } 100% {color: # FFD700; }}
```

+ Ora trova `#myCoolText` regole CSS precedenti e aggiungi il codice dell'animazione:

```css
    #myCoolText {color: # 003366; border: 2px ridge #ccffff; imbottitura: 15px; allineamento del testo: centro; nome-animazione: rainbowGlow; durata dell'animazione: 1,5 s; animazione-iterazione: 1; }
```

Quando utilizzi **valori percentuali** invece di `da` e da `a`, puoi impostare valori intermedi oltre a valori iniziali e finali. È possibile impostare tutti i valori intermedi desiderati utilizzando diversi valori percentuali da `0` fino a `100`.

+ Cambia il valore di `animazione-iterazione: conta da` a `infinito`. Vedi se riesci a indovinare cosa accadrà prima di testarlo!

+ Prova diversi valori per `animazione-durata` per accelerare o rallentare l'animazione.

+ Un ultimo trucco! Aggiungi questo codice di animazione:

```css
    @keyframes slide {0% {background-position-x: 0; } 100% {background-position-x: 600vw; }}
```

+ Ora trova i `#FrontPage` regole CSS che hai scritto in precedenza e cambiarle a:

```css
    #frontPage {background: ripetizione-linear-gradient (-45deg, rosso 0%, giallo 7,14%, calce 14,28%, cyan 21,42%, ciano 28,56%, blu 35,7%, magenta 42,84%, rosso 50%); dimensione dello sfondo: 600vw 600vw; animazione: slide 10s infiniti forward lineari; }
```

Non preoccuparti di capire tutto il codice sopra ... semplicemente siediti e divertiti !!

Per ulteriori informazioni su altre cose che puoi fare con l'animazione, visita [questa pagina web](http://dojo.soy/html2-css-animation){: target = "_ blank"}. Divertiti!

Nella prossima carta imparerai come far accadere cose interessanti quando passi il cursore del mouse sulle cose!