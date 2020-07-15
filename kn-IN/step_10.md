## ಉರುಳಲು ಟಿಟೊ(Tito) ಗೆ ಕಲಿಸಿ!

ಮೌಸ್ ಕರ್ಸರ್(mouse cursor) ಜೊತೆಗೆ ನೀವು ಸುಳಿದಾಡುತ್ತಿರುವಾಗ ಸುಂದರ ಸಂಗತಿಗಳನ್ನು ಮಾಡುವುದರ ಮೂಲಕ ನೀವು ನಿಮ್ಮ ವೆಬ್ಸೈಟ್ ಅನ್ನು ಹೆಚ್ಚು **interactive** ಆಗಿ ಮಾಡಬಹುದು!

+ `img` ಅಂಶಗಳಿಗಾಗಿ ನಿಮ್ಮ CSS ನಿಯಮಗಳನ್ನು ಹುಡುಕಿ, ಅಥವಾ ನಿಮ್ಮಲ್ಲಿ ಯಾವುದೂ ಇಲ್ಲದಿದ್ದರೆ ಕೆಲವನ್ನು ರಚಿಸಿ. ಗಡಿಯಲ್ಲಿ ಸೇರಿಸಿ, ತದನಂತರ ಹೊಸ ನಿಯಮಗಳ ಬ್ಲಾಕ್ ಅನ್ನು ಕೆಳಗೆ ಸೇರಿಸಿ:

```css
  img {
    border: 2px solid White;
  }
  img:hover {
    border: 2px dashed Navy;
  }
```

ನೀವು **pseudo-class** ಎಂಬ ವಿಶೇಷ ರೀತಿಯ CSS ಬ್ಲಾಕ್ ಅನ್ನು ಬಳಸಿದ್ದೀರಿ.

## \--- collapse \---

## title: ಇದು ಹೇಗೆ ಕೆಲಸ ಮಾಡುತ್ತದೆ?

ನೀವು ರಚಿಸಿರುವ **class** ಗಿಂತ **pseudo-class** ಭಿನ್ನವಾಗಿದೆ. ನೀವು ಇದನ್ನು ಈ ರೀತಿ ಗುರುತಿಸಬಹುದು `:`.

Pseudo-class ಗಳು HTML ಅಂಶಗಳಿಗೆ ನಿರ್ಮಿಸಲ್ಪಟ್ಟಿದೆ: ನಿಮ್ಮ HTML ಕೋಡ್ ಗೆ ಹೆಚ್ಚುವರಿಯಾಗಿ ಏನೂ ಸೇರಿಸದೆ, ನಿಮ್ಮ style sheet ನಲ್ಲಿ ಯಾವುದೇ element, class ಅಥವಾ `id`selector ಗೆ `:hover` style ನಿಯಮಗಳನ್ನ ಸೇರಿಸಬಹುದು.

\--- /collapse \---

+ ಏನಾಗುತ್ತದೆ ಎಂದು ನೀವು ಯೋಚಿಸುತ್ತೀರಿ? ನಿಮ್ಮ ವೆಬ್‌ಸೈಟ್‌ನಲ್ಲಿ ಯಾವ ಪುಟಗಳಲ್ಲಿ ಚಿತ್ರಗಳಿವೆ ಎಂಬುದನ್ನು ಪರಿಶೀಲಿಸಿ (ಯಾವುದೂ ಇಲ್ಲದಿದ್ದರೆ ಚಿತ್ರವನ್ನು ಸೇರಿಸಿ!), ನಂತರ ಕಂಡುಹಿಡಿಯಲು ನಿಮ್ಮ ಕರ್ಸರ್(cursor) ಅನ್ನು ಚಿತ್ರದ ಮೇಲೆ ಸರಿಸಿ!

+ ನೀವು ಅವುಗಳ ಮೇಲೆ ಸುಳಿದಾಡಿದಾಗ, ಲಿಂಕ್ ಗಳು ಹೊಳೆಯಲು ಹೊಸ CSS class ನ ಜೊತೆಗೆ ಒಟ್ಟಿಗೆ `:hover` pseudo-class ಅನ್ನು ಬಳಸೋಣ! ನಿಮ್ಮ ವೆಬ್ ಪುಟಕ್ಕೆ ಲಿಂಕ್ ಸೇರಿಸಿ ಮತ್ತು ವರ್ಗ ಹೆಸರನ್ನು ಸೂಚಿಸಲು ಗುಣಲಕ್ಷಣವನ್ನು ಸೇರಿಸಿ. ನೆನಪಿಡಿ, ಲಿಂಕ್‌ಗಳನ್ನು `<a>` ಟ್ಯಾಗ್ ಬಳಸಿ ವ್ಯಾಖ್ಯಾನಿಸಲಾಗಿದೆ, ಹಾಗೆ:

```html
    <p>
      Visit the <a class="niceLinks" href="https://en.wikipedia.org/wiki/Ireland">Wikipedia page</a> to learn even more about Ireland!
    </p>
```

+ ನಿಮ್ಮ ಸ್ಟೈಲ್ ಶೀಟ್‌(style sheet)‌ಗೆ ಈ ಕೆಳಗಿನ ಕೋಡ್ ಸೇರಿಸಿ, ನಂತರ ನಿಮ್ಮ ಸುಂದರವಾದ ಲಿಂಕ್‌ಗಳನ್ನು ನೋಡಲು ನಿಮ್ಮ ಕೋಡ್ ಅನ್ನು run ಮಾಡಿ.

```css
  .niceLinks {
    text-decoration: none;
    color: #FFFAF0;
  }
  .niceLinks:hover {
    color: #00FF7F;
  }
```

+ ನಿಮ್ಮ ಮೆನು ಬಾರ್‌ನಲ್ಲಿರುವ ಎಲ್ಲಾ ಲಿಂಕ್‌ಗಳಿಗೆ `class="niceLinks"` ಗುಣಲಕ್ಷಣವನ್ನು ಏಕೆ ಸೇರಿಸಬಾರದು?

ಈ ಎಲ್ಲಾ ತಂತ್ರಗಳನ್ನು ನೀವು ಅನಿಮೇಷನ್‌ಗಳೊಂದಿಗೆ ಸಂಯೋಜಿಸಬಹುದು!

+ ಟಿಟೊ(Tito) ಚಿತ್ರಕ್ಕಾಗಿ ಮತ್ತೆ CSS ಬ್ಲಾಕ್ ಅನ್ನು ಹುಡುಕಿ (ಅಥವಾ ನೀವು ಮೊದಲು ಕೆಲಸ ಮಾಡುತ್ತಿದ್ದ ಯಾವುದೇ ಚಿತ್ರ). ನಿಮ್ಮ style sheet‌ ಫೈಲ್ ಗೆ ಈ ಕೆಳಗಿನ Css ಕೋಡ್ ಸೇರಿಸಿ:

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

+ ಏನಾಗುತ್ತದೆ ಎಂದು ನೀವು ಊಹಿಸಬಲ್ಲಿರಾ?

+ ಈಗ ನೀವು ಕರ್ಸರ್ ಅನ್ನು ಚಿತ್ರದ ಮೇಲೆ ಚಲಿಸುವಾಗ "ರೋಲ್ ಓವರ್!"ಎಂದು ಕೂಗಿ ಹೇಳಿ!

\--- challenge \---

## ಸವಾಲು: ಪ್ರಜ್ವಲಿಸುವ ಮಳೆಬಿಲ್ಲು(glowing rainbow) ಲಿಂಕ್‌ಗಳನ್ನು ಮಾಡಿ

+ ಕರ್ಸರ(cursor) ಅದರಮೇಲೆ ಸುಳಿದಾಡುತ್ತಿರುವಾಗ ನಿಮ್ಮ menu ನಲ್ಲಿ ಲಿಂಕ್ ಗಳು ಬಣ್ಣಗಳನ್ನು ಬದಲಾಯಿಸುವಂತೆ ಮಾಡಲು ಹಿಂದಿನ ಕಾರ್ಡ್ ನಿಂದ ನೀವು `rainbowGlow` ಅನಿಮೇಷನ್ ಅನ್ನು ಬಳಸಬಹುದೇ?

\--- hints \---

\--- hint \---

ಕೆಳಗೆ `rainbowGlow` ಅನಿಮೇಷನ್ ಗಾಗಿ ಕೋಡ್ ಇದೆ. ಇದು ಐದು ಹಂತಗಳನ್ನು ವ್ಯಾಖ್ಯಾನಿಸಿದೆ, ಮತ್ತು ಇದು ಪ್ರತಿ ಹಂತದಲ್ಲೂ ವಿಭಿನ್ನ ಪಠ್ಯ ಬಣ್ಣವನ್ನು ಹೊಂದಿಸುತ್ತದೆ. ನೀವು ಹೆಚ್ಚಿನದನ್ನು ಸೇರಿಸಬಹುದು ಅಥವಾ ನಿಮಗೆ ಬೇಕಾದರೂ ಬದಲಾಯಿಸಬಹುದು!

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

\--- /hint \---

\--- hint \---

ನೀವು ಏನನ್ನಾದರೂ ಅನಿಮೇಟ್ ಮಾಡಲು, ನೀವು ಮೇಲೆ ಮಾಡಿದಂತೆ ನಿಯಮಗಳನ್ನು ವಿನ್ಯಾಸ ಮಾಡುವುದಕ್ಕಾಗಿ ಮೂರು `animation` ಗುಣಲಕ್ಷಣಗಳನ್ನು ಸೇರಿಸಿ. ಇಂದಿಗೂ ನೀವು ಬಳಸಲು ಬಯಸುವ ಅನಿಮೇಷನ್ ನ ಹೆಸರು `animation-name` ಜೊತೆಗೆ ಹೋಲಿಕೆಯಾಗುತ್ತದೆಯೇ ಎಂದು ಖಚಿತಪಡಿಸಿಕೊಳ್ಳಿ.

\--- /hint \---

\--- hint \---

ಈ ರೀತಿಯ `nav` menuಗೆ ನೀವು ನೇರವಾಗಿ `hover` effect ಗಳನ್ನು ಸೇರಿಸಬಹುದು:

```css
  nav ul li a:hover {
    animation-name: rainbowGlow;
    animation-duration: 1.5s;
    animation-iteration-count: infinite;
  }
```

ಅಥವಾ, ನಿಮ್ಮ ವೆಬ್‌ಸೈಟ್ ಫ್ಲ್ಯಾಷ್ ರೇನ್‌ಬೋ ಬಣ್ಣಗಳಲ್ಲಿ ಇತರ ಲಿಂಕ್‌ಗಳನ್ನು ಮಾಡಲು ನೀವು ಬಯಸಿದರೆ, ನೀವು ಈ ರೀತಿಯಾಗಿ ಅನಿಮೇಷನ್ ಅನ್ನು `.niceLinks` class ಗೆ ಸೇರಿಸಬಹುದು:

```css
  .niceLinks:hover {
    color: #00BFFF;
    animation-name: rainbowGlow;
    animation-duration: 1.5s;
    animation-iteration-count: infinite;
  }
```

\--- /hint \---

\--- /hints \---

\--- /challenge \---

![](images/badge-footer-image-html-intermed.png)