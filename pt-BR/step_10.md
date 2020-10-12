## Ensine Tito a rolar!

Você pode tornar seu site mais **interativo** fazendo coisas legais acontecerem quando você passa com o cursor do mouse sobre alguns elementos!

+ Encontre suas regras de CSS para os elementos `img`, ou crie alguma se você não tiver nenhuma. Adicione uma borda e também um novo bloco de regras logo abaixo:

```css
  img {
    border: 2px solid White;
  }
  img:hover {
    border: 2px dashed Navy;
  }
```

Você acabou de usar um tipo especial de bloco CSS chamado **pseudo-classe**.

--- collapse ---
---
title: Como isso funciona?
---

Uma **pseudo-classe** é um pouco diferente de uma **classe** que você mesmo cria. Você pode reconhecê-la pelo `:`.

As pseudo-classes são incorporadas aos elementos HTML: você pode adicionar regras de estilo `:hover` para qualquer elemento, classe ou seletor `id` na sua folha de estilos, sem precisar adicionar nada extra ao seu código HTML.

--- /collapse ---

+ O que você acha que vai acontecer? Verifique quais páginas do seu site têm fotos (adicione uma foto, se não houver!) e mova o cursor sobre uma foto para descobrir!

+ Vamos usar esta nova pseudo-classe `:hover` junto com uma classe CSS para fazer os links brilharem quando você passar o mouse sobre eles! Adicione um link à sua página da web e inclua um atributo para especificar o nome da classe. Lembre-se, os links são definidos usando a tag `<a>`, assim:

```html
    <p>
      Visite a <a class="niceLinks" href="https://en.wikipedia.org/wiki/Ireland">página da Wikipedia</a> para aprender ainda mais sobre a Irlanda!
    </p>
```

+ Adicione o seguinte código à sua folha de estilos, e execute o código para ver seus links adoráveis em ação.

```css
  .niceLinks {
    text-decoration: none;
    color: #FFFAF0;
  }
  .niceLinks:hover {
    color: #00FF7F;
  }
```

+ Por que não adicionar também o atributo `class="niceLinks"` para todos os links da barra de menu?

Você pode combinar todos esses truques com as animações também!

+ Encontre o bloco CSS da imagem do Tito novamente (ou qualquer imagem em que você estava trabalhando anteriormente). Adicione o seguinte código ao seu arquivo de folha de estilos:

```css
  #titoPicture {
    border-radius: 100%;
    width: 100px;
  }
  #titoPicture:hover {
    animation-name: rollOver;
    animation-duration: 1s;
    animation-iteration-count: 1;
  }
  @keyframes rollOver {
    0% {
      transform: rotate(0deg);
    }
    100% {
      transform: rotate(-360deg);
    }
  }
```

+ Você consegue adivinhar o que vai acontecer?

+ Agora grite "Role!" enquanto você move o cursor sobre a imagem!

--- challenge ---

## Desafio: faça links brilhantes nas cores de um arco-íris

+ Você pode usar a animação `rainbowGlow` do cartão anterior para fazer com que os links em seu menu continuem mudando de cor quando o cursor estiver sobre eles?

--- hints ---


--- hint ---

Abaixo está o código para a animação `rainbowGlow`. Existem cinco estágios definidos, e uma cor de texto diferente é definida em cada estágio. Você pode adicionar mais ou alterá-los como quiser!

```css
    @keyframes rainbowGlow {
        0% {
            color: #00BFFF;
        }
        25% {
            color: #00FF7F;
        }
        50% {
            color: #eeeeaf;
        }
        75% {
            color: #eeafee;
        }
        100% {
            color: #00BFFF;
        }
    }
```

--- /hint ---

--- hint ---

Para animar algo, você precisará adicionar as três propriedades de `animação` às regras de estilo, como você fez acima. Sempre verifique se `animation-name` corresponde ao nome da animação que você deseja usar.

--- /hint ---

--- hint ---

Você pode adicionar o efeito `hover` diretamente ao menu `nav` assim:

```css
  nav ul li a:hover {
    animation-name: rainbowGlow;
    animation-duration: 1.5s;
    animation-iteration-count: infinite;
  }
```

Ou, se você também quiser criar outros links em seu site com as cores do arco-íris, adicione a animação a classe `.niceLinks`, assim:

```css
  .niceLinks:hover {
    color: #00BFFF;
    animation-name: rainbowGlow;
    animation-duration: 1.5s;
    animation-iteration-count: infinite;
  }
```

--- /hint ---

--- /hints ---

--- /challenge ---

![](images/badge-footer-image-html-intermed.png)


***
Este projeto foi traduzido por voluntários:

Lucas Pereira Santos

Douglas Reis

Graças a voluntários, podemos dar às pessoas de todo o mundo a chance de aprender em seu próprio idioma. Você pode nos ajudar a alcançar mais pessoas oferecendo-se para traduzir - mais informações em rpf.io/translate.