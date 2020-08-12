## ನಿಮ್ಮ ಪುಟವನ್ನು ಆಯೋಜಿಸಲಾಗುತ್ತಿದೆ

ಇಲ್ಲಿಯವರೆಗೂ ನೀವು ನಿಮ್ಮ **content** ಅನ್ನು ಅಚ್ಚುಕಟ್ಟಾಗಿ ಮತ್ತು ಓದಲು ಸುಲಭವಾಗಲು **headings** ಮತ್ತು **paragraphs** ಅನ್ನು ಬಳಸಿದ್ದೀರಿ. ವಿಷಯಗಳನ್ನು ಒಟ್ಟಿಗೆ ಗುಂಪು ಮಾಡುವ ಮೂಲಕ ಅದನ್ನು ಇನ್ನಷ್ಟು ಸಂಘಟಿಸೋಣ.

--- collapse ---
---
title: ವಿಷಯ ಏನು?
---

**content** ನಿಮ್ಮ ವೆಬ್ ಪುಟದಲ್ಲಿನ ಎಲ್ಲಾ ವಿಷಯಗಳು, ಉದಾಹರಣೆಗಾಗಿ ಪಠ್ಯ ಮತ್ತು ಚಿತ್ರಗಳು.

--- /collapse ---

+ `attractions.html` ಫೈಲ್‌ಗೆ ಹೋಗಿ (ಅಥವಾ ನೀವು ಉದಾಹರಣೆ ಯೋಜನೆಯನ್ನು ಬಳಸದಿದ್ದರೆ ನಿಮ್ಮ ಸ್ವಂತ ಪುಟಗಳಲ್ಲಿ ಒಂದಾಗಿದೆ) ಮತ್ತು, ಮೇಲ್ಭಾಗದ ಹತ್ತಿರ, ಆರಂಭಿಕ **ಕೆಳಗೆ** `<main>` ಟ್ಯಾಗ್, ಹೊಸ ಸಾಲಿನಲ್ಲಿ ಈ ಕೆಳಗಿನವುಗಳನ್ನು ಟೈಪ್ ಮಾಡಿ: 

```html
  <main>
    <article>
```

+ ನಿಮ್ಮ ಸಂಪಾದಕವು ಸ್ವಯಂಚಾಲಿತವಾಗಿ ಮುಕ್ತಾಯದ `</article>` ಟ್ಯಾಗ್ ಅನ್ನು ನಿಮಗಾಗಿ ಸೇರಿಸಿದರೆ, ಅದನ್ನು ಅಳಿಸಿ.

+ ಫೈಲ್‌ನ ಕೆಳಭಾಗದಲ್ಲಿ, ಕೇವಲ ಮುಕ್ತಾಯದ `</main>` ಟ್ಯಾಗ್ **ಮೇಲೆ**, ಹೊಸ ಸಾಲನ್ನು ಸೇರಿಸಿ ಮತ್ತು `article` ಅಂಶವನ್ನು ಮುಚ್ಚಿ:

```html
    </article>
  </main>
```

ನಿಮ್ಮ `main` ಅಂಶವು ಈಗ ಈ ರೀತಿ ಕಾಣಬೇಕು (`article` ಟ್ಯಾಗ್‌ಗಳ ನಡುವೆ ನೀವು ವಿಭಿನ್ನ ವಿಷಯವನ್ನು ಹೊಂದಿರಬಹುದು):

```html
  <main>
    <article>
      <h1>My favourite places to see in Ireland</h1>
        <h2>The Cliffs of Moher</h2>
        <p>
        The Cliffs of Moher are found in County Clare, where I am from. Look how cool they are!</p>
        <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
        <h2>Achill Island</h2>
        <p>This is a large island off the coast of County Mayo. It has a wild and
        beautiful landscape of mountains, bogs and cliffs.
        </p>
        <img src="achill.JPG" width="200px" />
    </article>
  </main>
```

+ ಈಗ ನಿಮ್ಮ `article` ವಿಷಯವನ್ನು ನೋಡಿ ಮತ್ತು ಅದನ್ನು ವಿಭಾಗಗಳಾಗಿ ವಿಭಜಿಸಲು ಪ್ರಯತ್ನಿಸಿ. ಈ ಹೊಸ ಟ್ಯಾಗ್‌ಗಳ ಜೋಡಿಯನ್ನ ಪ್ರತಿ ಬಿಟ್(bit)‌ನ ಸುತ್ತಲೂ ಇರಿಸಿ: `<section> </section>`. ಅದು ಹೇಗಿರಬಹುದು ಎಂಬುದಕ್ಕೆ ಉದಾಹರಣೆ ಇಲ್ಲಿದೆ:

```html
  <article>
    <h1>My favourite places to see in Ireland</h1>
    <section>
      <h2>The Cliffs of Moher</h2>
      <p>
      The Cliffs of Moher are found in County Clare, where I am from. Look how cool they are!</p>
      <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
    </section>
    <section>
      <h2>Achill Island</h2>
      <p>This is a large island off the coast of County Mayo. It has a wild and
      beautiful landscape of mountains, bogs and cliffs.
      </p>
      <img src="achill.JPG" width="200px" />
    </section>
  </article>
```

--- collapse ---
---
title: ಹೊಸ ಟ್ಯಾಗ್‌ಗಳು ಯಾವುವು?
---

ಈ ಹೊಸ ಅಂಶಗಳನ್ನು **containers** ಎಂದು ಯೋಚಿಸಿ. ವಿಷಯಗಳನ್ನು ಒಟ್ಟಿಗೆ ಗುಂಪು ಮಾಡಲು ಅವುಗಳನ್ನು ಬಳಸಲಾಗುತ್ತದೆ. ಇದು ನಿಮ್ಮ ಮನೆಯಲ್ಲಿ ಪೆಟ್ಟಿಗೆಗಳು ಮತ್ತು ಕಪಾಟಿನಲ್ಲಿ ವಸ್ತುಗಳನ್ನು ಸಂಘಟಿಸುವಂತಿದೆ!

ಇದು ನಿಮ್ಮ ವೆಬ್‌ಸೈಟ್ ಸ್ಕ್ರೀನ್ ಓದುಗರಿಗೆ ಸ್ನೇಹಪರವಾಗಿಸುತ್ತದೆ, ಲೇಔಟ್(layout) ಮೇಲೆ ಹೆಚ್ಚಿನ ನಿಯಂತ್ರಣವನ್ನು ನೀಡುತ್ತದೆ, ಮತ್ತು ನೀವು ನೋಡುವಂತೆ, ಸ್ಟೈಲಿಂಗ್‌ನೊಂದಿಗೆ ನಿಜವಾಗಿಯೂ ಸೃಜನಶೀಲತೆಯನ್ನು ಪಡೆಯಲು ಇದು ನಿಮ್ಮನ್ನು ಅನುಮತಿಸುತ್ತದೆ.

ಟ್ಯಾಗ್‌ಗಳ ನಡುವೆ ಏನು ಬೇಕಾದರೂ ಹೋಗಬಹುದು. ಸಾಮಾನ್ಯವಾಗಿ ಇದು ಒಂದಕ್ಕಿಂತ ಹೆಚ್ಚು ಅಂಶಗಳಾಗಿರುತ್ತದೆ, ಆದರೆ ಅದು ಇರಬೇಕಾಗಿಲ್ಲ. ಇದು ಯಾವುದೇ ರೀತಿಯ HTML ಅಂಶಗಳಾಗಿರಬಹುದು. ನೀವು ಮಾಡುತ್ತಿರುವುದು ಏನೆಂದರೆ ಈ ಟ್ಯಾಗ್‌ಗಳ ನಡುವೆ ಎಲ್ಲವೂ ಒಟ್ಟಿಗೆ ಸೇರಿದೆ ಎಂದು ಬ್ರೌಸರ್‌ಗೆ ಹೇಳುವುದು.

### ಲೇಖನ

`article` ಅಂಶವು ಇಡೀ ವಿಷಯದ ಒಂದು ಧಾರಕವಾಗಿದೆ, ಈ ಸಂದರ್ಭದಲ್ಲಿ ಐರ್ಲೆಂಡ್‌ನಲ್ಲಿನ ಆಕರ್ಷಣೆಗಳ ಬಗ್ಗೆ ಮಾಹಿತಿಯ ಒಂದು ಸೆಟ್. ನೀವು ಸಂಬಂಧವಿಲ್ಲದ ವಿಭಿನ್ನ ಬಿಟ್‌ಗಳನ್ನು ಹೊಂದಿದ್ದರೆ, ಸ್ಥಳದ ಸುತ್ತ ಟ್ಯಾಗ್ ಗಳ ಗುಂಪನ್ನು ಹಾಕುವ ಬದಲು ಪ್ರತಿಯೊಂದನ್ನು ತನ್ನದೇ ಆದ `article` ಅಂಶದಲ್ಲಿ ಹಾಕಬೇಕು.

### ವಿಭಾಗ

`section` ಅಂಶಗಳ ಸಂಬಂಧಿತ ವಿಷಯವನ್ನು ಸಣ್ಣ ಭಾಗಗಳಾಗಿ ವಿಂಗಡಿಸಲು ಮತ್ತು ಪ್ರತಿಯೊಂದು ಭಾಗವನ್ನು ತನ್ನದೇ ಆದ ಪಾತ್ರೆಯಲ್ಲಿ ಇರಿಸಲು ಅಂಶವು ನಿಮಗೆ ಅನುಮತಿಸುತ್ತದೆ.

### ಇತರರು ಸಹ ಅಸ್ತಿತ್ವದಲ್ಲಿದ್ದಾರೆ!

ಇವುಗಳು HTML ನಲ್ಲಿರುವ ಏಕೈಕ ಧಾರಕ ಅಂಶಗಳಲ್ಲ. ನೀವು ಎಂದಾದರೂ ಮೆನುವನ್ನು ರಚಿಸಿ ನಂತರ ಅದನ್ನು `<nav> </nav>` ಟ್ಯಾಗ್‌ಗಳ ನಡುವೆ ಇರಿಸಿ, ಅದು ಒಂದು ರೀತಿಯ ಧಾರಕದ(container) ಮತ್ತೊಂದು ಉದಾಹರಣೆಯಾಗಿದೆ. ಆದ್ದರಿಂದ `<main> </main>` ಮತ್ತು `<header> </header>` - ನೀವು ಇನ್ನೇನಾದರೂ ಯೋಚಿಸಬಹುದೇ?

--- /collapse ---

--- challenge ---

ನಿಮ್ಮ ವೆಬ್ ಪುಟ ಇನ್ನೂ ವಿಭಿನ್ನವಾಗಿ ಕಾಣಿಸದೇ ಇರಬಹುದು, ಆದರೆ ವಿಷಯವನ್ನು ಕಂಟೇನರ್ ಟ್ಯಾಗ್‌ಗಳಾಗಿ ಸಂಘಟಿಸಿದ ನಂತರ, ನೀವು CSS‌ನೊಂದಿಗೆ ಅದಕ್ಕೆ ಕೆಲವು ಉತ್ತಮ ಕೆಲಸಗಳನ್ನು ಮಾಡಲು ಸಾಧ್ಯವಾಗುತ್ತದೆ. ನೆನಪಿಡಿ, ನಿಮ್ಮ ವೆಬ್‌ಸೈಟ್ ಹೇಗೆ ಸಂಘಟಿತವಾಗಿದೆ ಎಂಬುದನ್ನು HTML ನಿಯಂತ್ರಿಸುತ್ತದೆ ಮತ್ತು CSS ಅದು ಹೇಗೆ ಕಾಣುತ್ತದೆ ಎಂಬುದನ್ನು ನಿಯಂತ್ರಿಸುತ್ತದೆ.

## ಸವಾಲು: ನಿಮ್ಮ ವೆಬ್‌ಸೈಟ್ ಅನ್ನು ಆಯೋಜಿಸಿ

+ `article` ಮತ್ತು `section` ನಂತಹ ಧಾರಕಗಳನ್ನು ಉಪಯೋಗಿಸಿ ಈ ಮೂಲಕ ನಿಮ್ಮ ವೆಬ್ಸೈಟ್ ನ ಎಲ್ಲ ವಿಷಯವನ್ನು ಸಂಘಟಿಸಿ. 

--- hints ---


--- hint ---

ಉದಾಹರಣೆ ಯೋಜನೆಯ ಆಹಾರ ಪುಟವನ್ನು ನೋಡಿ. ನಾನು `food.html` ಫೈಲ್ ನಲ್ಲಿ `article` ನ ಜೊತೆಗೆ `section` ನ ಗುಂಪನ್ನು ಸೇರಿಸಿದ್ದೇನೆ ಎಂದು ನೀವು ನೋಡುವಿರಿ:

```html
  <main>
    <article>
      <h1>Food in Ireland</h1>
      <p>
        These are some of my favourite Irish foods!
      </p>  
      <section>
        <h2>Traditional Irish Breakfast</h2>
        <p>
          A "Full Irish" breakfast consists of sausages, rashers (bacon),
          eggs, black pudding, white pudding and toast.
        </p>
        <p>
          Often there will be a grilled tomato as well as mushrooms,
          and baked beans.
        </p>
        <p>
          And of course, no breakfast is complete without a lovely pot 
          of tea!
        </p>
      </section>

      <section>
        <h2>Bangers and Mash</h2>
        <p>
          This classic of sausages, mashed potato and gravy is not
          unique to Ireland, but what makes it special is the Irish
          sausages. Most countries have their own way of making sausages,
          and they are one thing I miss from home if I'm away travelling!
        </p>
      </section>

      <section>
        <h2>Bacon and Cabbage</h2>
        <p>
          I couldn't possibly make a list of Irish food without including
          this very traditional dish!
        </p>
        <p>
          It might not sound very interesting, but this hearty meal of
          boiled ham, potatoes and green cabbage is tasty and filling.
          I love to smother the potatoes in butter, and I also like a
          little mustard with the bacon.
        </p>
        <p>
          My mum always made it extra special by cooking the cabbage in
          the water that the ham was boiled in.
        </p>
        <p>
          If there are any leftovers you can make another one of my
          favourites: <strong>fried cabbage</strong>!
        </p>
      </section>
    </article>     
  </main>
```

--- /hint ---

--- /hints ---

ಮುಂದಿನ ಕಾರ್ಡ್‌ನಲ್ಲಿ, ಲೇಖನಗಳು ಮತ್ತು ವಿಭಾಗಗಳಾಗಿ ಸಂಘಟಿಸಲಾದ ಪ್ರತಿಯೊಂದು ಪುಟಕ್ಕೂ ನೀವು ವಿಭಿನ್ನ ಥೀಮ್ ಅನ್ನು ವಿನ್ಯಾಸಗೊಳಿಸುತ್ತೀರಿ!

--- /challenge ---