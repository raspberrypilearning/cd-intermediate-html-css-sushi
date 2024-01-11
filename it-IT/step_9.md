## Animazione

Sapevi che puoi usare i CSS per far muovere le cose? Imparerai come in questa scheda!

+ Prima di iniziare, assicurati di avere un'immagine sul tuo sito Web con un `id` e un blocco CSS corrispondente che imposta la larghezza (`width`) a `100px`. Uso l'immagine di Tito di prima, e il mio blocco CSS assomiglia a questo:

```css
    #titoPicture {
        border-radius: 100%;
        width: 100px;
    }
```

+ Vai in fondo al tuo file CSS e aggiungi il seguente codice:

```css
    @keyframes myFirstAnimation {
        from {
            width: 100px;
        }
        to {
            width: 300px;
        }
    }
```

Questo codice crea un'animazione chiamata `myFirstAnimation` che puoi aggiungere a qualsiasi elemento sul tuo sito web. Cosa pensi che farà?

+ Trova le tue regole CSS per l'immagine e aggiungi le seguenti tre proprietà:

```css
    animation-name: myFirstAnimation;
    animation-duration: 2s;
    animation-iteration-count: 1;
```

+ Ora guarda cosa succede sulla tua pagina web! Prova diversi valori per `animation-iteration-count` per vedere cosa fa.

+ Proviamo un'altra animazione! Aggiungi il seguente codice alla fine del tuo file CSS:

```css
    @keyframes rainbowGlow {
        0% {
            color: #FFD700;
        }
        50% {
            color: #663399;
        }
        100% {
            color: #FFD700;
        }
    }
```

+ Ora trova le regole CSS `#myCoolText` create in precedenza e aggiungi il codice dell'animazione:

```css
    #myCoolText {        
        color: #003366;
        border: 2px ridge #ccffff;
        padding: 15px;
        text-align: center;
        animation-name: rainbowGlow;
        animation-duration: 1.5s;
        animation-iteration-count: 1;
    }
```

Quando utilizzi **valori percentuali** invece di `from` e `to`, puoi impostare valori intermedi oltre ai valori iniziali e finali. È possibile impostare tutti i valori intermedi desiderati utilizzando diversi valori percentuali da `0` fino a `100`.

+ Cambia il valore di `animation-iteration-count` a `infinite`. Vedi se riesci a indovinare cosa accadrà prima di testarlo!

+ Prova diversi valori per `animazione-durata` per accelerare o rallentare l'animazione.

+ Un ultimo trucco! Aggiungi questo codice di animazione:

```css
    @keyframes slide {
        0% {
            background-position-x: 0;
        }
        100% {
            background-position-x: 600vw;
        }
    }
```

+ Ora trova le regole CSS `#FrontPage` che hai scritto in precedenza e cambiale in:

```css
    #frontPage {
        background: repeating-linear-gradient(-45deg, red 0%, yellow 7.14%, lime 14.28%, cyan 21.42%, cyan 28.56%, blue 35.7%, magenta 42.84%, red 50%);
        background-size: 600vw 600vw;
        animation: slide 10s infinite linear forwards;
    }
```

Non preoccuparti di capire tutto il codice sopra... semplicemente siediti e divertiti!!

Per ulteriori informazioni su altre cose che puoi fare con l'animazione, visita [questa pagina web](http://dojo.soy/html2-css-animation){:target="_blank"}. Divertiti!

Nella prossima scheda imparerai come far accadere cose interessanti quando passi il cursore del mouse sulle cose!