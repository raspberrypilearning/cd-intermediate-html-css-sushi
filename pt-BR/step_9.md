## Animação

Você sabia que pode usar CSS para fazer as coisas se moverem? Você aprenderá como neste cartão!

+ Antes de começar, verifique se você tem uma foto no seu site com um `id` e um bloco CSS correspondente que define o `width` para `100px`. Vou usar a foto de Tito de antes, e meu bloco CSS fica assim:

```css
    #titoPicture {
        border-radius: 100%;
        width: 100px;
    }
```

+ Vá para a parte inferior do seu arquivo CSS e adicione o seguinte código:

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

Este código cria uma animação chamada `myFirstAnimation` que você pode adicionar a qualquer elemento do seu site. O que você acha que isso vai fazer?

+ Encontre suas regras CSS para a imagem e adicione as três propriedades a seguir:

```css
    animation-name: myFirstAnimation;
    animation-duration: 2s;
    animation-iteration-count: 1;
```

+ Agora observe o que acontece na sua página! Tente valores diferentes para `animation-iteration-count` para ver o que faz.

+ Vamos tentar outra animação! Adicione o seguinte código ao final do seu arquivo CSS:

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

+ Agora encontre o `#myCoolText` nas regras de CSS anteriores e adicione o código de animação:

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

Quando você usa **valores percentuais** ao invés de `from` e `to`, poderá definir valores intermediários como apenas valores iniciais e finais. Você pode definir quantos valores entre eles quiser usando diferentes valores percentuais de `0` até `100`.

+ Alterar o valor de `animation-iteration-count` para `infinite`. Veja se você consegue adivinhar o que acontecerá antes de testá-lo!

+ Experimente valores diferentes para `animation-duration` para acelerar ou desacelerar sua animação.

+ Um truque final! Adicione este código de animação:

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

+ Agora encontre o `#frontPage` nas regras CSS que você escreveu anteriormente e altere para:

```css
    #frontPage {
        background: repeating-linear-gradient(-45deg, red 0%, yellow 7.14%, lime 14.28%, cyan 21.42%, cyan 28.56%, blue 35.7%, magenta 42.84%, red 50%);
        background-size: 600vw 600vw;
        animation: slide 10s infinite linear forwards;
    }
```

Não se preocupe em entender todo o código acima... apenas sente-se e divirta-se!!

Para saber mais sobre o que você pode fazer com animação, visite [este site](http://dojo.soy/html2-css-animation){:target="_blank"}. Divirta-se!

No próximo cartão, você aprenderá como fazer coisas legais acontecerem quando passar o mouse sobre os elementos!