## ティートに寝返りを教えろ!

マウスカーソルを物の上に置いたときにクールなことが起こるようにすることで、Webサイトをより**インタラクティブ**にすることができます!

+ `img` 要素のCSSルールを探したり、ない場合は作成してください。 境界線を追加し、その下に新しい規則のブロックを追加します。

```css
  img { border: 2px solid White; } img:hover { border: 2px dashed Navy; }
```

あなたは **擬似クラス**と呼ばれる特別なタイプのCSSブロックを使用しました。

## \--- collapse \---

## title:どのように動作するのか?

**擬似クラス** は、自分で作成した **クラス** とは少し異なります。 `:`で認識できます。

疑似クラスはHTML要素に組み込まれています。HTMLコードに何も追加しなくても、スタイルシートの任意の要素、クラス、または`id`セレクタに`:hover`スタイルルールを追加できます。

\--- /collapse \---

+ どうなると思いますか? Webサイトのどのページに画像があるかを確認し(画像がない場合は画像を追加)、画像の上にカーソルを移動して確認します。

+ この新しい`:hover`疑似クラスをCSSクラスとともに使用して、リンク上にマウスを置いたときにリンクが光るようにしましょう。 Webページへのリンクを追加し、クラス名を指定する属性を含めます。 リンクは、次のように`<a>`タグを使用して定義されます。

```html
    <p>
      Visit the <a class="niceLinks" href="https://en.wikipedia.org/wiki/Ireland">Wikipedia page</a> to learn even more about Ireland!
    </p>
```

+ 次のコードをスタイル・シートに追加し、コードを実行してリンクの動作を確認します。

```css
  .niceLinks {テキスト装飾：なし;色：＃FFFAF0; } .niceLinks：ホバー{色：＃00FF7F; }
```

+ メニュー・バーのすべてのリンクにも、属性`class="niceLinks"`を追加します。

これらのトリックをアニメーションと組み合わせることもできます。

+ Titoの画像のCSSブロックをもう一度探します(あるいは、前に作業していた画像を探します)。 スタイルシートファイルに次のコードを追加します。

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

+ どうなるかわかりますか?

+ 画像の上にカーソルを移動させながら、「Roll over!」と叫びます。

\--- challenge \---

## Challenge：輝く虹のリンクを作る

+ 前のカードの`rainbowGlow`アニメーションを使用して、メニュー内のリンクの上にカーソルを置いたときにリンクの色を変更し続けることができますか。

\--- hints \---

\--- hint \---

`rainbowGlow`アニメーションのコードを以下に示します。 5つのステージが定義されており、各ステージで異なるテキスト色を設定します。 追加や変更は自由自在!

```css
    @keyframes rainbowGlow {0％{カラー：＃00BFFF; } 25％{カラー：＃00FF7F; } 50％{カラー：#eeeeaf; } 75％{color：#eeafee; } 100％{カラー：＃00BFFF; }}
```

\--- /hint \---

\--- hint \---

何かをアニメートするには、上記と同様に、スタイルルールに3つの`animation`プロパティを追加します。 `animation-name`が、使用するアニメーションの名前と一致していることを必ず確認してください。

\--- /hint \---

\--- hint \---

`hover`エフェクトは、次のように`nav`メニューに直接追加できます。

```css
  nav ul li：hover {アニメーション名：rainbowGlow;アニメーションの持続時間：1.5秒;アニメーション反復カウント：無限; }
```

また、Webサイト上の他のリンクをFlash虹色にする場合は、次のように`.niceLinks`クラスにアニメーションを追加することもできます。

```css
  .niceLinks：ホバー{色：＃00BFFF;アニメーション名：rainbowGlow;アニメーションの持続時間：1.5秒;アニメーション反復カウント：無限; }
```

\--- /hint \---

\--- /hints \---

\--- /challenge \---

![](images/badge-footer-image-html-intermed.png)