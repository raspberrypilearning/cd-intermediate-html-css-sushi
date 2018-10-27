## ¡Enséñale a Tito a darse la vuelta!

Puede hacer que su sitio web sea más **interactiva** haciendo cosas interesantes sucede cuando se pasa sobre las cosas con el cursor del ratón!

+ Encuentra tus reglas CSS para los elementos `img` , o crea algunos si no tienes ninguno. Agregue un borde y luego agregue un nuevo bloque de reglas justo debajo:

```css
  img {border: 2px sólido Blanco; } img: hover {border: 2px dashed Navy; }
```

Acaba de utilizar un tipo especial de bloque CSS llamado **pseudo-class**.

## \--- colapso \---

## título: ¿Cómo funciona?

Una **pseudo-clase** es un poco diferente de una **clase** que usted mismo crea. Puedes reconocerlo por `:`.

Las pseudo-clases vienen integradas en elementos HTML: puede agregar reglas de estilo `: hover` a cualquier elemento, clase o selector de `id` en su hoja de estilos sin la necesidad de agregar nada adicional en su código HTML.

\--- /colapso \---

+ ¿Qué piensas tú que sucederá? Compruebe qué páginas de su sitio web tienen imágenes (¡agregue una imagen si no hay ninguna!), Luego mueva el cursor sobre una imagen para descubrirla.

+ ¡Usemos esta nueva pseudoclase `: hover` junto con una clase CSS para hacer que los enlaces brillen cuando pasamos el cursor sobre ellos! Agregue un enlace a su página web e incluya un atributo para especificar el nombre de la clase. Recuerda, los enlaces se definen usando la etiqueta `<a>` , así:

```html
    <p>
      Visita la página <a class="niceLinks" href="https://en.wikipedia.org/wiki/Ireland">Wikipedia</a> para aprender aún más sobre Irlanda!
    </p>
```

+ Agregue el siguiente código a su hoja de estilo, luego ejecute su código para ver sus enlaces encantadores en acción.

```css
  .niceLinks {text-decoration: none; color: # FFFAF0; } .niceLinks: hover {color: # 00FF7F; }
```

+ ¿Por qué no agregar el atributo `class = "niceLinks"` a todos los enlaces en su barra de menú también?

¡Puedes combinar todos estos trucos con animaciones también!

+ Encuentra el bloque CSS para la imagen de Tito nuevamente (o la imagen en la que estuviste trabajando antes). Agregue el siguiente código a su archivo de hoja de estilo:

```css
  #titoPicture {border-radius: 100%; ancho: 100px; } #titoPicture: hover {nombre-animación: rollOver; animación-duración: 1s; recuento de iteración-animación: 1; } @keyframes rollOver {0% {transform: rotate (0deg); } 100% {transform: rotate (-360deg); }}
```

+ ¿Puedes adivinar lo que sucederá?

+ Ahora grita "¡Rueda!" a medida que mueves el cursor sobre la imagen

\--- desafío \---

## Desafío: hacer brillantes enlaces de arcoiris

+ ¿Puedes usar la animación `rainbowGlow` de la tarjeta anterior para hacer que los enlaces en tu menú sigan cambiando de color cuando el cursor se cierne sobre ellos?

\--- consejos \---

\--- insinuación \---

A continuación se muestra el código para la animación `rainbowGlow`. Tiene cinco etapas definidas, y establece un color de texto diferente en cada etapa. ¡Puedes agregar más o cambiarlos como quieras!

```css
    @keyframes rainbowGlow {0% {color: # 00BFFF; } 25% {color: # 00FF7F; } 50% {color: #eeeeaf; } 75% {color: #eeafee; } 100% {color: # 00BFFF; }}
```

\--- /insinuación \---

\--- insinuación \---

Para animar algo, agregue las tres propiedades `animación` a sus reglas de estilo como lo hizo anteriormente. Siempre asegúrese de que el `nombre-animación` coincida con el nombre de la animación que desea usar.

\--- /insinuación \---

\--- insinuación \---

Puede agregar `efectos de desplazamiento estacionario` directamente al menú `nav` esta manera:

```css
  nav ul li a: hover {nombre-animación: rainbowGlow; animación-duración: 1.5s; animation-iteration-count: infinite; }
```

O bien, si desea hacer que otros enlaces de su sitio web también muestren colores del arcoíris, puede agregar la animación a la clase `.niceLinks` , como esta:

```css
  .niceLinks: hover {color: # 00BFFF; nombre-animación: rainbowGlow; animación-duración: 1.5s; animation-iteration-count: infinite; }
```

\--- /insinuación \---

\--- / consejos \---

\--- / desafío \---

![](images/badge-footer-image-html-intermed.png)