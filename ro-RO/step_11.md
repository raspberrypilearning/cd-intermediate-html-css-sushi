## Învățați-l pe Tito să se răcească!

Puteți face site-ul dvs. mai mult **interactiv** făcând lucruri interesante să se întâmple atunci când treceți peste lucrurile cu cursorul mouse-ului!

+ Găsiți regulile CSS pentru elementele `img` sau creați unele dacă nu aveți niciun element. Adăugați o margine și apoi adăugați un nou bloc de reguli chiar mai jos:

```css
  img {border: 2px solid alb; } img: hover {frontieră: 2px marcat cu Navy; }
```

Tocmai ați folosit un tip special de bloc CSS numit **pseudo-clasa**.

## \--- colaps \---

## titlu: Cum funcționează?

O **pseudo-clasa** este un pic diferit de **clasa** pe care le creați singur. O puteți recunoaște cu `:`.

Pseudo-clasele sunt construite în elementele HTML: puteți adăuga `: hover` rules style la orice element, clasă sau `id` selector în foaia dvs. de stil fără a fi nevoie să adăugați nimic suplimentar în codul HTML.

\--- / colaps \---

+ Ce crezi ca se va intampla? Verificați ce pagini de pe site-ul dvs. au imagini pe ele (adăugați o imagine dacă nu există!), Apoi mutați cursorul peste o imagine pentru a afla!

+ Să folosim acest nou `: hover` pseudo-clasă, împreună cu o clasă CSS pentru a face legături stralucitoare atunci când hover peste ele! Adăugați un link către pagina dvs. web și includeți un atribut pentru a specifica numele clasei. Amintiți-vă că legăturile sunt definite folosind eticheta `<a>` , astfel:

```html
    <p>
      Vizitați pagina <a class="niceLinks" href="https://en.wikipedia.org/wiki/Ireland">Wikipedia</a> pentru a afla mai multe despre Irlanda!
    </p>
```

+ Adăugați următorul cod în foaia dvs. de stil, apoi executați codul pentru a vedea legăturile minunate în acțiune.

```css
  .niceLinks {text-decoration: none; culoare: # FFFAF0; } .niceLinks: hover {culoare: # 00FF7F; }
```

+ De ce nu adăugați atributul `class = "niceLinks"` la toate linkurile din bara de meniu, de asemenea?

Puteți combina toate aceste trucuri cu animații prea!

+ Găsiți din nou blocul CSS pentru fotografia lui Tito (sau orice imagine pe care ați lucrat mai devreme). Adăugați următorul cod în fișierul cu foi de stil:

```css
  #titoPicture {limita-raza: 100%; lățime: 100px; } #titoPicture: mutați {animation-name: rollOver; durata animației: 1s; animație-iterație-număr: 1; } @frame de chei rollOver {0% {transform: rotate (0deg); } 100% {transform: rotate (-360deg); }}
```

+ Poti ghici ce se va intampla?

+ Acum striga "Rotiți-vă!" în timp ce mutați cursorul peste imagine!

\--- provocare \---

## Provocare: faceți legături strălucitoare de curcubeu

+ Puteți utiliza animația `rainbowGlow` de pe cardul anterior pentru a face legăturile din meniu să schimbe culorile atunci când cursorul se află peste acestea?

\--- sugestii \---

\--- hint \---

Mai jos este codul pentru `rainbowGlow` animația. Are cinci etape definite și stabilește o altă culoare a textului în fiecare etapă. Puteți să adăugați mai multe sau să le schimbați oricum doriți!

```css
    @ cadre cheie rainbowGlow {0% {culoare: # 00BFFF; } 25% {culoare: # 00FF7F; } 50% {culoare: #eeeeaf; } 75% {culoare: #eeafee; } 100% {culoare: # 00BFFF; }}
```

\--- / indiciu \---

\--- hint \---

Pentru a anima ceva, adăugați cele trei proprietăți `animație` la regulile de stil, așa cum ați procedat mai sus. Întotdeauna asigurați - vă că `animație nume-` se potrivește cu numele de animație pe care doriți să îl utilizați.

\--- / indiciu \---

\--- hint \---

Puteți adăuga `efecte de hover` direct în meniul `nav` astfel:

```css
  nav ul li a: hover {animație-nume: rainbowGlow; durata animației: 1,5 s; animație-iterație-count: infinit; }
```

Sau, dacă doriți să faceți alte link - uri pe culorile curcubeului flash site - ul le puteți adăuga animația la `.niceLinks` clasă în schimb, ca aceasta:

```css
  .niceLinks: hover {culoare: # 00BFFF; animație-nume: rainbowGlow; durata animației: 1,5 s; animație-iterație-count: infinit; }
```

\--- / indiciu \---

\--- / sugestii \---

\--- /provocare \---

![](images/badge-footer-image-html-intermed.png)