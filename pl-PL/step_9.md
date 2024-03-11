## Animacje

Czy wiesz, że możesz użyć CSS, aby wszystko się poruszało? Dowiesz się, jak na tej karcie!

+ Zanim zaczniesz, upewnij się, że masz zdjęcie na swojej stronie z `id` i odpowiednim blokiem kodu CSS, który ustawia `width` na `100px`. Wykorzystam zdjęcie Tito z poprzedniej wersji, a mój blok CSS wygląda tak:

```css
    #titoPicture {
        border-radius: 100%;
        width: 100px;
    }
```

+ Przejdź do dołu pliku CSS i dodaj następujący kod:

```css
    @keyframes myFirstAnimation {
        from {
            width: 100px;
        }
        to {
            width: 300px;
        }
    }
```

Ten kod tworzy animację o nazwie `myFirstAnimation` którą możesz dodać do dowolnego elementu na swojej stronie. Jak myślisz, co to zrobi?

+ Znajdź swoje reguły CSS dla obrazu i dodaj następujące trzy właściwości:

```css
    animation-name: myFirstAnimation;
    animation-duration: 2s;
    animation-iteration-count: 1;
```

+ Zobacz teraz, co dzieje się na twojej stronie internetowej! Wypróbuj różne wartości dla `animation-iteration-count` aby zobaczyć co to robi.

+ Spróbujmy kolejnej animacji! Dodaj następujący kod na końcu pliku CSS:

```css
    @keyframes rainbowGlow {
        0% {
            color: #FFD700;
        }
        50% {
            color: #663399;
        }
        100% {
            color: #FFD700;
        }
    }
```

+ Teraz znajdź reguły CSS `#myCoolText` z wcześniejszych wersji i dodaj kod animacji:

```css
    #myCoolText {        
        color: #003366;
        border: 2px ridge #ccffff;
        padding: 15px;
        text-align: center;
        animation-name: rainbowGlow;
        animation-duration: 1.5s;
        animation-iteration-count: 1;
    }
```

Gdy używasz **wartości procentowe** zamiast `z` i `do`, możesz ustawić wartości zarówno pomiędzy wartościami, jak i tylko wartości początkowe i końcowe. Możesz ustawić tyle wartości pomiędzy wartościami, ile chcesz, używając różnych wartości procentowych z `0` aż do `100`.

+ Zmień wartość `animation-iteration-count` na `infinite`. Zobacz, czy możesz zgadnąć, co się stanie, zanim go przetestujesz!

+ Wypróbuj różne wartości przez `animation-duration` aby przyspieszyć lub spowolnić animację.

+ Ostatnia sztuczka! Dodaj ten kod animacji:

```css
    @keyframes slide {
        0% {
            background-position-x: 0;
        }
        100% {
            background-position-x: 600vw;
        }
    }
```

+ Teraz znajdź zasady CSS `#frontPage`, które napisałeś wcześniej, i zmień je na:

```css
    #frontPage {
        background: repeating-linear-gradient(-45deg, red 0%, yellow 7.14%, lime 14.28%, cyan 21.42%, cyan 28.56%, blue 35.7%, magenta 42.84%, red 50%);
        background-size: 600vw 600vw;
        animation: slide 10s infinite linear forwards;
    }
```

Nie martw się o zrozumienie całego kodu powyżej... po prostu usiądź i ciesz się!!

Aby dowiedzieć się więcej rzeczy możesz zrobić z animacją, odwiedź [tę stronę internetową](http://dojo.soy/html2-css-animation){:target="_blank"}. Miłej zabawy!

Na następnej karcie nauczysz się, jak robić fajne rzeczy, gdy najedziesz kursorem myszy na rzeczy!