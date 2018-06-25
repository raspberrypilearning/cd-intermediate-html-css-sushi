## Ajusta automáticamente el tamaño

Hasta ahora has estado usando **píxeles** para establecer el tamaño de las cosas, por ejemplo, `10px`. En esta tarjeta, aprenderá sobre otras medidas que puede usar.

+ Vaya a `index.html` y encuentre el elemento `img` con la imagen de Tito, o encuentre otra etiqueta `img` en su sitio web.

+ Elimine el atributo `width` si está allí, y otorgue al elemento un `id` si aún no tiene uno.

```html
  <img src="tito.png" id="titoPicture" alt="Tito the dog" />
```

+ En su archivo CSS, defina la propiedad `width` para su imagen como se muestra a continuación (puede que necesite crear el bloque CSS con el selector `id` si aún no lo ha hecho en una tarjeta anterior).

```css
  #titoPicture {ancho: 50%; radio del borde: 100%; }
```

Nota: 50% (50 por ciento) es **mitad**.

+ Intenta cambiar el tamaño de la ventana de tu navegador y mira lo que sucede con la imagen.

Debería ver que la imagen se hace más grande y más pequeña cuando hace que la ventana sea más grande y más pequeña. Esto se debe a que ocupa el 50% del ancho del **elemento principal** (que es aproximadamente el ancho de la página).

## \--- colapso \---

## título: ¿Cómo funciona?

Cuando establece el tamaño de algo en píxeles, está configurando un tamaño exacto y no cambia. Esto se llama una medida **absoluta**.

Otra forma de establecer el tamaño de las cosas es usando **medidas relativas** , de modo que el tamaño depende de cuán grandes sean los elementos comparados entre sí. Entonces, cada vez que una cosa cambia de tamaño, todo lo demás va a cambiar automáticamente el tamaño así mantener los mismos **proporciones**.

Cuando usa **medidas relativas** , es importante saber cuál es el **padre** de su elemento. El padre es el elemento en el que se encuentra tu elemento, y con eso se relacionará con la medida. Por ejemplo, el padre de la imagen de arriba es el elemento `artículo` , porque el elemento `img` está entre las `<article></article>` etiquetas.

Si se establece el `anchura de` de un elemento a `100%`, que hará que sea la misma anchura que el contenedor primario que se encuentra.

\--- /colapso \---

+ Experimenta con diferentes números frente al `%`.