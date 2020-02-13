## الرسوم المتحركة

هل تعلم أنه يمكنك استخدام CSS لجعل الاشياء تتحرك؟ سوف تتعلم كيف في هذه البطاقة!

+ قبل أن تبدأ، تأكد من أن لديك صورة على موقع الويب الخاص بك مع معرف `id` وكتلة CSS المقابلة لها والتي تحدد العرض `width` إلى `100 بكسل`. سأستحدم صورة تيتو التي استخدمناها سابقاً، وكتلة CSS الخاصة بي تشبه التالي:

```css
    #titoPicture {
        border-radius: 100%;
        width: 100px;
    }
```

+ انتقل إلى أسفل ملف CSS وأضف الكود التالي:

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

يقوم هذا الرمز بإنشاء رسم متحرك يسمى `myFirstAnimation` الذي يمكنك إضافته إلى أي عنصر على موقع الويب الخاص بك. ما الذي تظن أنه سيفعل؟

+ ابحث عن قواعد CSS للصورة وأضف الخصائص الثلاثة التالية:

```css
    animation-name: myFirstAnimation;
    animation-duration: 2s;
    animation-iteration-count: 1;
```

+ والآن شاهد ما يحدث على صفحة الويب الخاصة بك! جرب قيمًا مختلفة للمتغير `animation-iteration-count` لنرى ماذا يفعل.

+ لنجرب رسوم متحركة أخرى! أضف الكود التالي إلى نهاية ملف CSS الخاص بك:

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

+ الآن ابحث عن `#myCoolText` في قواعد CSS التي استخدمتها سابقاً وإضف التعليمات البرمجية الخاصة بالحركة:

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

عند استخدام قيم **النسبة المئوية** بدلاً من `من` و `إلى`، ستتمكن من ضبط القيم الفاصلة وكذلك قيم البداية والنهاية. يمكنك تعيين العديد من القيم الفاصلة بين ما تريد باستخدام قيم النسبة المئوية المختلفة من `0` حتى `100`.

+ قم بتغيير قيمة `animation-iteration-count` إلى لا نهائية `infinite`. أنظر إذا ما كان يمكنك تخمين ما سيحدث قبل اختباره!

+ جرب قيمًا مختلفة لـ `animation-duration` لتسريع أو إبطاء الرسوم المتحركة الخاصة بك.

+ خدعة أخيرة! أضف هذه التعليمات البرمجية للرسوم المتحركة:

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

+ الآن يمكنك العثور على قواعد CSS `#frontPage` التي كتبتها سابقًا وتغييرها إلى:

```css
    #frontPage {
        background: repeating-linear-gradient(-45deg, red 0%, yellow 7.14%, lime 14.28%, cyan 21.42%, cyan 28.56%, blue 35.7%, magenta 42.84%, red 50%);
        background-size: 600vw 600vw;
        animation: slide 10s infinite linear forwards;
    }
```

لا تقلق بشأن فهم كل الكود الذي قمت بلصقه للتو... فقط اجلس وتمتع بها!!

لمعرفة المزيد من الأشياء التي يمكنك القيام بها باستخدام الرسوم المتحركة، تفضل بزيارة [صفحة الويب هذه](http://dojo.soy/html2-css-animation){:target="_blank"}. إستمتع!

على البطاقة التالية، ستتعلم كيفية جعل الأشياء الرائعة تحدث عندما تحوم مؤشر الماوس فوق الأشياء!