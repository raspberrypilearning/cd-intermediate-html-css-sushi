## Je pagina organiseren

Tot dusverre heb je **koppen** en **alinea's** gebruikt om je **inhoud** te maken, er netjes uit te laten zien en ervoor gezorgd dat het gemakkelijk te lezen is. Laten we het nog beter organiseren door dingen samen te voegen.

## \--- collapse \---

## title: wat is inhoud?

**Inhoud** is alles op je webpagina, zoals tekst en afbeeldingen.

\--- /collapse \---

+ Ga naar het bestand `attractions.html` (of een van je eigen pagina's als je het voorbeeldproject niet gebruikt) en bovenaan, net **onder** de `<main>` tag, typ je het volgende op een nieuwe regel: 

```html
  <main>
    <article>
```

+ Als jouw editor automatisch een sluit `</article>` tag toegevoegd, verwijder deze dan.

+ Onderaan het bestand, net **boven** de `</main>` tag, voeg je een nieuwe regel toe en sluit het `article` element:

```html
    </article>
  </main>
```

Je `main` element zou er nu ongeveer zo uit moeten zien (jij hebt mogelijk andere inhoud tussen de `article` tags):

```html
  <main>
    <article>
        <h1> Mijn favoriete plekken om te zien in Ierland </h1>  
          <h2> De kliffen van Moher </h2> 
          <p> 
          De kliffen van Moher zijn te vinden in County Clare, waar ik vandaan kom. Kijk hoe mooi het er is!</p>
        <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
        <h2>Texel</h2>
        <p>Dit is het grootste eiland van Nederland. Er zijn schapen en
        een prachtig landschap met stranden en duinen.
        </p>
        <img src="achill.JPG" width="200px" />
    </article>
  </main>
```

+ Bekijk nu de inhoud in je ` artikel ` en probeer het op te splitsen in secties. Plaats de volgende nieuwe tags rond elk deel: `<section> </section>`. Hier is een voorbeeld van hoe het eruit zou kunnen zien:

```html
  <article>
    <h1>Mijn favoriete plaatsen in Nederland</h1>
    <section>
      <h2>De Hoge Veulwe</h2>
      <p>
      De Hoge Veluwe is een natuurgebied in de provincie Gelderland. Look how cool they are!</p>
      <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
    </section>
    <section>
      <h2>Texel</h2>
      <p>Dit is het grootste eiland van Nederland. Er zijn schapen en
        een prachtig landschap met stranden en duinen.
      </p>
      <img src="achill.JPG" width="200px" />
    </section>
  </article>
```

## \--- collapse \---

## title: Waar gaan de nieuwe tags over?

Zie deze nieuwe elementen als ** containers **. Ze worden gebruikt om dingen te groeperen (samen te voegen). Het is een beetje alsof je dingen in dozen en planken bij je thuis organiseert!

Dit maakt je website vriendelijk voor schermlezers, geeft je meer controle over de lay-out (opmaak) en, zoals je zult zien, kun je met de styling echt creatief worden.

Alles kan tussen de tags gaan. Meestal zal het meer dan één element zijn, maar dat hoeft niet zo te zijn. Het kunnen allerlei soorten HTML-elementen zijn. Wat je doet, is de browser laten weten dat alles tussen deze tags bij elkaar hoort.

### Article

Het `article `(artikel) element is een container voor een heel stuk inhoud, in dit geval een verzameling informatie over bezienswaardigheden in Nederland. Als je verschillende stukjes inhoud hebt die geen verband met elkaar hebben, moet je elke stuk in een eigen ` article ` element plaatsen in plaats van de tags rond de gehele inhoud zetten.

### Section

Met het `section ` element kunt je verwante inhoud verdelen in kleinere delen en elk deel in een eigen container plaatsen.

### Andere containers bestaan ook nog!

Dit zijn niet de enige container elementen in HTML. Als je ooit een menu hebt gemaakt en vervolgens tussen `<nav> </nav>` tags hebt geplaatst, is dat een ander voorbeeld van een type container. Dat geldt ook voor `<main> </main>` en `<header> </header>` - kan jij er nog meer bedenken?

\--- /collapse \---

\--- challenge \---

Je webpagina ziet er misschien nog niet zo anders uit, maar zodra de inhoud is georganiseerd in container tags, kunt je er met CSS leuke dingen mee doen. Onthoud dat HTML bepaalt hoe je website is georganiseerd en CSS bepaalt hoe het eruit ziet.

## Uitdaging: organiseer je website

+ Probeer de inhoud van je website op deze manier met behulp van de ` article ` en ` section ` containers te organiseren. 

\--- hints \---

\--- hint \---

Kijk naar de Food-pagina van het voorbeeldproject. Je ziet dat ik een ` article ` heb toegevoegd met een heleboel ` section ` tags in het bestand ` food.html `:

```html
  <main>
    <article>
      <h1>Eten in Nederland</h1>
      <p>
        Dit zijn enkele favoriete gerechten van mij!
      </p>  
      <section>
        <h2>Een broodjes ontbijt</h2>
        <p>
          Een compleet ontbijt met broodjes, gekookt eitje,
          jus d'orange en een beschuitje.
        </p>
        <p>
          Often there will be a grilled tomato as well as mushrooms,
          and baked beans.
        </p>
        <p>
          And of course, no breakfast is complete without a lovely pot 
          of tea!
        </p>
      </section>

      <section>
        <h2>Bangers and Mash</h2>
        <p>
          This classic of sausages, mashed potato and gravy is not
          unique to Ireland, but what makes it special is the Irish
          sausages. Most countries have their own way of making sausages,
          and they are one thing I miss from home if I'm away travelling!
        </p>
      </section>

      <section>
        <h2>Bacon and Cabbage</h2>
        <p>
          I couldn't possibly make a list of Irish food without including
          this very traditional dish!
        </p>
        <p>
          It might not sound very interesting, but this hearty meal of
          boiled ham, potatoes and green cabbage is tasty and filling.
          I love to smother the potatoes in butter, and I also like a
          little mustard with the bacon.
        </p>
        <p>
          My mum always made it extra special by cooking the cabbage in
          the water that the ham was boiled in.
        </p>
        <p>
          If there are any leftovers you can make another one of my
          favourites: <strong>fried cabbage</strong>!
        </p>
      </section>
    </article>     
  </main>
```

\--- /hint \---

\--- /hints \---

On the next card, you'll design a different theme for each page that's organised into articles and sections!

\--- /challenge \---