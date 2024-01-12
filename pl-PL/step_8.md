## Automatyczne dopasowanie rozmiarów

Do tej pory używałeś **pikseli** aby ustawić rozmiar rzeczy, np. `10px`. Na tej karcie poznasz inne pomiary, których możesz użyć.

+ Przejdź do `index.html` i znajdź element `img` z obrazem Tito, lub znajdź inny tag `img` na swojej stronie.

+ Usuń atrybut `width` jeśli jest tam i nadaj temu elementowi `id` jeśli go jeszcze nie posiada.

```html
  <img src="tito.png" id="titoPicture" alt="Tito the dog" />
```

+ W pliku CSS zdefiniuj właściwość `width` (szerokość) dla swojego obrazu, jak pokazano poniżej (może być konieczne utworzenie bloku CSS z selektorem `id`, jeśli jeszcze tego nie zrobiłeś na poprzedniej karcie).

```css
  #titoPicture {
    width: 50%;
    border-radius: 100%;
  }
```

Uwaga: 50% (50 procent) to **połowa**.

+ Spróbuj zmienić rozmiar okna przeglądarki i obserwuj, co dzieje się z obrazem.

Powinieneś zobaczyć, że obraz staje się większy i mniejszy, gdy powiększasz i zmniejszasz okno. Dzieje się tak, ponieważ zajmuje 50% szerokości elementu **main** (który jest w przybliżeniu szerokością strony).

--- collapse ---
---
title: Jak to działa?
---

Kiedy ustawiasz rozmiar czegoś w pikselach, ustawiasz dokładny rozmiar i to się nie zmienia. Jest to wymiar **bezwzględny**.

Innym sposobem na ustawienie rozmiaru rzeczy jest użycie **względnych** pomiarów, więc rozmiar zależy od tego, jak duże elementy są porównywane ze sobą. Następnie, gdy jedna rzecz zmieni rozmiar, wszystkie inne zmiany również automatycznie zmienią rozmiar, aby zachować te same **proporcje**.

Gdy używasz **względnych** pomiarów, ważne jest, aby wiedzieć, jaki jest **element nadrzędny** twojego elementu. Element nadrzędny jest tym, w czym znajduje się twój element i do tego zmierza pomiar. Na przykład elementem nadrzędnym powyższego obrazu jest element `article`, ponieważ element `img` znajduje się pomiędzy tagami `<article></article>`.

SzerokośćJeśli ustawisz `width`(szerokość) elementu na `100%`, to sprawi, że będzie to taka sama szerokość jak kontener nadrzędny.

--- /collapse ---

+ Eksperymentuj z różnymi liczbami przed `%`.