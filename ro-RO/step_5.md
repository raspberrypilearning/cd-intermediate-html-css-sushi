## Organizarea paginii dvs.

Până acum ați utilizat **rubricile** și **alineatele** pentru a face dvs. **conținut** aspect ordonat și ușor de citit. Să o facem mai bine organizată prin gruparea lucrurilor.

## \--- colaps \---

## titlu: Ce este conținutul?

**Conținutul** reprezintă toate lucrurile de pe pagina dvs. web, cum ar fi text și imagini.

\--- / colaps \---

+ Mergeți la `attractions.html` fișier (sau una din paginile proprii dacă nu utilizați exemplul de proiect) și, în partea de sus, doar **sub** eticheta de deschidere `<main>` , tastați următoarele pe o linie nouă : 

```html
  <main>
    <article>
```

+ Dacă editorul dvs. a adăugat automat într-o etichetă de închidere `</article>` pentru dvs., ștergeți-l.

+ În partea de jos a fișierului, doar **de mai sus** închidere `</main>` tag - ul, adăugați o nouă linie și închideți `articolul` elemente:

```html
    </article>
  </main>
```

Elementul principal `elementul dvs.` ar trebui să arate așa ceva acum (este posibil să aveți un conținut diferit între cele `etichete din articolul` desigur):

```html
  <main>
    <article>
      <h1>Locurile mele preferate de vizitat în Irlanda</h1>
        <h2>Stâncile din Moher</h2>
        <p>
        Stâncile din Moher se găsesc în județul Clare, de unde sunt. Uită-te cât de cool sunt!</p>
        <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
        <h2>Achill Island</h2>
        <p>Aceasta este o insula mare de pe coasta județului Mayo. Are un peisaj sălbatic și frumos de munți, mlaștini și stânci.
        </p>
        <img src="achill.JPG" width="200px" />
    </article>
  </main>
```

+ Acum , uita - te la conținutul dvs. `articolul` și să încerce să - l rupe în secțiuni. Puneți această nouă pereche de etichete în jurul fiecărui bit: `<section> </section>`. Iată un exemplu despre cum ar putea să arate:

```html
  <article>
    <h1>Locurile mele preferate de vizitat în Irlanda</h1>
    <section>
      <h2>Stâncile din Moher</h2>
      <p>
      Stâncile din Moher se găsesc în județul Clare, de unde sunt. Uită-te cât de cool sunt!</p>
      <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
    </section>
    <section>
      <h2>Achill Island</h2>
      <p>Aceasta este o insula mare de pe coasta județului Mayo. Are un peisaj sălbatic și frumos de munți, mlaștini și stânci.
      </p>
      <img src="achill.JPG" width="200px" />
    </section>
  </article>
```

## \--- colaps \---

## titlu: Care sunt toate etichetele noi?

Gândiți-vă la aceste noi elemente ca **containere**. Ele sunt folosite pentru a grupa lucrurile impreuna. E un pic cam cum ai organiza lucrurile în cutii și rafturi în casa ta!

Acest lucru face site-ul dvs. prietenos pentru cititorii de ecran, vă oferă mai mult control asupra aspectului și, după cum veți vedea, vă permite să deveniți cu adevărat creativi cu stilul.

Orice poate intra între etichete. De obicei, va fi mai mult decât un element, dar nu trebuie să fie. Ele pot fi elemente HTML de orice fel. Ceea ce faceți este să spuneți browser-ului că totul între aceste etichete aparține împreună.

### Articol

Elementul de `articolul` este un container pentru o întreagă bucată de conținut, în acest caz un set de informații despre atracțiile din Irlanda. Dacă aveți biți diferiți de conținut care nu sunt corelați, ar trebui să puneți fiecare în propriul element `articol` în loc să puneți un set de etichete în jurul întregului lot.

### Secțiune

Elementul `secțiunea` vă permite să împărțiți conținutul asociat în bucăți mai mici și să puneți fiecare bucată în containerul propriu.

### Altele exista prea!

Acestea nu sunt singurele elemente de container din HTML. Dacă ați creat vreodată un meniu și apoi l-ați pus între `<nav> </nav>` tag-uri, acesta este un alt exemplu de tip de container. Deci sunt `<main> </main>` si `<header> </header>` - te poti gandi mai mult?

\--- / colaps \---

\--- provocare \---

Este posibil ca pagina dvs. Web să nu arate altfel, dar odată ce conținutul a fost organizat în etichete de container, veți putea să faceți niște lucruri interesante cu CSS. Rețineți că HTML controlează modul în care site-ul dvs. este organizat și CSS controlează cum arată.

## Provocare: organizați-vă site-ul web

+ Deplasați-vă la organizarea întregului conținut de pe site-ul dvs. folosind containerele `articolul` și `secțiunea` în acest fel. 

\--- sugestii \---

\--- hint \---

Uită-te la pagina de alimentare a proiectului de exemplu. Vei vedea că am adăugat un `articol` , cu un buchet de `secțiunea` tag - uri în fișierul `food.html`:

```html
  <main>
    <article>
      <h1>Alimente în Irlanda</h1>
      <p>
        Acestea sunt câteva din mâncurile mele preferate irlandeze!
      </p>  
      <section>
        <h2>Mic dejun tradițional irlandez</h2>
        <p>
          Un mic dejun complet irlandez este format din cârnați, rashers (șuncă), ouă, budincă neagră, budincă albă și pâine prăjită.
        </p>
        <p>
          Deseori va exista o roșii la grătar, ciuperci și fasole coapte.
        </p>
        <p>
          Și, bineînțeles, nici un mic dejun nu este complet fără o ceașcă de ceai!
        </p>
      </section>

      <section>
        <h2>Bangers și Mash</h2>
        <p>
          Acest clasic de cârnați, cartofi piure și sos nu este unic pentru Irlanda, dar ceea ce îl face deosebit este mezelurile irlandeze. Majoritatea țărilor au propriul mod de a face cârnați și sunt un lucru pe care mi-l lipsește de acasă dacă sunt departe de călătorie!
        </p>
      </section>

      <section>
        <h2>Bacon și varză</h2>
        <p>
          Nu puteam să fac o listă cu mâncarea irlandeză fără a include această fel de mâncare foarte tradițională!
        </p>
        <p>
          Este posibil să nu sune foarte interesant, dar această masă consistentă de șuncă fiartă, cartofi și varză verde este gustoasă și umplutătoare.
          Îmi place să împușc cartofii în unt și îmi place și puțin mustar cu șuncă.
        </p>
        <p>
          Mama mea a făcut întotdeauna ceva deosebit prin gătitul varzei în apa în care a fost lăsată șuncă.
        </p>
        <p>
          Dacă există resturi puteți face unul dintre favoritele mele: <strong>varză prăjită</strong>!
        </p>
      </section>
    </article>     
  </main>
```

\--- / indiciu \---

\--- / sugestii \---

Pe următoarea carte, veți crea o temă diferită pentru fiecare pagină care este organizată în articole și secțiuni!

\--- /provocare \---