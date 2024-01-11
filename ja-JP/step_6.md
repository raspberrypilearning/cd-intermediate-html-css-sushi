## 個別のスタイル

Let's jazz up the home page a bit! 別の種類のCSSセレクタを使用すると、**1つの特定の要素**のみに一意のCSSルールのセットを適用できます。

+ `index.html`に移動して段落(`p`)要素を探します。段落がない場合は要素を追加します。 次の**属性**をタグに追加します。

```html
    <p id="myCoolText">
        My website is about Ireland.
    </p> 
```

`id`は、特定の要素を**指定**するための名前です。 ページ上の2つの要素が同じ`id`を持つことはできません。

+ スタイルシートに移動し、次のコードを追加します。

```css
    #myCoolText {
        color: #003366;
        border: 2px ridge #ccffff;
        padding: 15px;
        text-align: center;
    }
```

テキストは次のようになります。

![異なる色のテキストと境界線](images/paragraphIdStyle.png)

前に`#`が付いているセレクタは、Webサイト上の特定の要素にCSSルールを適用するために使用されます。 要素の`id`属性に割り当てた名前を使用して、要素を指定します。

+ ホーム・ページの`body`に対して1つ実行します。 `index.html`に移動し、`body`タグに`id`を追加します。

```html
    <body id="frontPage">
```

+ スタイルシートで、次のCSSルールを追加します。

```css
    #frontPage {
        background: #48D1CC;
        background: linear-gradient(#fea3aa, #f8b88b, #faf884, #baed91, #baed91, #b2cefe, #f2a2e8, #fea3aa);
    }
```

次のようなものが表示されます。

![レインボーグラデーション背景](images/frontPageIdStyles.png)

**gradient**を使いました! ある色が別の色にまざりこむ効果に付けられた名前です。 注:グラデーションの上にある最初の`background`プロパティは、グラデーションをサポートしていないブラウザの既定の色を決定します。

コードを完璧に入力して、上記のような美しい虹の効果が得られなかった場合、ブラウザーがグラデーションをサポートしていない可能性があります。

グラデーションを使用すると、さまざまな効果を作成できます。 詳細については、[ここ](http://dojo.soy/html2-css-gradients){:target="_blank"}を参照してください。

\--- challenge \---

## Challenge: いくつかの要素をスタイル設定する

+ 別の要素に`id`を指定し、上記のように`#`を持つIDセレクタを使用して、その要素のスタイルを設定します。 1枚の写真を`100%`の`border-radius`にして、完全に丸くするのはどうですか? Webサイト上の他の画像はすべて同じのままになります。 

\--- hints \---

\--- hint \---

要素に`id`を指定するには、次のように`id`属性をHTMLタグに追加します。

```html
  <img src="tito.png" id="titoPicture" alt="Tito the dog" />        
```

任意の`id`名を選択します。

\--- /hint \---

\--- hint \---

特定の要素のスタイルルールを定義するには、`#`記号と、`id`として要素に付けた名前を使用します。

```css
  #titoPicture {
    border-radius: 100%;
  }
```

注:CSSルールの前に入力する名前は、要素の`id`属性に入力した名前と**正確に**一致する必要があります。

\--- /ヒント \---

\--- /hints \---

![白い縁取りのティトの丸い絵](images/titoPictureIdStyle.png)

\--- /challenge \---