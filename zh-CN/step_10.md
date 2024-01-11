## 教 Tito 翻转！

您可以使您的网站更具互动性** **当您将鼠标悬停在事物上时，可以使事物变酷！

+ 查找`img`元素的 CSS 规则，或在您没有任何元素时创建一些规则。 添加一个边框，然后在下面添加一个新的规则块：

```css
  img {
    border: 2px solid White;
  }
  img:hover {
    border: 2px dashed Navy;
  }
```

您刚刚使用了一种特殊的CSS块，称为** 伪类 ** 。

## \--- collapse \---

## 标题：它是如何工作的？

一个 **伪类** 与您自己创建的 **class** 略有不同。 您可以通过`:`来识别它。

伪类被编入HTML元素: 你可以添加`:hover`样式规则到任何元素, 类, 或 `id` 选择器在您的样式表中无需添加额外的 HTML 代码。

\--- /collapse \---

+ 你觉得会发生什么？ 检查您网站上的哪些页面上有图片（如果没有图片，请添加图片！），然后将光标移到图片上查找！

+ 让我们使用这个新的 `:hover` 伪类和一个 CSS 类来在你悬停时显示链接！ 将链接添加到您的网页，并包含一个属性以指定类名称。 记住，链接使用`<a>`标签定义，如：

```html
    <p>
      Visit the <a class="niceLinks" href="https://en.wikipedia.org/wiki/Ireland">Wikipedia page</a> to learn even more about Ireland!
    </p>
```

+ 将以下代码添加到您的样式表中，然后运行您的代码来查看您的可爱链接。

```css
  .niceLinks {
    text-decoration: none;
    color: #FFFAF0;
  }
  .niceLinks:hover {
    color: #00FF7F;
  }
```

+ 为什么不将属性`class="niceLinks"`添加到菜单栏中的所有链接？

你也可以将所有这些技巧和动画结合起来！

+ 再次找到Tito图片的 CSS 块 (或您先前工作的任何图片)。 将以下代码添加到样式表文件中：

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

+ 你能猜会发生什么吗？

+ 现在大喊“翻滚！”当您将光标移到图片上时！

\--- challenge \---

## 挑战：建立发光的彩虹链接

+ 您是否可以使用上一张卡片中的`rainbowGlow`动画来使您菜单中的链接在鼠标悬停在它们上面时保持颜色变化？

\--- hints \---

\--- hint \---

下面是`rainbowGlow`动画的代码。 它定义了五个阶段，并且每个阶段都设置了不同的文本颜色。 您可以随意添加更多或更改他们！

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

\--- /hint \---

\--- hint \---

要制作动画，请添加三个`动画`属性，就像您在上面所做的一样。 始终确保`动画名称`与您要使用的动画名称匹配。

\--- /hint \---

\--- hint \---

您可以添加`悬停`直接影响` nav `像这样的菜单：

```css
  nav ul li a:hover {
    animation-name: rainbowGlow;
    animation-duration: 1.5s;
    animation-iteration-count: infinite;
  }
```

或者，如果您也想使网站上的其他链接也闪烁彩虹色，则可以将动画添加到`.niceLinks `类，就像这样：

```css
  .niceLinks:hover {
    color: #00BFFF;
    animation-name: rainbowGlow;
    animation-duration: 1.5s;
    animation-iteration-count: infinite;
  }
```

\--- /hint \---

\--- /hints \---

\--- /challenge \---

![](images/badge-footer-image-html-intermed.png)