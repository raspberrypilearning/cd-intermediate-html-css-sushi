## Ajustar automáticamente el tamaño

Hasta ahora has estado usando **píxeles** para establecer el tamaño de las cosas, por ejemplo, `10px`. En esta tarjeta, aprenderás sobre otras medidas que puedes usar.

+ Ve a `index.html` y encuentra el elemento `img` con la imagen de Tito, o encuentra otra etiqueta `img` en tu sitio web.

+ Elimina el atributo `width` si está allí, y dale al elemento un `id` si aún no tiene uno.

```html
  <img src="tito.png" id="titoPicture" alt="Tito the dog" />
```

+ En tu archivo CSS, define la propiedad `width` para tu imagen como se muestra a continuación (puede que necesites crear el bloque CSS con el selector `id` si aún no lo has hecho en una tarjeta anterior).

```css
  #titoPicture {
    width: 50%;
    border-radius: 100%;
  }
```

Nota: 50% (50 por ciento) es la **mitad**.

+ Intenta cambiar el tamaño de la ventana de tu navegador y mira lo que sucede con la imagen.

Deberías ver que la imagen se hace más grande y más pequeña cuando haces que la ventana sea más grande y más pequeña. Esto se debe a que ocupa el 50% del ancho del elemento **principal** (que es aproximadamente el ancho de la página).

--- collapse ---
---
title: ¿Cómo funciona?
---

Cuando estableces el tamaño de algo en píxeles, estás configurando un tamaño exacto y no cambia. Esto se llama una medida **absoluta**.

Otra forma de establecer el tamaño de las cosas es usando **medidas relativas**, de modo que el tamaño depende de cuán grandes sean los elementos comparados entre sí. Entonces, cada vez que una cosa cambia de tamaño, todo lo demás va a cambiar automáticamente de tamaño para así mantener las mismas **proporciones**.

Cuando usas **medidas relativas**, es importante saber cuál es el **padre** de su elemento. El padre es el elemento en el que se encuentra tu elemento, y la medida será en relación con ese elemento. Por ejemplo, el padre de la imagen de arriba es el elemento `article`, porque el elemento `img` está entre las etiquetas `<article></article>`.

Si se establece el `width` de un elemento a `100%`, hará que sea la misma anchura que el contenedor padre en el que se encuentra.

--- /collapse ---

+ Experimenta con diferentes números frente al `%`.