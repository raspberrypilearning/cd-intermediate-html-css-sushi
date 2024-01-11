## アニメーション

CSSを使って表示物を動かすことができることを知っていましたか? このカードでその方法を学びます！

+ 作業を開始する前に、`id`が付いた画像と、`width`を`100px`に設定した`id`が一致するCSSブロックをWebサイトに用意してください。 以前のティートの画像を使用しますが、CSSブロックは以下のようになります。

```css
    #titoPicture {
        border-radius: 100%;
        width: 100px;
    }
```

+ CSSファイルの一番下に移動し、次のコードを追加します。

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

このコードは `myFirstAnimation` というアニメーションを作成し、ウェブサイト上の任意の要素に追加できます。 どうすると思う?

+ 画像のCSSルールを見つけて、次の3つのプロパティを追加します。

```css
    animation-name: myFirstAnimation;
    animation-duration: 2s;
    animation-iteration-count: 1;
```

+ Webページで何が起こるか見てみましょう！ `animation-iteration-count`に別の値を試してください。

+ 別のアニメーションを試してみましょう！ CSS ファイルの最後に次のコードを追加しましょう:

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

+ 以前の`#myCoolText`というCSSルールを見つけて、アニメーションコードを追加してください。

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

`from`と`to`の代わりに**percentage values**を使用する場合、開始値と終了値だけでなく、中間の値も設定できます。 `0`から`100`まで異なるパーセント値を使用して、好きなように幾らの中間値を設定できます。

+ `animation-iteration-count`の値を`infinite`に変更します。 確認する前に、何が起こるかを推測してください。

+ `animation-duration`に異なる値を設定して、アニメーションの速度を上げたり下げたりしてみてください。

+ 最後のトリック！ 次のアニメーションコードを追加します。

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

+ ここでは、以前に書いた`#frontPage`のCSSルールを見つけて、次のように変更します:

```css
    #frontPage {
        background: repeating-linear-gradient(-45deg, red 0%, yellow 7.14%, lime 14.28%, cyan 21.42%, cyan 28.56%, blue 35.7%, magenta 42.84%, red 50%);
        background-size: 600vw 600vw;
        animation: slide 10s infinite linear forwards;
    }
```

上記のコードをすべて理解する必要はありません。 ただ座って楽しんでください!!

アニメーションでできることの詳細については、[このWebページにアクセスしてください](http://dojo.soy/html2-css-animation) {：target = "_ blank"}。 楽しんで!

次のカードでは、マウスカーソルを物の上に置いたときにクールなことが起こるようにする方法を学びます。