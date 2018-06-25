## テーマをデザインする

`セクション` や `p` ような要素のCSSルールを書くことは素晴らしいですが、それらのいくつかを他のものと見た目を変えたい場合はどうすればいいでしょうか？ このカードでは、同じタイプの要素にさまざまなスタイルルールを適用し、ウェブサイトの各ページごとに異なるテーマを作成する方法を学習します。

+ あなたのスタイルシートファイルに移動して、以下を追加してください - ドットを必ず先頭に入れてください！

```css
  .topDivider {border-top-style：solid; border-top-width：2px;ボーダートップカラー：＃F5FFFA;パディングボトム：10px; }
```

+ 今度は `tourism.html` （または独自のプロジェクトを使用している場合は作業中のHTMLファイル）に移動し、次の **属性** を各 `セクション` タグに追加します。

```html
  <section class="topDivider">
```

ページの各セクションの上に線が現れるはずです。 おめでとうございます-あなたは自分の最初の使用してきた **CSSクラス**！

![セクション間に行があるページ](images/sectionsWithTopBorder.png)

+ あなたのウェブページがどのように見えるかを見て、セクション</code> 要素が `ある他のページと比較してください。 <code>class = "topDivider"` という属性を追加したものだけが一番上に表示されます。

## \---崩壊\---

## タイトル：どのように機能するのですか？

ことを覚えていますが、CSSを使用する場合 **セレクタ** のような `項` または `のp` または `のnav ulの`、スタイルのルールが適用さ **すべて** あなたのウェブサイト上でそのタイプの要素を。

CSS **クラス**では、要素のうち</strong> うちの ****だけのスタイルを変更することができます。

あなたのセレクタの前にドットを置くことに、それを作る **クラスセレクタ**。 クラスは任意の名前を持つことができるので、HTML要素の名前である必要はありません。 例えば：

```css
  .myAwesomeClass {/ *私のクールなスタイルのルールはここにある* /}
```

スタイルルールが適用された要素を選択するには、[追加 `クラス` **属性** 、属性の値として、クラスの名前を入れて：HTMLコードでそれらの要素に **なし** のように、ドットを：

```html
  class = "myAwesomeClass"
```

\--- /崩壊\---

+ 別のクラスを試す準備ができていますか？ 次のCSSコードを `styles.cssに追加します`：

```css
  .stylishBox {背景色：＃87CEFA;色：＃A52A2A; border-style：solid; border-width：2px; border-color：＃F5FFFA; border-radius：10px; }
```

+ 次に、あなたのウェブサイトの別のページで、そこのいくつかの要素にクラスを追加します。 私はこれを次のように私のウェブサイトのFoodページの `セクション` 要素に追加します： `<section class="stylishBox">`。

それは素晴らしそうに見えますが、私のセクションはすべて一緒に押しつぶされています。

![ニースの見ているセクションは一緒に潰れた](images/squashedSections.png)

要素には、好きなだけ多くのCSSクラスを適用できます。 `クラス` 属性（ドットなしで覚えておいてください）内で使用したいすべてのクラスの名前をスペースで区切って記述してください。

+ セクションにいくつかのマージンとパディングを与える別のCSSクラスを作ってみましょう。 `styles.css` ファイルで、次のCSSクラスを作成します。

```css
  .someSpacing {パディング：10px; margin-top：20px; }
```

+ `html` コードで、次のように、作業していた各要素に新しいクラスを追加します。

```html
  <section class="stylishBox someSpacing">
```

![マージンとパディングが追加されたセクション](images/sectionsWithSpacing.png)

だから、CSSクラスを使用すると、聞かせて **選択** スタイルにどの要素、そして、彼らはあなたが聞かせて **リユース** あなたが望む任意の要素のスタイル規則の同じセットを。

+ `index.html` 移動し、 `stylishBox` クラスを `メイン` 要素またはページの別の要素に追加します。 後でもう一度取り除くことができます！

```html
    <main class="stylishBox">   
```

私のホームページはCSSクラスのように見えます。 私はTitoの写真で `img` タグに `topDivider` クラスを追加しました。

![ホームページで使用されているCSSクラス](images/homePageWithClasses.png)

\---挑戦\---

## 課題：新しいクラスを作る

+ CSSを使って **クラス** 例えば、あなたのウェブサイトのために、いくつかの異なる画像のサイズを定義するために `.smallPictures` 及び `.mediumPictures`。 その後、削除 `幅` あなたのそれぞれから属性を `IMG` 要素を、代わりに適切なクラスを追加します。

- - ヒント - -

\---ヒント\---

このような要素の幅だけを定義するCSSクラスを作ることができます：

```css
  .smallPictures {width：100px; }
```

\--- /ヒント\---

\---ヒント\---

ここにあります `のimg` とタグ `幅` 属性：

```html
  <img src="tito.png" alt="Tito the dog" width="100px" />       
```

`幅` 属性を削除し、CSSクラスを使用してサイズを制御すると、次のようになります。

```html
  <img src="tito.png" class="smallPictures" alt="Tito the dog" />       
```

By using a CSS class, you can easily change the width of all the pictures at once by changing only one line of code in your style sheet!

\--- /ヒント\---

- - /ヒント - -

\--- /チャレンジ\---