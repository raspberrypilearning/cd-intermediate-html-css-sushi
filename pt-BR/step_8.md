## Ajuste automaticamente o tamanho

Até agora você estava usando **pixels** para definir o tamanho das coisas, por exemplo `10px`. Neste cartão, você aprenderá sobre outras medidas que você pode usar.

+ Vá para `index.html` e encontre o elemento `img` com a imagem de Tito, ou encontre outra tag `img` no seu site.

+ Exclua o atributo `width`, se houver, e forneça ao elemento um `id` se ainda não tiver um.

```html
  <img src="tito.png" id="titoPicture" alt="Tito o cachorro" />
```

+ No seu arquivo CSS, defina a propriedade `width` para sua imagem, como mostrado abaixo (pode ser necessário criar um bloco CSS com o seletor `id` se você ainda não o fez em um cartão anterior).

```css
  #titoPicture {
    width: 50%;
    border-radius: 100%;
  }
```

Nota: 50% (50 por cento) é **metade**.

+ Tente redimensionar a janela do seu navegador e observe o que acontece com a imagem.

Você deve ver que a imagem aumenta e diminui quando você aumenta ou diminui a janela. Isso ocorre porque ocupa 50% da largura do elemento **main** (que é aproximadamente a largura da página).

--- collapse ---
---
title: Como isso funciona?
---

Quando você define o tamanho de algo em pixels, está definindo um tamanho exato e ele não muda. Isso é chamado de medida **absoluta**.

Outra maneira de definir o tamanho das coisas é usar medidas **relativas**, para que o tamanho dependa do tamanho dos elementos comparados entre si. Então, sempre que algo mudar de tamanho, todo o resto mudará automaticamente de tamanho para manter as mesmas **proporções**.

Quando você está usando medidas **relativas**, é importante saber qual é o **pai** do seu elemento. O pai é a coisa da qual o seu elemento está dentro, e é a isso que a medida será em relação. Por exemplo, o pai da imagem acima é o elemento `article`, porque o elemento `img` está entre as tags `<article></article>`.

Se você definir o `width` de um elemento para `100%`, isso fará com que tenha a mesma largura do contêiner pai.

--- /collapse ---

+ Experimente números diferentes na frente da `%`.