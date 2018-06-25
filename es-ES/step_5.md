## Organizando tu página

Hasta ahora se ha utilizado **epígrafes** y **párrafos** para hacer su **Contenido** aspecto ordenado y fácil de leer. Vamos a hacerlo aún más organizado al agrupar las cosas.

## \--- colapso \---

## título: ¿Qué es contenido?

**contenido** es todo lo que está en su página web, como texto e imágenes.

\--- /colapso \---

+ Vaya al archivo `attractions.html` (o una de sus propias páginas si no está utilizando el proyecto de ejemplo) y, cerca de la parte superior, solo **debajo de** la etiqueta de apertura `<main>` , escriba lo siguiente en una nueva línea : 

```html
  <main>
    <article>
```

+ Si su editor agregó automáticamente una etiqueta de cierre `</article>` , elimínela.

+ En la parte inferior del archivo, solo **encima de** cierre la etiqueta `</main>` , agregue una nueva línea y cierre el elemento `artículo`:

```html
    </article>
  </main>
```

Su `principal` elemento debe ser algo como esto ahora (es posible que tenga un contenido diferente entre el `del artículo` etiquetas por supuesto):

```html
  <main>
    <article>
      <h1>Mis lugares favoritos para ver en Irlanda</h1>
        <h2>The Cliffs of Moher</h2>
        <p>
        Los acantilados de Moher se encuentran en el condado de Clare, de donde soy. ¡Mira qué geniales son!</p>
        <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
        <h2>Achill Island</h2>
        <p>Esta es una gran isla frente a la costa del Condado de Mayo. Tiene un paisaje salvaje y hermoso de montañas, pantanos y acantilados.
        </p>
        <img src="achill.JPG" width="200px" />
    </article>
  </main>
```

+ Ahora mira el contenido de su `artículo` y tratar de dividirlo en secciones. Coloque este nuevo par de etiquetas alrededor de cada bit: `<section> </section>`. Aquí hay un ejemplo de cómo podría verse:

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
      <p>Esta es una gran isla frente a la costa del Condado de Mayo. Tiene un paisaje salvaje y hermoso de montañas, pantanos y acantilados.
      </p>
      <img src="achill.JPG" width="200px" />
    </section>
  </article>
```

## \--- colapso \---

## título: ¿De qué se tratan las nuevas etiquetas?

Piense en estos nuevos elementos como **contenedores**. Se usan para agrupar cosas. ¡Es un poco como organizar cosas en cajas y estantes en tu casa!

Esto hace que su sitio web sea amigable para los lectores de pantalla, le da más control sobre el diseño y, como verá, le permite ser realmente creativo con el diseño.

Cualquier cosa puede ir entre las etiquetas. Por lo general, será más de un elemento, pero no tiene por qué serlo. Puede ser elementos HTML de cualquier tipo. Lo que estás haciendo es decirle al navegador que todo lo que hay entre estas etiquetas pertenece al mismo tiempo.

### Artículo

El elemento `artículo` es un contenedor para una pieza completa de contenido, en este caso un conjunto de información sobre atracciones en Irlanda. Si tiene diferentes fragmentos de contenido que no están relacionados, debe poner cada uno en su propio elemento `artículo` lugar de poner un conjunto de etiquetas alrededor del lote completo.

### Sección

El elemento `sección` permite dividir el contenido relacionado en trozos más pequeños y colocar cada fragmento en su propio contenedor.

### ¡Otros existen también!

Estos no son los únicos elementos contenedores en HTML. Si alguna vez creó un menú y luego lo puso entre `<nav> </nav>` etiquetas, ese es otro ejemplo de un tipo de contenedor. Entonces son `<main> </main>` y `<header> </header>` - ¿Puedes pensar en algo más?

\--- /colapso \---

\--- desafío \---

Es posible que su página web aún no se vea diferente, pero una vez que el contenido se haya organizado en etiquetas de contenedor, podrá hacer algunas cosas interesantes con CSS. Recuerde, HTML controla cómo se organiza su sitio web y CSS controla cómo se ve.

## Desafío: organiza tu sitio web

+ Intente organizar todo el contenido de su sitio web utilizando los contenedores `artículo` y `sección` de esta manera. 

\--- consejos \---

\--- insinuación \---

Mira la página de Comida del proyecto de ejemplo. Verás que agregué un `artículo` con un grupo de `etiquetas de la sección` en el archivo `food.html`:

```html
  <main>
    <article>
      <h1>Comida en Irlanda</h1>
      <p>
        Estas son algunas de mis comidas irlandesas favoritas!
      </p>  
      <section>
        <h2>Desayuno irlandés tradicional</h2>
        <p>
          El desayuno "irlandés completo" consiste en salchichas, lonchas (tocino), huevos, morcilla, budín blanco y pan tostado.
        </p>
        <p>
          A menudo habrá un tomate asado, hongos y frijoles horneados.
        </p>
        <p>
          Y por supuesto, ¡ningún desayuno está completo sin una hermosa olla de té!
        </p>
      </section>

      <section>
        <h2>Bangers and Mash</h2>
        <p>
          Este clásico de salchichas, puré de patatas y salsa no es exclusivo de Irlanda, pero lo que lo hace especial es el de las salchichas irlandesas. La mayoría de los países tienen su propia forma de hacer salchichas, y son una cosa que extraño de casa si estoy de viaje.
        </p>
      </section>

      <section>
        <h2>Bacon y repollo</h2>
        <p>
          No podría hacer una lista de comida irlandesa sin incluir este plato tan tradicional!
        </p>
        <p>
          Puede que no parezca muy interesante, pero esta abundante comida de jamón cocido, patatas y repollo verde es sabrosa y abundante.
          Me encanta sofocar las papas en mantequilla, y también me gusta un poco de mostaza con tocino.
        </p>
        <p>
          Mi madre siempre lo hizo muy especial cocinando el repollo en el agua en la que se hirvió el jamón.
        </p>
        <p>
          Si hay restos, puede hacer otro de mis favoritos: <strong>repollo frito</strong>!
        </p>
      </section>
    </article>     
  </main>
```

\--- /insinuación \---

\--- / consejos \---

En la próxima tarjeta, ¡diseñarás un tema diferente para cada página organizada en artículos y secciones!

\--- / desafío \---