## Reglați automat dimensiunea

Până acum utilizați **pixeli** pentru a seta dimensiunea lucrurilor, de exemplu, `<strong> pixeli`. Pe acest card veți afla despre alte măsurători pe care le puteți utiliza.

+ Mergeți la `index.html` și găsiți elementul `img` cu imaginea lui Tito sau găsiți o altă etichetă de `img` pe site-ul dvs. web.

+ Ștergeți atributul `lățime` dacă este acolo și dați elementului un `id` dacă acesta nu are deja unul.

```html
  <img src="tito.png" id="titoPicture" alt="Tito the dog" />
```

+ În fișierul dvs. CSS, definiți proprietatea `lățimea` după cum se arată mai jos (poate fi necesar să creați blocul CSS cu selectorul `id` dacă nu ați făcut deja acest lucru pe o carte anterioară).

```css
  #titoPicture {lățime: 50%; raza de raza: 100%; }
```

Notă: 50% (50%) este **jumătate**.

+ Încercați să redimensionați fereastra browserului dvs. și urmăriți ce se întâmplă cu imaginea.

Ar trebui să observați că imaginea devine mai mare și mai mică atunci când faceți fereastra mai mare și mai mică. Aceasta deoarece ocupa mult de 50% din lățimea **principale** element (care este aproximativ lățimea paginii).

## \--- colaps \---

## titlu: Cum funcționează?

Când setați dimensiunea unui element în pixeli, setați o dimensiune exactă și nu se modifică. Aceasta se numește un **absolut** măsurătoare.

O altă modalitate de a seta dimensiunea lucrurilor este folosirea a **măsurători relative** , astfel încât dimensiunea să depindă de modul în care elementele mari sunt comparate unul cu celălalt. Apoi, ori de câte ori un lucru schimbă mărimea, totul se va schimba automat dimensiunea cât și pentru a menține aceleași **proporții**.

Când utilizați **măsurători relative** , este important să știți care sunt cele **părinte** ale elementului dvs. Parintele este elementul în care este elementul dvs. în interiorul lui și măsura va fi în legătură cu acesta. De exemplu, părintele imaginii de mai sus este elementul `articol` , deoarece elementul `img` se află între etichetele `<article></article>`.

Dacă setați `lățimea` a unui element la `100%`, care va face să aibă aceeași lățime ca și containerul părinte este în.

\--- / colaps \---

+ Experimentați cu numere diferite în fața a `%`.