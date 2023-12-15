## Tito가 롤오버하도록 가르쳐주세요!

마우스 커서로 물건을 가리킬 때 멋진 일이 발생하도록 해서 웹 사이트를 더욱 활성화 할 수 있습니다!

+ `img` 요소에 대한 CSS 규칙을 찾고, 규칙이 없는 경우 몇개의 규칙을 만듭니다. 테두리를 추가 한 다음 바로 아래에 새 규칙 블록을 추가합니다.

```css
  img {
    border: 2px solid White;
  }
  img:hover {
    border: 2px dashed Navy;
  }
```

방금 **pseudo-class** (가상 클래스) 라는 특수 유형의 CSS 블록을 사용했습니다.

## \--- collapse \---

## title: 어떻게 동작하나요?

**가상 클래스**는 직접 만든 **클래스**와 약간 다릅니다. 다음과 같이 구분할 수 있습니다: ``

가상 클래스는 HTML 요소에 내장되어 있습니다. HTML 코드에 추가 할 필요없이 스타일 시트의 모든 요소, 클래스 또는 `id` 선택기에 `:hover` 스타일 규칙을 추가 할 수 있습니다.

\--- /collapse \---

+ 어떤 일이 일어날 것 같습니까? 웹 사이트의 어떤 페이지에 사진이 있는지 확인한 다음 (사진이 없으면 사진을 추가하십시오!) 커서를 사진 위로 이동하여 알아보십시오!

+ 이 새로운 `:hover` 가상 클래스를 CSS 클래스와 함께 사용하여 링크 위로 마우스를 가져갈 때 링크가 빛나게 됩니다! 웹 페이지에 대한 링크를 추가하고 클래스 이름을 지정하는 속성을 포함하십시오. 다음과 같이 링크는 `<a>` 태그를 사용하여 정의된다는 것을 기억하세요:

```html
    <p>
      아일랜드에 대해 더 자세히 알아 보려면 <a class="niceLinks" href="https://en.wikipedia.org/wiki/Ireland">Wikipedia 페이지</a> 을 방문하십시오!
    </p>
```

+ 스타일 시트에 다음 코드를 추가 한 다음 코드를 실행하여 멋진 링크가 작동하는지 확인하십시오.

```css
  .niceLinks {
    text-decoration: none;
    color: #FFFAF0;
  }
  .niceLinks:hover {
    color: #00FF7F;
  }
```

+ 메뉴 모음의 모든 링크에도 `class="niceLinks"` 속성을 추가하는 것이 어때요?

이 모든 트릭을 애니메이션과 결합 할 수도 있습니다!

+ 다시 Tito의 그림 (또는 이전에 작업 한 그림 중 아무거나) 에 대한 CSS 블록을 찾습니다. 이제 자신만의 스타일 시트에 맞춰서 다음의 코드를 추가하십시오:

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

+ 무슨 일이 일어날 지 짐작할 수 있습니까?

+ 커서를 그림 위로 이동하면 "롤오버!" 라고 외치세요!

\--- challenge \---

## 과제: 빛나는 무지개 링크 만들기

+ 이전 카드의 `rainbowGlow` 애니메이션을 사용하여 커서가 위에있을 때 메뉴의 링크 색상이 계속 변경되도록 할 수 있습니까?

\--- hints \---

\--- hint \---

다음은 `rainbowGlow` 애니메이션의 코드입니다. 5 개의 단계가 정의되어 있으며 각 단계에서 다른 텍스트 색상을 설정합니다. 자신이 원하는대로 더 추가하거나 변경할 수 있습니다!

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

애니메이션을 적용하려면 위에서 한 것처럼 스타일 규칙에 `animation` 속성 3 개를 추가합니다. 항상 `animation-name` 이 사용하려는 애니메이션의 이름과 일치하는지 확인하십시오.

\--- /hint \---

\--- hint \---

다음과 같이 `hover` 효과를 `nav` 메뉴에 직접 추가 할 수 있습니다.

```css
  nav ul li a:hover {
    animation-name: rainbowGlow;
    animation-duration: 1.5s;
    animation-iteration-count: infinite;
  }
```

또는 웹 사이트의 다른 링크도 무지개색으로 깜박이게 하려면 다음과 같이 대신 `.niceLinks` 클래스에 애니메이션을 추가 할 수 있습니다:

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