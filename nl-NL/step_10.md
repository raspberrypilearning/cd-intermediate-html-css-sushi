## Animatie

Wist je dat je CSS kunt gebruiken om dingen te laten bewegen? Hoe zul je leren op deze kaart!

+ Voordat je begint, zorg ervoor dat je een afbeelding op je website hebt met een `id` en een bijbehorende CSS blok welke de `width` instelt op `100 pixels`. Ik gebruik het beeld van Tito van hiervoor, en mijn CSS blok ziet er als volgt uit:

```css
    #titoPicture {
        border-radius: 100%;
        width: 100px;
    }
```

+ Ga naar het einde van je CSS bestand en voeg de volgende code toe:

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

Deze code maakt een animatie met de naam `myFirstAnimation` (mijnEersteAnimatie) aan die je aan elk element op je website kunt toevoegen. Wat denk je dat het zal doen?

+ Zoek je CSS regels voor de afbeelding en voeg de volgende drie eigenschappen toe:

```css
    animation-name: myFirstAnimation;
    animation-duration: 2s;
    animation-iteration-count: 1;
```

+ Bekijk nu wat er gebeurt op je webpagina! Probeer verschillende waarden voor `animatie-iteratie-count` om te zien wat het doet.

+ Laten we een andere animatie proberen! Voeg de volgende code toe aan het einde van je CSS-bestand:

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

+ Zoek nu de `#myCoolText` CSS regels van hiervoor en voeg de animatiecode toe:

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

Wanneer je **procentuele waarden** gebruikt in plaats van `from` en `to`, kun je tussen waarden instellen en niet alleen begin- en eindwaarden. Je kunt net zoveel tussenliggende waarden instellen als je wilt, met verschillende percentages van `0` helemaal tot `100`.

+ Wijzig de waarde van `animation-iteration-count` tot `infinite` (oneindig). Kijk of je kunt raden wat er zal gebeuren voordat je het test!

+ Probeer verschillende waarden uit voor `animation-duration` om je animatie te versnellen of te vertragen.

+ Een laatste truc! Voeg deze animatiecode toe:

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

+ Zoek nu de `#frontPage` CSS-regels die je eerder hebt geschreven en wijzig deze in:

```css
    #frontPage {
        background: repeating-linear-gradient(-45deg, red 0%, yellow 7.14%, lime 14.28%, cyan 21.42%, cyan 28.56%, blue 35.7%, magenta 42.84%, red 50%);
        background-size: 600vw 600vw;
        animation: slide 10s infinite linear forwards;
    }
```

Maak je geen zorgen als je bovenstaande code niet begrijpt ... leun achterover en geniet ervan!!

Ga naar [deze webpagina](http://dojo.soy/html2-css-animation) {: Target = "_ blank"} voor meer informatie over andere dingen die je met animatie kunt doen. Veel plezier!

Op de volgende kaart leer je hoe je leuke dingen kunt laten gebeuren als je met de muis over dingen beweegt!