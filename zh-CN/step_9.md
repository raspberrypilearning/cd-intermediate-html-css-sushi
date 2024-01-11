## 动画

你知道你可以使用 CSS 来移动东西吗？ 您将学习如何使用此卡！

+ 在您开始之前， 请确保您网站上有一张图片，上面有一个 `id` 和一个相应的 CSS 块，它将`width` 设置为 `100px`。 我要用以前的Tito的图片，我的CSS块如下所示：

```css
    #titoPicture {
        border-radius: 100%;
        width: 100px;
    }
```

+ 转到CSS文件的底部，然后添加以下代码：

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

此代码创建了一个名为 `myFirstAnimation` 的动画，您可以添加到您网站上的任何元素。 你认为他会怎样做？

+ 查找图片的 CSS 规则并添加以下三个属性：

```css
    animation-name: myFirstAnimation;
    animation-duration: 2s;
    animation-iteration-count: 1;
```

+ 现在看看您网页上发生的事情！ 为` animation-iteration-count` 尝试不同的值，看看它做什么。

+ 让我们尝试另一个动画！ 将以下代码添加到CSS文件的末尾：

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

+ 现在找到更早的`#myCoolText` CSS 规则并添加到动画代码中：

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

当您使用**百分比值**，而不是`从`和`到`时，您可以在值之间以及刚刚开始和结束值之间设定。 您可以在两个值之间设置像您喜欢使用`0`的不同百分比值一样多。直到`100`。

+ 更改` animation-iteration-count`的值到`无限` 。 测试之前，看看是否可以猜测会发生什么！

+ 试用不同的数值为 `animation-duration`，以加速或减缓您的动画。

+ 最后一招！ 添加此动画代码：

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

+ 现在找到您先前写过的 `#frontPage` CSS 规则，并将其更改为:

```css
    #frontPage {
        background: repeating-linear-gradient(-45deg, red 0%, yellow 7.14%, lime 14.28%, cyan 21.42%, cyan 28.56%, blue 35.7%, magenta 42.84%, red 50%);
        background-size: 600vw 600vw;
        animation: slide 10s infinite linear forwards;
    }
```

不用担心理解上面的所有代码... 只是坐下来享受！

要了解更多的动画，请访问[这个网页](http://dojo.soy/html2-css-animation){:target="_blank"}。 享受快乐

在下一张卡片上，当鼠标光标悬停在鼠标上时，你会学习如何使事情变得很酷！