## Animación

¿Sabía que puede usar CSS para hacer que las cosas se muevan? ¡Aprenderá cómo en esta tarjeta!

+ Antes de comenzar, asegúrese de tener una imagen en su sitio web con `id` y un bloque CSS correspondiente que establezca el ancho `` a `100px`. Voy con la imagen de Tito de antes, y mi bloque CSS se ve así:

```css
    #titoPicture {border-radius: 100%; ancho: 100px; }
```

+ Vaya a la parte inferior de su archivo CSS y agregue el siguiente código:

```css
    @keyframes myFirstAnimation {from {width: 100px; } a {ancho: 300px; }}
```

Este código crea una animación llamada `myFirstAnimation` que puede agregar a cualquier elemento de su sitio web. ¿Qué crees que hará?

+ Encuentre sus reglas de CSS para la imagen y agregue las siguientes tres propiedades:

```css
    nombre-animación: myFirstAnimation; animación-duración: 2s; recuento de iteración-animación: 1;
```

+ ¡Ahora mira lo que sucede en tu página web! Pruebe diferentes valores para `animation-iteration-count` para ver lo que hace.

+ Probemos otra animación! Agregue el siguiente código al final de su archivo CSS:

```css
    @keyframes rainbowGlow {0% {color: # FFD700; } 50% {color: # 663399; } 100% {color: # FFD700; }}
```

+ Ahora encuentre las reglas</code> CSS `# myCoolText ` anteriores y agregue el código de animación:

```css
    #myCoolText {color: # 003366; borde: cresta 2px #ccffff; relleno: 15px; text-align: center; nombre-animación: rainbowGlow; animación-duración: 1.5s; recuento de iteración-animación: 1; }
```

Cuando usa **valores porcentuales** lugar de `de` y de `a`, puede establecer valores intermedios y solo valores iniciales y finales. Puede establecer tantos valores intermedios como desee utilizando diferentes valores de porcentaje desde `0` hasta `100`.

+ Cambia el valor de `animation-iteration-count` a `infinite`. Vea si puede adivinar lo que sucederá antes de probarlo.

+ Pruebe diferentes valores para `animación-duración` para acelerar o ralentizar su animación.

+ ¡Un truco final! Agregue este código de animación:

```css
    @keyframes slide {0% {background-position-x: 0; } 100% {background-position-x: 600vw; }}
```

+ Ahora encuentre las reglas `#frontPage` CSS que escribió anteriormente y cámbielas a:

```css
    #frontPage {background: repeating-linear-gradient (-45deg, red 0%, yellow 7.14%, lime 14.28%, cian 21.42%, cian 28.56%, azul 35.7%, magenta 42.84%, red 50%); fondo de tamaño: 600vw 600vw; animación: diapositiva 10s adelante infinito infinito; }
```

No te preocupes por entender todo el código anterior ... solo siéntate y disfruta !!

Para conocer más cosas que puedes hacer con animación, visita [esta página web](http://dojo.soy/html2-css-animation){: target = "_ blank"}. ¡Que te diviertas!

En la siguiente carta, aprenderás cómo hacer que pasen cosas interesantes cuando colocas el cursor del mouse sobre las cosas.