## Організація вашої сторінки

Досі ви використовували **заголовки** та **абзацими** щоб зробити **вміст** вашої сторінки більш охайним та легким для читання. Давайте тепер зробимо її більш організованою шляхом групування речей.

## \--- collapse \---

## title: Що таке вміст?

** Зміст ** - це всі речі на вашій вебсторінці, такі як текст та зображення.

\--- /collapse \---

+ Перейдіть до `attractions.html` файлу (або на одну з ваших власних сторінок, якщо ви не використовуєте проекту з прикладу), та, напочатку, просто **нижче** відкриваючого тегу `<main>`, введіть наступне у новому рядку: 

```html
  <main>
    <article>
```

+ Якщо ваш редактор автоматично додає закриваючий тег `</article>` за вас, видаліть його.

+ У нижній частині файлу - просто **вище** закриваючого `</main>`</code> тегу, додати новий рядок та закрити ` article </1> елемент:</p></li>
</ul>

<pre><code class="html">    </article>
  </main>
`</pre> 
    
    Ваш `main` елемент повинен виглядати приблизно так (Звичайно, ви можете мати інший вміст між `article` тегами):
    
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
    
    + Тепер подивіться на зміст у своїй ` article ` і спробуйте розділити його на розділи. Додайте нову пару тегів `<section> </section>` навколо кожного розділу. Ось приклад того, як це може виглядати:
    
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
    
    ## \--- collapse \---
    
    ## title: Що таке ці нові теги?
    
    Подумайте про ці нові елементи як **контенери**. Вони використовуються для групування. Це трохи схоже на організацію речей по коробках та полицях у вашому домі!
    
    Це дозволяє зробити ваш сайт зручним для читання з екрану, надає вам більше контролю над макетом сайту, і, як ви бачите, це дозволяє по-справжньому творчо виконувати стилізування.
    
    Будь-що може бути розміщене між тегами. Зазвичай це буде більше ніж один елемент, але це необов'язково. Це можуть бути будь-які HTML елементи. Що ви робите, так це говорите браузеру, що все, що знаходиться між цими тегами йде разом.
    
    ### Елемент Article
    
    Елемент `article` - це контейнер для цілого шматка вмісту, у цьому випадку для інформації про пам'ятки України. Якщо у вас є різні частини контенту, які не пов'язані між собою, тоді ви повинні помістити кожну частину у свій ` article ` елемент замість того, щоб покласти один набір тегів навколо всього лоту.
    
    ### Section
    
    The `section` element lets you divide up related content into smaller chunks and put each chunk into its own container.
    
    ### Others exist too!
    
    These aren't the only container elements in HTML. If you've ever created a menu and then put it in between `<nav> </nav>` tags, that's another example of a type of container. So are `<main> </main>` and `<header> </header>` — can you think of any more?
    
    \--- /collapse \---
    
    \--- challenge \---
    
    Your web page might not look different yet, but once the content has been organised into container tags, you'll be able to do some cool things to it with CSS. Remember, HTML controls how your website is organised, and CSS controls how it looks.
    
    ## Challenge: organise your website
    
    + Have a go at organising all of the content on your website using the `article` and `section` containers in this way. 
    
    \--- hints \---
    
    \--- hint \---
    
    Подивіться на сторінку Food у проекті-прикладі. You'll see that I've added an `article` with a bunch of `section` tags into the file `food.html`:
    
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
    
    \--- /hint \---
    
    \--- /hints \---
    
    On the next card, you'll design a different theme for each page that's organised into articles and sections!
    
    \--- /challenge \---