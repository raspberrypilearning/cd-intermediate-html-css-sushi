## Proiectați câteva teme

Scrierea regulilor CSS pentru elemente cum ar fi `secțiunea` și `p` este mare, dar ce dacă doriți să faceți ca unele dintre ele să arate diferit de altele? Pe acest card veți învăța cum să aplicați diferite seturi de reguli de stil elementelor de același tip și să creați o temă diferită pentru fiecare pagină de pe site-ul dvs. web!

+ Du-te la fișierul foaie de stil și adăugați următoarele - asigurați-vă că includeți punct în față!

```css
  .topDivider {stil de frontieră: solid; frontieră-top-lățime: 2px; frontal-culoarea de sus: # F5FFFA; padding-bottom: 10px; }
```

+ Acum du - te la `attractions.html` (sau fișierul HTML care lucrați , dacă utilizați propriul proiect), și se adaugă următoarele **atribut** la fiecare `secțiunea` tag - ul:

```html
  <section class="topDivider">
```

Ar trebui să vedeți o linie care să apară deasupra fiecărei secțiuni din pagină. Felicitări - ai folosit doar prima dvs. **CSS clasa**!

![Pagina cu linii între secțiuni](images/sectionsWithTopBorder.png)

+ Uită-te la modul în care arată pagina dvs. web acum și comparați-l cu celelalte pagini care au `elemente din secțiunea`. Veți vedea că numai acelea în care ați adăugat atributul `class = "topDivider"` vor avea linia de sus.

## \--- colaps \---

## titlu: Cum funcționează?

Amintiți-vă că atunci când utilizați un selector CSS **** cum ar fi `secțiunea` sau `p` sau `nav ul`, regulile de stil se aplică la **toate cele** elemente de tipul respectiv de pe site-ul dvs. Web.

Cu CSS **clasele**, poți schimba stilul de doar **din** elemente.

Punerea unui punct în fața selectorului dvs. o face într-un selector de clasă ****. O clasă poate avea orice nume, deci nu trebuie să fie numele unui element HTML. De exemplu:

```css
  .myAwesomeClass {/ * regulile mele de stil cool merg aici * /}
```

Pentru a alege ce elemente se aplică regulile de stil la, adăugați `clasa` **Atributul** la acele elemente în codul HTML: pune numele clasei în ca valoare pentru atributul, **fără a** punct, astfel:

```html
  class = "myAwesomeClass"
```

\--- / colaps \---

+ Sunteți gata să încercați altă clasă? Adăugați următorul cod CSS la `stiles.css`:

```css
  .stylishBox {background-color: # 87CEFA; culoare: # A52A2A; stilul frontal: solid; lățimea frontală: 2px; culoare frontală: # F5FFFA; raza de graniță: 10 pixeli; }
```

+ Apoi, pe o altă pagină a site-ului dvs., adăugați clasa la unele elemente acolo. O să o adaug pe elementele `secțiunea` pe pagina alimentară a site-ului meu web, după cum urmează: `<section class="stylishBox">`.

Arată grozav, dar acum secțiunile mele sunt toate sparte împreună.

![Secțiuni frumoase înfățișate s-au zdrobit împreună](images/squashedSections.png)

Puteți aplica cât mai multe clase CSS unui element pe care îl doriți. Doar scrieți toate clasele pe care doriți să le utilizați în cadrul atributului `class` (amintiți-vă fără punct!), Separându-le cu spații.

+ Să facem o altă clasă CSS pentru a oferi secțiunilor o marjă și o umplutură. În fișierul `styles.css` , creați următoarea clasă CSS:

```css
  .someSpacing {padding: 10px; margin-top: 20px; }
```

+ În codul dvs. `html` , adăugați noua clasă la fiecare dintre elementele pe care lucrați, cum ar fi:

```html
  <section class="stylishBox someSpacing">
```

![Au fost adăugate secțiuni cu margini și cusături](images/sectionsWithSpacing.png)

Deci , clase CSS vă permit să **alegeți** care elemente de stil, și vă lăsați **reutilizarea** același set de reguli de stil pe orice elemente pe care doriți.

+ Du - te la `index.html` și se adaugă `stylishBox` clasa la `principale` elementul, sau un alt element pe pagină. Îl poți elimina din nou după aceea!

```html
    <main class="stylishBox">   
```

Iată ce arată pagina mea de pornire cu clasa CSS. De asemenea, am adăugat clasa `topDivider` la eticheta `img` cu imaginea lui Tito.

![Clasele CSS sunt utilizate pe pagina de pornire](images/homePageWithClasses.png)

\--- provocare \---

## Provocare: faceți câteva clase noi

+ Utilizați clasele CSS **clase** pentru a defini câteva dimensiuni diferite ale imaginilor pentru site-ul dvs., de exemplu, `imagini mici` și `.mediumPictures`. Apoi, eliminați atributul `lățime` din fiecare dintre elementele `img` și adăugați în schimb clasa corespunzătoare.

\--- sugestii \---

\--- hint \---

Puteți crea o clasă CSS care definește doar lățimea unui element ca acesta:

```css
  .smallPictures {width: 100px; }
```

\--- / indiciu \---

\--- hint \---

Iată un `img` etichetă cu `lățime` atribut:

```html
  <img src="tito.png" alt="Tito the dog" width="100px" />       
```

Când eliminați atributul `lățime` și controlați mărimea cu clasa CSS, arata astfel:

```html
  <img src="tito.png" class="smallPictures" alt="Tito the dog" />       
```

Utilizând o clasă CSS, puteți schimba ușor lățimea tuturor imaginilor simultan, schimbând doar o singură linie de cod în foaia dvs. de stil!

\--- / indiciu \---

\--- / sugestii \---

\--- /provocare \---