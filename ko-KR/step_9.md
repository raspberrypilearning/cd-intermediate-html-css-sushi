## 애니메이션

CSS를 사용하여 사물을 움직일 수 있다는 것을 알고 계셨습니까? 이 섹션에서 방법을 배우게 됩니다!

+ 시작하기 전에, 웹 사이트에 `id`와 `폭`이 `100px`로 설정된 해당 CSS 블록 사진이 있는 지 확인하세요. 저는 전에 썼던 Tito 사진으로 쓸 것 입니다. 저의 CSS 블록은 다음과 같습니다.

```css
    #titoPicture {
        border-radius: 100%;
        width: 100px;
    }
```

+ CSS 파일 하단으로 이동하여 다음 코드를 추가합니다.

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

이 코드는 웹 사이트의 모든 요소에 추가 할 수있는 `myFirstAnimation` 이라는 애니메이션을 만듭니다. 어떤 일이 일어날 것 같습니까?

+ 그림에 대한 CSS 규칙을 찾고 다음 세 가지 속성을 추가합니다.

```css
    animation-name: myFirstAnimation;
    animation-duration: 2s;
    animation-iteration-count: 1;
```

+ 이제 웹 페이지에서 무슨 일이 일어나는지보세요! `animation-iteration-count` 에 대해 다른 값을 시도하여 무슨일이 일어나는지 확인하십시오.

+ 또 다른 애니메이션을 시도해 봅시다! CSS 파일 스크립트의 끝에 다음 코드를 추가하십시오:

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

+ 이제 이전의 `#myCoolText` CSS 규칙을 찾아 애니메이션 코드를 추가합니다.

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

` from ` 과 ` to `대신 **퍼센트 값** 을 사용하면 시작 및 종료 값뿐 아니라 중간 값도 설정할 수 있습니다. `0` 에서 최대 `100`까지 다른 백분율 값을 사용하여 원하는만큼 중간 값을 설정할 수 있습니다.

+ `animation-iteration-count` 값을 `infinite`으로 설정하세요. 테스트하기 전에 어떤 일이 일어날 지 추측해 보세요!

+ 애니메이션 속도를 높이거나 낮추려면 `animation-duration` 에 대해 다른 값을 시도하십시오.

+ 마지막 트릭입니다! 이 애니메이션 코드를 추가하십시오.

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

+ 이제 이전에 작성한 `#frontPage` CSS 규칙을 찾아 다음과 같이 변경합니다.

```css
    #frontPage {
        background: repeating-linear-gradient(-45deg, red 0%, yellow 7.14%, lime 14.28%, cyan 21.42%, cyan 28.56%, blue 35.7%, magenta 42.84%, red 50%);
        background-size: 600vw 600vw;
        animation: slide 10s infinite linear forwards;
    }
```

위의 모든 코드를 이해해야 된다는 걱정은 하지 마세요... 그냥 보고 즐기세요!!

애니메이션으로 할 수있는 작업에 대해 자세히 알아 보려면 [이 웹 페이지](http://dojo.soy/html2-css-animation){: target = "_ blank"}를 방문하세요. 즐기세요!

다음 챕터에서는 마우스 커서를 어떤 곳 위로 가져갈 때 멋진 일이 일어나도록하는 방법을 배울 것 입니다!