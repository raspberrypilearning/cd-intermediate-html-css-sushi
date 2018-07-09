## Automatisch de grootte aanpassen

Tot nu toe heb je **pixels** gebruikt om de grootte van dingen in te stellen, bijv. `10px`. Op deze kaart leer je over andere afmetingen die je kunt gebruiken.

+ Ga naar `index.html` en zoek het `img` element met de afbeelding van Tito, of zoek een andere `afbeelding` tag op je website.

+ Verwijder het `with` attribuut als het er is, en geef het element een `id` als het er nog geen heeft.

```html
  <img src="tito.png" id="titoPicture" alt="Tito the dog" />
```

+ Definieer in je CSS-bestand de `with` eigenschappen voor je foto, zoals hieronder weergegeven (je moet mogelijk het CSS-blok met de `id` selector maken als je dit nog niet in een eerdere kaart gedaan hebt).

```css
  #titoPicture {
    width: 50%;
    border-radius: 100%;
  }
```

Opmerking: 50% (50 procent) is **de helft**.

+ Probeer het formaat van je browservenster aan te passen en kijk wat er met de foto gebeurt.

Je zou moeten zien dat de foto groter en kleiner wordt als je het venster groter en kleiner maakt. Dat komt omdat het 50% van de breedte van het **main** (hoofd) element in beslag neemt (dat is ongeveer de breedte van de pagina).

## \--- collapse \---

## title: Hoe werkt het?

Wanneer je de grootte van iets in pixels instelt, stel je een exacte grootte in en deze verandert niet. Dit wordt een **absolute** afmeting genoemd.

Een andere manier om de grootte van de dingen in te stellen is het gebruik van **relatieve** afmetingen, zodat de grootte afhankelijk is van hoe elementen met elkaar worden vergeleken. Zodat, wanneer een ding van afmeting verandert, ook al het andere automatisch van grootte verandert om dezelfde **verhoudingen** te behouden.

Wanneer je **relatieve** afmetingen gebruikt, is het belangrijk om te weten wat de **parent** (ouder) van je element is. De parent (ouder) is het element waar het in zit, en dat is waarmee de afmeting in relatie zal zijn. Als voorbeeld: de parent van de afbeelding hierboven is het `article` element, omdat het `img` element zich tussen de `<article></article>` tags bevindt.

Als je de `with` van een element ingesteld op `100%`, dat zal dat dezelfde breedte hebben als de container waarin het zich bevindt.

\--- /collapse \---

+ Experimenteer met verschillende nummers voor de `%`.