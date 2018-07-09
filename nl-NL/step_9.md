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

Another way to set the size of things is using **relative** measurements, so that size depends on how big elements are compared to each other. Then, whenever one thing changes size, everything else will automatically change size as well to keep the same **proportions**.

When you're using **relative** measurements, it's important to know what the **parent** of your element is. The parent is the thing that your element is inside of, and that's what the measurement will be in relation to. For example, the parent of the image above is the `article` element, because the `img` element is in between the `<article></article>` tags.

If you set the `width` of an element to `100%`, that will make it be the same width as the parent container it's in.

\--- /collapse \---

+ Experiment with different numbers in front of the `%`.