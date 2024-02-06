## Organizowanie twojej strony

Do tej pory używałeś **nagłówków** i **akapitów** aby **zawartość** Twojej strony wyglądała dobrze i była łatwo czytelna. Zorganizujmy ją jeszcze lepiej, grupując niektóre elementy razem.

## \--- collapse \---

## title: Co to jest zawartość strony?

**Zawartość** to wszystko to, cp zawiera strona, na przykład tekst i grafika.

\--- /collapse \---

+ Przejdź do pliku `attractions.html` (lub jednej ze swoich stron, jeśli nie korzystasz z przykładowego projektu). Na górze, **poniżej** `<main>`, wpisz w nowym wierszu: 

```html
  <main>
    <article>
```

+ Jeśli edytor dodał automatycznie znacznik zamykający `</article>`, usuń go.

+ Na dole pliku, tuż **powyżej** zamykającego znacznika `</main>`, dodaj nowy wiersz i zamknij element `article`:

```html
    </article>
  </main>
```

Twój element `main` powinien wyglądać jak poniżej (możesz mieć oczywiście inną zawartość między tagami `article`):

```html
  <main>
    <article>
      <h1>Moje ulubione miejsca do zwiedzenia w Irlandii</h1>
        <h2>Klify Moher</h2>
        <p>
        Klify Moher znajdują się w hrabstwie Clare, skąd pochodzę. Zobacz, jakie są fajne!</p>
        <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
        <h2>Wyspa Achill</h2>
        <p>
        Jest to duża wyspa u wybrzeży hrabstwa Mayo. Ma dziki i
        piękny krajobraz gór, torfowisk i klifów.
        </p>
        <img src="achill.JPG" width="200px" />
    </article>
  </main>
```

+ Teraz spójrz na zawartość swojego artykułu `article` i spróbuj rozbić ją na sekcje. Umieść nową parę tagów wokół każdego fragmentu: `<section> </section>`. Na przykład może to wyglądać w ten sposób:

```html
  <article>
    <h1>Moje ulubione miejsca do zwiedzania w Irlandii</h1>
    <section>
      <h2>Klify Moher</h2>
      <p>
      Klify Moher znajdują się w hrabstwie Clare, skąd pochodzę. Zobacz, jakie są fajne!</p>
      <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
    </section>
    <section>
      <h2>Wyspa Achill</h2>
      <p>
      Jest to duża wyspa u wybrzeży hrabstwa Mayo. Ma dziki i
      piękny krajobraz gór, torfowisk i klifów.
      </p>
      <img src="achill.JPG" width="200px" />
    </section>
  </article>
```

## \--- collapse \---

## title: Na czym polegają te nowe tagi?

Pomyśl o tych nowych tagach jak o **kontenerach**. Służą do grupowania rzeczy razem. To trochę jak porządkowanie rzeczy w pudełkach i na półkach w domu!

Dzięki nim Twoja strona jest przyjazna dla czytników ekranu, daje większą kontrolę nad układem i, jak zobaczysz, pozwala na kreatywną stylizację zawartości.

Między tymi tagami może znajdować się wszystko. Zwykle będzie to więcej niż jeden element, chociaż nie musi tak być. Mogą to być dowolne elementy HTML. W ten sposób mówisz przeglądarce, że wszystko między tymi tagami jest ze sobą powiązane.

### Article

Element `article` jest kontenerem dla całej treści, w tym przypadku jest to zestaw informacji o atrakcjach w Irlandii. Jeżeli masz różne fragmenty zawartości, które nie są ze sobą powiązane, każdy z nich powinien znajdować się w swoim własnym tagu `article`, zamiast umieszczania jednego zestawu tagów dla całej zawartości.

### Sekcja

Element `section` pozwala podzielić zawartość na mniejsze fragmenty i umieścić każdy fragment we własnym pojemniku.

### Istnieją też inne!

To nie są jedyne kontenery w HTML. Jeśli kiedykolwiek utworzyłeś menu, a następnie umieściłeś je między tagami `<nav> </nav>`, jest to kolejny przykład rodzaju kontenera. Podobnie jest z tagami `<main> </main>` i `<header> </header>` - czy znasz jakieś inne przykłady?

\--- /collapse \---

\--- challenge \---

Twoja strona jeszcze nie wygląda inaczej, ale gdy zawartość zostanie zorganizowana w tagach pojemników, będziesz mógł zrobić z nią kilka fajnych rzeczy za pomocą CSS. Pamiętaj, że HTML określa sposób organizacji Twojej strony, a CSS określa jej wygląd.

## Wyzwanie: zorganizuj swoją stronę internetową

+ Spróbuj zorganizować całą zawartość swojej strony za pomocą tagów artykułu `article` i sekcji `section` w ten sposób. 

\--- hints \---

\--- hint \---

Spójrz na stronę Jedzenie w przykładowym projekcie. Zobaczysz, że dodałem tag `article` z kilkoma tagami `section` do pliku `food.html`:

```html
  <main>
    <article>
      <h1> Jedzenie w Irlandii </h1>
      <p>
        Oto niektóre z moich ulubionych irlandzkich potraw!
      </p>  
      <section>
        <h2> Tradycyjne śniadanie irlandzkie </h2>
        <p>
          „Pełne irlandzkie” śniadanie składa się z kiełbas, boczku (bekonu),
          jajek, czarnego puddingu, białego puddingu i tostów.
        </p>
        <p>
          Często będzie też grillowany pomidor, a także grzyby
          i pieczona fasolka.
        </p>
        <p>
          I oczywiście żadne śniadanie nie jest kompletne bez czajniczka ulubionej 
          herbaty!
        </p>
      </section>

      <section>
        <h2> Bangers i Mash </h2>
        <p>
          Ten klasyk z kiełbasy, puree ziemniaczanego i sosu można znaleźć nie tylko
          w Irlandii, ale to, co czyni go wyjątkowym, to irlandzkie
          kiełbaski. Większość krajów ma swój własny sposób robienia kiełbas.
          To jedna z rzeczy, za którymi tęsknię, kiedy jestem w podróży!
        </p>
      </section>

      <section>
        <h2> Kapusta z boczkiem </h2>
        <p>
          Nie mógłbym zrobić listy irlandzkich potraw bez
          tej bardzo tradycyjnej potrawy!
        </p>
        <p>
          Może to nie brzmieć zbyt interesująco, ale ten posiłek z
          gotowanej szynki, ziemniaków i zielonej kapusty jest smaczny i wypełniający.
          Uwielbiam dusić ziemniaki na maśle, a także dodać
          trochę musztardy do boczku.
        </p>
        <p>
          Moja mama zawsze robiła ją wyjątkowo, gotując kapustę w
          wodzie, w której gotowana była szynka.
        </p>
        <p>
          Jeśli coś zostanie, możesz zrobić jeszcze jedną z moich
          ulubionych potraw: <strong>zasmażaną kapustę</strong>!
        </p>
      </section>
    </article>     
  </main>
```

\--- /hint \---

\--- /hints \---

Na następnej karcie zaprojektujesz inny motyw dla każdej strony podzielonej na artykuły i sekcje!

\--- /challenge \---