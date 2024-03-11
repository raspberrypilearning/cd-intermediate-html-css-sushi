## Zadanie: naucz Tito turlać się!

Możesz uczynić swoją stronę bardziej **interaktywną** powodując, że fajne rzeczy dzieją się, gdy najedziesz kursorem myszy na rzeczy!

+ Znajdź swoje reguły CSS dla elementów `img` lub utwórz jakieś jeśli nie masz żadnych elementów. Dodaj obramowanie, a następnie dodaj nowy blok reguł bezpośrednio poniżej:

```css
  img {
    border: 2px solid White;
  }
  img:hover {
    border: 2px dashed Navy;
  }
```

Właśnie użyłeś specjalnego typu bloku CSS o nazwie **pseudo-class**(pseudo klasa).

--- collapse ---
---
title: Jak to działa?
---

**pseudo-klasa** różni się nieco od **klasy**, którą tworzysz. Możesz to rozpoznać przez `:`.

Pseudoklasy zostały wbudowane w elementy HTML: możesz dodać `:hover` reguły stylu do dowolnego elementu, klasy, lub selektora `id` w arkuszu stylów bez konieczności dodawania czegokolwiek dodatkowego do kodu HTML.

--- /collapse ---

+ Jak myślisz, co się stanie? Sprawdź, które strony w Twojej witrynie zawierają zdjęcia (dodaj zdjęcie, jeśli ich nie ma!), A następnie przesuń kursor nad zdjęciem, aby się dowiedzieć!

+ Użyjmy tej nowej pseudoklasy `:hover` razem z klasą CSS, aby sprawić, że linki się świeciły po najechaniu na nie kursorem! Dodaj link do swojej strony internetowej i dołącz atrybut określający nazwę klasy. Pamiętaj, linki są zdefiniowane za pomocą tagu `<a>`, jak tak:

```html
    <p>
      Odwiedź <a class="niceLinks" href="https://en.wikipedia.org/wiki/Ireland">stronę Wikipedia</a>, aby dowiedzieć się więcej o Irlandii!
    </p>
```

+ Dodaj następujący kod do arkusza stylów, a następnie uruchom kod, aby zobaczyć swoje piękne linki w akcji.

```css
  .niceLinks {
    text-decoration: none;
    color: #FFFAF0;
  }
  .niceLinks:hover {
    color: #00FF7F;
  }
```

+ Dlaczego nie dodać atrybutu `class="niceLinks"` do wszystkich linków w pasku menu?

Możesz również połączyć wszystkie te sztuczki z animacjami!

+ Znajdź ponownie blok CSS dla zdjęcia Tito (lub dowolny obrazek nad którym pracowałeś wcześniej). Dodaj następujący kod do pliku arkusza stylów:

```css
  #titoPicture {
    border-radius: 100%;
    width: 100px;
  }
  #titoPicture:hover {
    animation-name: rollOver;
    animation-duration: 1s;
    animation-iteration-count: 1;
  }
  @keyframes rollOver {
    0% {
      transform: rotate(0deg);
    }
    100% {
      transform: rotate(-360deg);
    }
  }
```

+ Czy potrafisz zgadnąć, co się stanie?

+ Teraz krzycz „Przewróć się!” gdy przesuwasz kursor nad zdjęciem!

--- challenge ---

## Wyzwanie: wykonaj świecące tęczowe linki

+ Czy możesz użyć animacji `RinbowGlow` z poprzedniej karty, aby linki w menu nadal zmieniały kolory, gdy kursor nad nimi znajduje się nad nimi?

--- hints ---

--- hint ---

Poniżej znajduje się kod dla animacji `rainbowGlow`. Ma pięć zdefiniowanych etapów i ustawia inny kolor tekstu na każdym etapie. Możesz dodać więcej lub zmienić je, jak chcesz!

```css
    @keyframes rainbowGlow {
        0% {
            color: #00BFFF;
        }
        25% {
            color: #00FF7F;
        }
        50% {
            color: #eeeeaf;
        }
        75% {
            color: #eeafee;
        }
        100% {
            color: #00BFFF;
        }
    }
```

--- /hint ---

--- hint ---

Aby coś animować, dodajesz trzy właściwości `animation` do jego reguł stylu, tak jak to zrobiłeś powyżej. Zawsze upewnij się, że `animation-name` pasuje do nazwy animacji, której chcesz użyć.

--- /hint ---

--- hint ---

Możesz dodać efekty `hover` bezpośrednio do menu `nav`:

```css
  nav ul li a:hover {
    animation-name: rainbowGlow;
    animation-duration: 1.5s;
    animation-iteration-count: infinite;
  }
```

Albo, jeśli chcesz również spowodować, żeby inne linki na swojej stronie internetowej świeciły kolorami tęczy, możesz zamiast tego dodać animację do klasy `.niceLinks` w następujący sposób:

```css
  .niceLinks:hover {
    color: #00BFFF;
    animation-name: rainbowGlow;
    animation-duration: 1.5s;
    animation-iteration-count: infinite;
  }
```

--- /hint ---

--- /hints ---

--- /challenge ---

![](images/badge-footer-image-html-intermed.png)

***

Ten projekt został przetłumaczony przez wolontariuszy:

Marek Lubinski
Paweł Wilk
Sylwia Łuczak-Jagieła

Dzięki wolontariuszom możemy dać ludziom na całym świecie szansę nauki w ich własnym języku. Możesz pomóc nam dotrzeć do większej liczby osób, zgłaszając się na ochotnika do tłumaczenia - więcej informacji na stronie [rpf.io/translate](https://rpf.io/translate).
