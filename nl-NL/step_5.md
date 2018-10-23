## Je pagina organiseren

Tot dusverre heb je **koppen** en **alinea's** gebruikt om je **inhoud** te maken, er netjes uit te laten zien en ervoor gezorgd dat het gemakkelijk te lezen is. Laten we het nog beter organiseren door dingen samen te voegen.

## \--- collapse \---

## title: Wat is inhoud?

**Inhoud** is alles op je webpagina, zoals tekst en afbeeldingen.

\--- /collapse \---

+ Ga naar het bestand `attractions.html` (of een van je eigen pagina's als je het voorbeeldproject niet gebruikt) en bovenaan, net **onder** de `<main>` tag, typ je het volgende op een nieuwe regel: 

```html
  <main>
    <article>
```

+ Als jouw editor automatisch een sluit `</article>` tag heeft toegevoegd, verwijder deze dan.

+ Onderaan het bestand, net **boven** de `</main>` tag, voeg je een nieuwe regel toe en sluit het `article` element:

```html
    </article>
  </main>
```

Je `main` element zou er nu ongeveer zo uit moeten zien (jij hebt mogelijk andere inhoud tussen de `article` tags):

```html
  <main>
    <article>
        <h1>Mijn favoriete plekken om te zien in Ierland</h1>  
          <h2>De kliffen van Moher</h2> 
          <p>
          De kliffen van Moher zijn te vinden in County Clare, waar ik vandaan kom. Kijk hoe cool ze zijn!</p> 
       <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
       <h2>Achill Island</h2> 
        <p>Dit is een groot eiland voor de kust van County Mayo. Je vindt er wild en 
       een mooi landschap van bergen, moerassen en kliffen.
        </p>
        <img src="achill.JPG" width="200px" />
    </article>
  </main>
```

+ Bekijk nu de inhoud in je `artikel` en probeer het op te splitsen in secties. Plaats de volgende nieuwe tags rond elk deel: `<section> </section>`. Hier is een voorbeeld van hoe het eruit zou kunnen zien:

```html
  <article>
    <h1>Mijn favoriete plekken om te zien in Ierland</h1>
    <section>
       <h2>De kliffen van Moher</h2> 
          <p>
          De kliffen van Moher zijn te vinden in County Clare, waar ik vandaan kom. Kijk hoe cool ze zijn!</p> 
      <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
    </section>
     <section>
       <h2>Achill Island</h2> 
        <p>Dit is een groot eiland voor de kust van County Mayo. Je vindt er een wild en mooi landschap van bergen, moerassen en kliffen.
      </p>
      <img src="achill.JPG" width="200px" />
    </section>
  </article>
```

## \--- collapse \---

## title: Waar gaan de nieuwe tags over?

Zie deze nieuwe elementen als **containers**. Ze worden gebruikt om dingen te groeperen (samen te voegen). Het is een beetje alsof je dingen in dozen en op planken bij je thuis organiseert!

Dit maakt je website vriendelijk voor schermlezers, geeft je meer controle over de lay-out (opmaak) en, zoals je zult zien, kun je met de styling echt creatief worden.

Alles kan tussen de tags staan. Meestal zal het meer dan één element zijn, maar dat hoeft niet zo te zijn. Het kunnen allerlei soorten HTML-elementen zijn. Wat je doet, is de browser laten weten dat alles tussen deze tags bij elkaar hoort.

### Article

Het `article`(artikel) element is een container voor een heel stuk inhoud, in dit geval een verzameling informatie over bezienswaardigheden in Nederland. Als je verschillende stukjes inhoud hebt die geen verband met elkaar hebben, moet je elke stuk in een eigen `article` element plaatsen in plaats van de tags rond de gehele inhoud zetten.

### Section

Met het `section` element kunt je verwante inhoud verdelen in kleinere delen en elk deel in een eigen container plaatsen.

### Andere containers bestaan ook nog!

Dit zijn niet de enige container elementen in HTML. Als je ooit een menu hebt gemaakt en vervolgens tussen `<nav> </nav>` tags hebt geplaatst, is dat een ander voorbeeld van een type container. Dat geldt ook voor `<main> </main>` en `<header> </header>` \--- kan jij er nog meer bedenken?

\--- /collapse \---

\--- challenge \---

Je webpagina ziet er misschien nog niet zo anders uit, maar zodra de inhoud is georganiseerd in container tags, kunt je er met CSS leuke dingen mee doen. Onthoud dat HTML bepaalt hoe je website is georganiseerd en CSS bepaalt hoe het eruit ziet.

## Uitdaging: organiseer je website

+ Probeer de inhoud van je website op deze manier met behulp van de `article` en `section` containers te organiseren. 

\--- hints \---

\--- hint \---

Kijk naar de Eten pagina van het voorbeeldproject. Je ziet dat ik een `article` heb toegevoegd met een heleboel `section` tags in het bestand `food.html`:

```html
  <main> 
   <article> 
    <h1> Eten in Ierland </h1> 
    <p>
     Dit zijn enkele van mijn favoriete Ierse gerechten!
      </p>
   <section>
      <h2>Traditioneel Iers ontbijt</h2>
      <p>
        Een "Full Irish" ontbijt bestaat uit worstjes, plakjes (bacon), 
        eieren, bloedworst, worst en toast.
        </p>
         <p> Vaak zijn er een gegrilde tomaat, champignons 
           en gebakken bonen bij.
        </p>
          <p>
            En natuurlijk is geen ontbijt compleet zonder een heerlijke
            pot thee!
        </p>
      </section>

      <section> 
        <h2>Bangers en Mash</h2>
        <p>
          Deze klassieker van worsten, aardappelpuree en jus is niet uniek voor Ierland, maar wat het speciaal maakt, zijn de Ierse worsten. De meeste landen hebben hun eigen manier om worsten te maken, 
         en dit is één ding dat ik mis van thuis als ik op reis ben!
        </p>
      </section>

      <section>
         <h2> Baco and Cabbage </h2> 
         <p>
           Ik zou onmogelijk een lijst met Iers eten kunnen maken zonder dit zeer traditionele gerecht te noemen!
        </p>
      <p>
         Het klinkt misschien niet zo interessant, maar deze hartige maaltijd 'met gekookte ham, aardappelen en groene kool is smakelijk en vullend.
          Ik hou ervan de aardappelen in boter te smoren en ik hou ook van een beetje mosterd bij het spek.
        </p>
        <p>
          Mijn moeder maakt het altijd extra speciaal door de kool 
           in het water te koken waarin de ham is gekookt.
        </p>
        <p>
          Als er nog restjes zijn, kun je nog een van mijn 
          favorieten maken: <strong>fried cabbage</strong> (gefrituurde kool)!
        </p>
      </section>
    </article>     
  </main>
```

\--- /hint \---

\--- /hints \---

Op de volgende kaart ontwerp je een ander thema voor elke pagina die is georganiseerd in artikelen en secties!

\--- /challenge \---