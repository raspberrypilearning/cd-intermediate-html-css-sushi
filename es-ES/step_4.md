## Organizando tu página

Hasta ahora has utilizado **epígrafes** y **párrafos** para hacer que el **contenido** tenga un aspecto ordenado y fácil de leer. Vamos a hacerlo aún más organizado al agrupar las cosas.

## \--- collapse \---

## title: ¿Qué es el contenido?

**Contenido** es todo lo que está en tu página web, como texto e imágenes.

\--- /collapse \---

+ Ve al archivo `attractions.html` (o una de tus propias páginas si no estás utilizando el proyecto de ejemplo) y, cerca de la parte superior, solo **debajo de** la etiqueta de apertura `<main>`, escribe lo siguiente en una nueva línea: 

```html
  <main>
<article>
```

+ Si tu editor añadió automáticamente una etiqueta de cierre `</article>`, elimínala.

+ En la parte inferior del archivo, solo **encima del** cierre de la etiqueta `</main>`, añade una nueva línea y cierra el elemento `article`:

```html
    </article>
</main>
```

Tu elemento `main` debe ser algo como esto (es posible que tenga un contenido diferente entre las etiquetas `article`):

```html
  <main>
    <article>
      <h1>Mis lugares favoritos para ver en Irlanda</h1>
        <h2>The Cliffs of Moher</h2>
        <p>
        Los acantilados de Moher se encuentran en el condado de Clare, de donde soy. ¡Mira qué geniales son!</p>
        <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
        <h2>Achill Island</h2>
        <p>Esta es una gran isla frente a la costa del Condado de Mayo. Tiene un paisaje salvaje y
hermoso de montañas, pantanos y acantilados.
        </p>
        <img src="achill.JPG" width="200px" />
    </article>
  </main>
```

+ Ahora mira el contenido de tu `article` y trata de dividirlo en secciones. Put this new pair of tags around each bit: `<section> </section>`. Aquí hay un ejemplo de cómo podría verse:

```html
  <article>
    <h1>Mis lugares favoritos para ver en Irlanda</h1>
    <section>
      <h2>The Cliffs of Moher</h2>
      <p>
      The Cliffs of Moher se encuentran en el condado de Clare, de donde soy. ¡Mira qué geniales son!</p>
      <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
    </section>
    <section>
      <h2>Achill Island</h2>
      <p>Esta es una gran isla frente a la costa del Condado de Mayo. Tiene un paisaje salvaje y
        hermoso de montañas, pantanos y acantilados.
      </p>
      <img src="achill.JPG" width="200px" />
    </section>
  </article>
```

## \--- collapse \---

## title: What are the new tags all about?

Piensa en estos nuevos elementos como **contenedores**. Se usan para agrupar cosas. ¡Es un poco como organizar cosas en cajas y estantes en tu casa!

Esto hace que tu sitio web sea amigable para los lectores de pantalla, te da más control sobre el diseño y, como verás, te permite ser realmente creativo con el diseño.

Cualquier cosa puede ir entre las etiquetas. Por lo general, será más de un elemento, pero no tiene por qué serlo. Pueden ser elementos HTML de cualquier tipo. Lo que estás haciendo es decirle al navegador que todo lo que hay entre estas etiquetas debe estar unido.

### Artículo

El elemento `article` es un contenedor para una pieza completa de contenido, en este caso un conjunto de información sobre atracciones en Irlanda. Si tienes diferentes fragmentos de contenido que no están relacionados, debes poner cada uno en su propio elemento `article` en lugar de poner un conjunto de etiquetas alrededor del lote completo.

### Sección

El elemento `section` permite dividir el contenido relacionado en trozos más pequeños y colocar cada fragmento en su propio contenedor.

### ¡Existen más elementos!

Estos no son los únicos elementos contenedores en HTML. Si alguna vez creaste un menú y luego lo pusiste entre etiquetas `<nav> </nav>`, ese es otro ejemplo de un tipo de contenedor. También lo son `<main> </main>` y `<header> </header>` - ¿Puedes pensar en algunos más?

\--- /collapse \---

\--- challenge \---

Es posible que tu página web aún no se vea diferente, pero una vez que el contenido se haya organizado en etiquetas de contenedor, podrás hacer algunas cosas interesantes con CSS. Recuerda, HTML controla cómo se organiza tu sitio web y CSS controla cómo se ve.

## Desafío: organiza tu sitio web

+ Intenta organizar todo el contenido de tu sitio web utilizando los contenedores `article` y `section` de esta manera. 

\--- hints \---

\--- hint \---

Mira la página de Comida del proyecto de ejemplo. Verás que añadí un `article` con un grupo de etiquetas `section` en el archivo `food.html`:

```html
  <main>
    <article>
      <h1>Comida en Irlanda</h1>
      <p>
        ¡Estas son algunas de mis comidas irlandesas favoritas!
      </p>  
      <section>
        <h2>Traditional Irish Breakfast</h2>
        <p>
          A "Full Irish" breakfast consists of sausages, rashers (bacon),
          eggs, black pudding, white pudding and toast.
        </p>
        <p>
          A menudo habrá un tomate asado, así como champiñones 
          y judías horneadas.
        </p>
        <p>
          Y por supuesto, ¡ningún desayuno está completo sin una hermosa taza
          de té!
        </p>
      </section>

      <section>
        <h2>Bangers y Mash</h2>
        <p>
          Este clásico de salchichas, puré de patatas y salsa no es
          exclusivo de Irlanda, pero lo que lo hace especial es las salchichas
          irlandesas. La mayoría de los países tienen su propia forma de hacer salchichas,
         ¡y son una cosa que extraño de casa si estoy de viaje!
        </p>
      </section>

      <section>
        <h2>Bacon and Cabbage</h2>
        <p>
          I couldn't possibly make a list of Irish food without including
          this very traditional dish!
        </p>
        <p>
          Puede que no parezca muy interesante, pero esta abundante comida de
          jamón cocido, patatas y repollo verde es sabrosa y abundante.
          I love to smother the potatoes in butter, and I also like a
          little mustard with the bacon.
        </p>
        <p>
          My mum always made it extra special by cooking the cabbage in
          the water that the ham was boiled in.
        </p>
        <p>
          ¡Si hay sobras, puedes hacer otro de mis favoritos: <strong>repollo frito</strong>!
        </p>
      </section>
    </article>     
  </main>
```

\--- /hint \---

\--- /hints \---

En la próxima tarjeta, ¡diseñarás un tema diferente para cada página, organizada en artículos y secciones!

\--- /challenge \---