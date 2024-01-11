## ページを整理する

これまで**見出し**と**段落**を使用して、**コンテンツ**を整理して読みやすくしました。 物事をまとめてまとめることで、さらに整理してみましょう。

## \--- collapse \---

## タイトル：Contentとは何ですか？

**content**は、あなたのウェブページのすべてのもの、例えばastextやpicturesです。

\--- /collapse \---

+ ` attractions.html` ファイル（またはサンプルプロジェクトを使用していない場合は自分のページの1つ）に移動し、上部にある openingタグの**下**で、新しい行に次のように入力します。 

```html
  <main>
    <article>
```

+ エディタが閉じる`</article>`タグに自動的に追加された場合は、削除してください。

+ ファイルの一番下にある**上記**閉じる`</main>`タグ、新しい行を追加し、`記事`要素を閉じます。

```html
    </article>
  </main>
```

`main`要素は以下のようになります。（もちろん、`article`タグの間に異なるコンテンツがあるかもしれません）：

```html
  <main>
    <article>
      <h1>My favourite places to see in Ireland</h1>
        <h2>The Cliffs of Moher</h2>
        <p>
        The Cliffs of Moher are found in County Clare, where I am from. Look how cool they are!</p>
        <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
        <h2>Achill Island</h2>
        <p>This is a large island off the coast of County Mayo. 山や沼、崖などの自然豊かな景観が美しい。
        </p>
        <img src="achill.JPG" width="200px" />
    </article>
  </main>
```

+ 次に、`article`の内容を見て、セクションに分けてみてください。 この新しいタグのペアを各ビットの周りに配置します：`<section> </section>` 。 次のようになります。

```html
  <article>
    <h1>My favourite places to see in Ireland</h1>
    <section>
      <h2>The Cliffs of Moher</h2>
      <p>
      The Cliffs of Moher are found in County Clare, where I am from. Look how cool they are!</p>
      <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
    </section>
    <section>
      <h2>Achill Island</h2>
      <p>This is a large island off the coast of County Mayo. 山や沼、崖などの自然豊かな景観が美しい。
      </p>
      <img src="achill.JPG" width="200px" />
    </section>
  </article>
```

## \--- collapse \---

## タイトル：新しいタグとは何ですか？

これらの新しい要素を**containers**と考えてください。 それらは、物事をグループ化するために使用されます。 まるで家の箱や棚に物を整理するようなものです。

これにより、ウェブサイトがスクリーンリーダーにとって使いやすくなり、レイアウトをより細かく制御できるようになります。また、おわかりのように、スタイリングを使って本当にクリエイティブになることができます。

タグの間に何でも入れることができます。 通常は複数の要素になりますが、そうである必要はありません。 任意の種類のHTML要素にすることができます。 あなたがやっていることは、これらのタグの間にあるすべてが一緒に属していることをブラウザに伝えることです。

### Article

`article`要素は、コンテンツ全体のコンテナであり、この場合、アイルランドのアトラクションに関する情報のセットです。 関連のないさまざまなコンテンツがある場合は、全体に一つのタグセットを置くのではなく、それぞれを独自の`article`要素に入れる必要があります。

### Section

`section`要素では、関連するコンテンツを小さなチャンクに分割し、それぞれのチャンクをそれぞれのコンテナに入れることができます。

### 他の要素にも存在する！

これらは、HTMLの唯一のコンテナー要素ではありません。 メニューを作成し、`<nav> </nav>` タグの間に入れたことがある場合は、コンテナのタイプのもう一つの例です。 `<main></main>`と`<header></header>`も——これ以上考えられますか？

\--- /collapse \---

\--- challenge \---

Webページの外観はまだ変わらないかもしれませんが、コンテンツがコンテナータグに整理されると、CSSを使用していくつかの素晴らしいことができるようになります。 HTMLはWebサイトの編成方法を制御し、CSSはWebサイトの外観を制御します。

## チャレンジ：ウェブサイトを整理する

+ `article`と`section`コンテナを使用して、ウェブサイト上のすべてのコンテンツを整理してください。 

\--- hints \---

\--- hint \---

サンプルプロジェクトのフードページを見てください。 `food.html`ファイルに`section`タグの束を付けた`article`を追加しました。

```html
  <main>
    <article>
      <h1>Food in Ireland</h1>
      <p>
        These are some of my favourite Irish foods!
      </p>  
      <section>
        <h2>Traditional Irish Breakfast</h2>
        <p>
          A "Full Irish" breakfast consists of sausages, rashers (bacon),
          eggs, black pudding, white pudding and toast.
        </p>
        <p>
          Often there will be a grilled tomato as well as mushrooms,
          and baked beans.
        </p>
        <p>
          And of course, no breakfast is complete without a lovely pot 
          of tea!
        </p>
      </section>

      <section>
        <h2>Bangers and Mash</h2>
        <p>
          This classic of sausages, mashed potato and gravy is not
          unique to Ireland, but what makes it special is the Irish
          sausages. ほとんどの国には独自のソーセージの作り方がありますが、それは私が旅行に出かけているときに家から懐かしくなるものです!
        </p>
      </section>

      <section>
        <h2>Bacon and Cabbage</h2>
        <p>
          I couldn't possibly make a list of Irish food without including
          this very traditional dish!
        </p>
        <p>
          It might not sound very interesting, but this hearty meal of
          boiled ham, potatoes and green cabbage is tasty and filling.
          ジャガイモをバターでくすぶるのが好きで、ベーコンにからしを少しつけるのも好きです。
        </p>
        <p>
          My mum always made it extra special by cooking the cabbage in
          the water that the ham was boiled in.
        </p>
        <p>
          If there are any leftovers you can make another one of my
          favourites: <strong>fried cabbage</strong>!
        </p>
      </section>
    </article>     
  </main>
```

\--- /hint \---

\--- /hints \---

次のカードでは、articlesやsectionsに整理されたページごとに異なるテーマをデザインしましょう!

\--- /challenge \---