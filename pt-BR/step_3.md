## Todas as cores!

Como você já viu antes, é possível digitar muitos nomes de cores diferentes como palavras, e o navegador as reconhecerá. Mas, uma maneira mais comum de definir cores é usar algo chamado **códigos hexadecimais** ('hex' é a abreviação para **hexadecimal**, uma forma especial de contagem).

+ Dê uma olhada na sua **folha de estilo**. Esse é o arquivo que tem `.css` no nome.

+ Dentro das regras CSS para o `body`, defina a cor do plano de fundo com o código hexadecimal `#7B68EE`:

```html
  background-color: #7B68EE;
```

Nota: Se você estiver usando um Mac, poderá digitar `#` pressionando as teclas <kbd>alt</kbd> e <kbd>3</kbd> ao mesmo tempo.

Agora seu site deve ter um fundo roxo.

![](images/HexColourFirst.png) ![](images/HexColourFirstResult.png)

+ Você não é um fã de roxo? Vá para [esta página da web](http://dojo.soy/html2-colors){:target="_blank"} e escolha outra cor para sua folha de estilos - em vez de digitar o nome da cor, digite o código hexadecimal. 

![](images/ColorNamesHex.png)

Os códigos de cores permitem criar qualquer cor, mesmo que não esteja em nenhuma lista de nomes de cores.

+ Tente criar seu próprio código de cores. Ele deve começar com um `#`. Isso informa ao navegador que é um código hexadecimal em vez de um nome de cor. O restante do código é composto por seis caracteres. Eles podem ser qualquer número de **0 a 9** e qualquer letra de **A a F**.

--- collapse ---
---
title: Como isso funciona?
---

Cada cor é feita misturando diferentes quantidades de **vermelho**, **verde** e **azul**. Às vezes você verá isso escrito como **RGB**. Cada uma dessas cores é representada por dois dos seis dígitos no seu código HEX. `00` é o mínimo, e `FF` é o máximo.

**Hexadecimal** é uma forma reduzida de escrever os números usando letras de A a F e dígitos. O número `255` é escrito como `FF` em hexadecimal. Você não precisa se preocupar em aprender a contar com números hexadecimais. Em vez disso, experimente diferentes códigos hexadecimais para se acostumar a usá-los.

+ Aqui estão algumas cores básicas para experimentar no seu site. Tente colocar números menores em vez de `FF` para ver como os tons mudam.

|      | R  | G  | B  |   Resultado    |
| ---- | -- | -- | -- |:--------------:|
| \# | FF | 00 | 00 |    Vermelho    |
| \# | 00 | FF | 00 |     Verde      |
| \# | 00 | 00 | FF |      Azul      |
| \# | FF | FF | 00 |    Amarelo     |
| \# | FF | 00 | FF |    Magenta     |
| \# | 00 | FF | FF |     Ciano      |
| \# | FF | 8c | 00 | Laranja escuro |

--- /collapse ---

Misturar a cor perfeita pode exigir muitos experimentos. Felizmente, existem muitas ferramentas de seleção de cores online que podem te ajudar a obter o código hexadecimal de qualquer cor desejada.

![](images/W3ColorPicker.png)

+ Experimente [este seletor de cores](http://dojo.soy/html2-color-picker){:target="_blank"} para escolher alguns códigos de cores hexadecimais para usar nos demais estilos do seu site.