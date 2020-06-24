## Organizando sua página

Até agora você usou **títulos** e **parágrafos** para fazer com que seu **conteúdo** pareça organizado e fácil de ler. Vamos torná-lo ainda mais organizado agrupando as coisas.

## \--- collapse \---

## title: O que é conteúdo?

**Conteúdo** são todas as coisas na sua página da web, tais texto e imagens.

\--- /collapse \---

+ Vá para o arquivo `attractions.html` (ou uma de suas próprias páginas, se você não estiver usando o projeto de exemplo) e, próximo a parte superior, logo **abaixo** da tag abrindo `<main>`, digite isso em uma nova linha: 

```html
  <main>
    <article>
```

+ Se o seu editor adicionou automaticamente para você uma tag fechando `</article>`, exclua-a.

+ Na parte inferior do arquivo, logo **acima** da tag fechando `</main>`, adicione uma nova linha e feche o elemento `article`:

```html
    </article>
  </main>
```

Seu elemento `main` deve se parecer com isso agora (você pode ter conteúdos diferentes entre as tags `article`):

```html
  <main>
    <article>
      <h1>Meus lugares favoritos para ver na Irlanda</h1>
        <h2>Os Penhascos de Moher</h2>
        <p>
        Os Penhascos de Moher são encontrados no Condado de Clare, de onde eu sou. Olha como eles são legais!</p>
        <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
        <h2>Ilha Achill</h2>
        <p>Esta é uma grande ilha na costa do Condado de Mayo. Tem uma paisagem
        selvagem e bonita de montanhas, pântanos e penhascos.
        </p>
        <img src="achill.JPG" width="200px" />
    </article>
  </main>
```

+ Agora veja o conteúdo do seu `article` e tente dividi-lo em seções. Coloque esse novo par de tags em torno de cada parte: `<section></section>`. Aqui está um exemplo de como ele pode ficar:

```html
  <article>
    <h1>Meus lugares favoritos para ver na Irlanda</h1>
      <section>
        <h2>Os Penhascos de Moher</h2>
        <p>
        Os Penhascos de Moher são encontrados no Condado de Clare, de onde eu sou. Olha como eles são legais!</p>
      <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
    </section>
    <section>
      <h2>Ilha Achill</h2>
      <p>Esta é uma grande ilha na costa do Condado de Mayo. Tem uma paisagem
        selvagem e bonita de montanhas, pântanos e penhascos.
      </p>
      <img src="achill.JPG" width="200px" />
    </section>
  </article>
```

## \--- collapse \---

## title: Sobre o que são as novas tags?

Pense nesses novos elementos como **contêineres**. Eles estão usados para agrupar as coisas. É um pouco parecido como organizar coisas em caixas e prateleiras em sua casa!

Isso torna seu site compatível com os leitores de tela, oferece mais controle sobre o layout, e, como você verá, permite que você seja realmente criativo com o estilo.

Qualquer coisa pode entrar entre as tags. Geralmente será mais de um elemento, mas não tem que ser. Podem ser elementos HTML de qualquer tipo. O que você está fazendo é dizer ao navegador que tudo entre essas tags deve ficar junto.

### Article

O elemento `article` é um bloco para todo um conteúdo, neste caso um conjunto de informações sobre atrações na Irlanda. Se você tiver diferentes partes do conteúdo que não estão relacionadas, coloque cada uma em seu próprio elemento `article` em vez de colocar um conjunto de tags em todo o lote.

### Section

O elemento `section` permite dividir o conteúdo relacionado em partes menores e colocar cada parte no seu próprio contêiner.

### Existem outros mais!

Esses não são os únicos elementos do contêiner em HTML. Se você já criou um menu e o coloca entre tags `<nav> </nav>`, esse é outro exemplo de um tipo de contêiner. Também são `<main> </main>` e `<header> </header>` — você consegue pensar em algo mais?

\--- /collapse \---

\--- challenge \---

Sua página web pode não parecer diferente ainda, mas depois que o conteúdo for organizado em tags de contêiner, você poderá fazer algumas coisas legais com CSS. Lembre-se, o HTML controla como o site é organizado e o CSS controla a aparência.

## Desafio: organize seu site

+ Tente organizar todo o conteúdo do seu site usando os elementos `article` e `section` dessa maneira. 

\--- hints \---

\--- hint \---

Veja a página Comida do projeto de exemplo. Você verá que adicionei um `article` com um monte de tags `section` no arquivo `food.html`:

```html
  <main>
    <article>
      <h1>Alimentos na Irlanda</h1>
      <p>
        Estas são algumas das minhas comidas irlandesas favoritas!
      </p>  
      <section>
        <h2>Tradicional café da manhã Irlandês</h2>
        <p>
          Um café da manhã "Irlandês Completo" consiste em salsichas, fatias de toucinho (bacon),
          ovos, pudim preto, pudim branco e torradas.
        </p>
        <p>
          Geralmente haverá um tomate grelhado, acompanhado de cogumelos,
          e feijões cozidos.
        </p>
        <p>
          E claro, o café da manhã não está completo sem um lindo bule 
          de chá!
        </p>
      </section>

      <section>
        <h2>Bangers e Mash</h2>
        <p>
          Este clássico de salsichas, purê de batata e molho não é
          único na Irlanda,  o que o torna especial são as
          salsichas irlandesas. A maioria dos países tem sua própria maneira de fazer salsichas,
          e é uma coisa que sinto falta de casa se estiver viajando!
        </p>
      </section>

      <section>
        <h2>Bacon e Repolho</h2>
        <p>
          Eu não poderia fazer uma lista de comida irlandesa sem incluir
          este prato muito tradicional!
        </p>
        <p>
          Pode não parecer muito interessante, mas esta refeição saudável de
          presunto cozido, batata e repolho verde é saborosa e recheada.
          Eu amo refogar as batatas na manteiga, e eu também como um
          pouco de mostarda com o bacon.
        </p>
        <p>
          Minha mãe sempre fez esse prato mais especial ao cozinhar o repolho na
          água em que o presunto foi cozido.
        </p>
        <p>
          Se houver sobras, você pode fazer outro dos meus
          favoritos: <strong>repolho frito</strong>!
        </p>
      </section>
    </article>     
  </main>
```

\--- /hint \---

\--- /hints \---

No próximo cartão, você criará um tema diferente para cada página organizada em artigos e seções!

\--- /challenge \---