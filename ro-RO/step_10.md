## Animaţie

Știați că puteți folosi CSS pentru a face lucrurile să se deplaseze? Veți învăța cum se face pe acest card!

+ Înainte de a începe, asigurați - vă că aveți o imagine de pe site - ul dvs. cu un `id` și un bloc CSS corespunzător care stabilește `lățime de` To `100px`. Merg acum cu fotografia lui Tito și blocul meu CSS arată astfel:

```css
    #titoPicture {limita-raza: 100%; lățime: 100px; }
```

+ Mergeți în partea de jos a fișierului dvs. CSS și adăugați următorul cod:

```css
    @frame-cheie myFirstAnimation {din {width: 100px; } la {width: 300px; }}
```

Acest cod creează o animație numită `myFirstAnimation` care o puteți adăuga la orice element de pe site-ul dvs. Web. Ce credeți că va face?

+ Găsiți regulile CSS pentru imagine și adăugați următoarele trei proprietăți:

```css
    animație-nume: myFirstAnimation; durata animației: 2s; animație-iterație-număr: 1;
```

+ Acum urmăriți ce se întâmplă pe pagina dvs. web! Încercați diferite valori pentru `animație-iterație-număr` pentru a vedea ce face.

+ Să încercăm o altă animație! Adăugați următorul cod la sfârșitul fișierului dvs. CSS:

```css
    @ cadre cheie rainbowGlow {0% {culoare: # FFD700; } 50% {culoare: # 663399; } 100% {culoare: # FFD700; }}
```

+ Acum găsi `#myCoolText` regulile CSS de mai devreme și se adaugă în codul de animație:

```css
    #myCoolText {culoare: # 003366; frontieră: 2px creasta #ccffff; padding: 15px; text-align: centru; animație-nume: rainbowGlow; durata animației: 1,5 s; animație-iterație-număr: 1; }
```

Când utilizați **valori procentuale** în loc de `la` și `până la`, puteți seta valorile între valori, precum și doar valori de început și de sfârșit. Puteți seta cât mai multe valori între valorile dorite utilizând valori procentuale diferite de la `0` până la `100`.

+ Modificați valoarea `animație-iterație-număr` la `infinit`. Vedeți dacă puteți ghici ce se va întâmpla înainte de al testa!

+ Încercați diferite valori pentru `animație - durata` pentru a accelera sau încetini animația.

+ Un truc final! Adăugați acest cod de animație:

```css
    @ slideframe cheie {0% {background-position-x: 0; } 100% {background-position-x: 600vw; }}
```

+ Acum găsiți regulile `#frontPage` CSS pe care le-ați scris mai devreme și le schimbați la:

```css
    #frontPage {fundal: gradient liniar repetat (-45deg, roșu 0%, galben 7,14%, var 14,28%, cyan 21,42%, cyan 28,56%, albastru 35,7%, magenta 42,84%, roșu 50%); dimensiunea fundalului: 600vw 600vw; animație: diapozitiv 10s infinit liniar înainte; }
```

Nu vă faceți griji cu privire la înțelegerea întregului cod de mai sus ... doar stai înapoi și bucurați-vă!

Pentru a afla mai multe despre mai multe lucruri pe care le puteți face cu animație, accesați [această pagină web](http://dojo.soy/html2-css-animation){: target = „_ blank“}. A se distra!

Pe următoarea carte veți învăța cum să faceți lucruri reci se întâmplă atunci când plasați cursorul mouse-ului peste lucruri!