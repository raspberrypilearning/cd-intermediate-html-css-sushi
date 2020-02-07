## Animación

¿Sabías que puedes usar CSS para hacer que las cosas se muevan? ¡Aprenderás cómo en esta tarjeta!

+ Antes de comenzar, asegúrate de tener una imagen en tu sitio web con `id` y un bloque CSS correspondiente que establezca `width` a `100px`. Voy con la imagen de Tito de antes, y mi bloque CSS se ve así:

```css
    #titoPicture {
        border-radius: 100%;
        width: 100px;
    }
```

+ Ve a la parte inferior de tu archivo CSS y añade el siguiente código:

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

Este código crea una animación llamada `myFirstAnimation` que puedes añadir a cualquier elemento de tu sitio web. ¿Qué crees que hará?

+ Encuentra tus reglas de CSS para la imagen y añade las siguientes tres propiedades:

```css
    animation-name: myFirstAnimation;
    animation-duration: 2s;
    animation-iteration-count: 1;
```

+ ¡Ahora mira lo que sucede en tu página web! Prueba diferentes valores para `animation-iteration-count` para ver lo que hace.

+ ¡Probemos otra animación! Añade el siguiente código al final de tu archivo CSS:

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

+ Ahora encuentra las reglas CSS `#myCoolText` anteriores y añade el código de animación:

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

Cuando usas **valores porcentuales** en lugar de `from` y de `to`, puedes establecer valores intermedios, así como valores iniciales y finales. Puedes establecer tantos valores intermedios como desees utilizando diferentes valores de porcentaje desde `0` hasta `100`.

+ Cambia el valor de `animation-iteration-count` a `infinite`. ¡Mira si puedes adivinar lo que sucederá antes de probarlo!

+ Prueba diferentes valores para `animation-duration` para acelerar o ralentizar tu animación.

+ ¡Un truco final! Añade este código de animación:

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

+ Ahora encuentra las reglas CSS `#frontPage` que escribiste anteriormente y cámbialas a:

```css
    #frontPage {
        background: repeating-linear-gradient(-45deg, red 0%, yellow 7.14%, lime 14.28%, cyan 21.42%, cyan 28.56%, blue 35.7%, magenta 42.84%, red 50%);
        background-size: 600vw 600vw;
        animation: slide 10s infinite linear forwards;
    }
```

No te preocupes por entender todo el código anterior... ¡¡solo siéntate y disfruta!!

Para conocer más cosas que puedes hacer con animación, visita [esta página web](http://dojo.soy/html2-css-animation){:target="_blank"}. ¡Qué te diviertas!

¡En la siguiente tarjeta, aprenderás cómo hacer que pasen cosas interesantes cuando colocas el cursor del ratón sobre las cosas!