## Organising your page

So far you've used **headings** and **paragraphs** to make your **content** look tidy and easy to read. Let's make it even more organised by grouping things together.

--- collapse ---
---
title: What is content?
---

**Content** is all the "stuff" on your web page, like information and pictures.

--- /collapse ---

+ Go to the `attractions.html` file \(or one of your own pages if you're not using the example project\) and, near the top, just **underneath** the opening `<main>` tag, type the following on a new line: 

```html
  <main>
    <article>
```

+ If your editor automatically added in a closing `</article>` tag for you, delete it.

+ At the bottom of the file, just **above** the closing `</main>` tag, add a new line and close the `article` element:

```html
    </article>
  </main>
```

Your `main` element should look something like this now:

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

+ Now look at the content in your `article`: can you break it up into chunks or sections? If so, put this new set of tags around each bit: `<section> </section>`. Here's an example of what it might look like:

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
title: What are the new tags for?
---

Think of these new elements as **containers**. They are used to group things together. 

Anything can go in between the tags. Usually it will be more than one element but it doesn't have to be, and they can be HTML elements of any kind. What you are doing is telling the browser that everything in between these tags belongs together. Like organising things in boxes and shelves in your home!

### Article

The `article` element is a container for a whole piece of content, in this case a set of information about attractions in my home country, Ireland. If you have different bits of content that aren't related, you should put each one into its own `article` element instead of putting one set of the tags around the whole lot.

### Section

The `section` element lets you divide up related content into smaller chunks and put each chunk into its own container.

### Others exist too!

These aren't the only container elements in HTML. If you've ever created a menu and then put it in between `<nav> </nav>` tags, that's another example of a type of container. 

Using the container elements like this makes your website friendly for screen readers, gives you more control over the layout, and, as you'll see, lets you really get creative with the styling.

--- /collapse ---

Once your content has been organised into `article`s and `section`s you can create CSS rules in the stylesheet to control how the different bits look! The `article` and `section` elements can be styled just like any other HTML element.

+ See if you can understand the CSS rules below and then try to make some of your own.

```css
  section {
    border-top-style: solid;
    border-top-width: 2px;
    border-top-color: #F5FFFA;
    padding-bottom: 10px;
  }

  article {
    border-radius: 10px;
    background-color: #48D1CC;
    padding: 10px;
  }
```

--- challenge ---

## Challenge: Organise your website

+ Have a go at organising all of the content on your website using the `article` and `section` containers in this way. 

--- hints ---

--- hint ---

Look at the Food page of the example project. You'll see I've added an `article` with a bunch of `section`s into the file `food.html`:

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

On the next card you'll design a different theme for each page that's organised into `article`s and `section`s!

--- /challenge ---