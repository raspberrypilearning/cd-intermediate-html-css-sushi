## अ‍ॅनिमेशन

आपल्याला माहित आहे की आपण गोष्टी हलविण्यासाठी CSS वापरू शकता? आपण या कार्डवर कसे हे शिकणार!

+ आपण प्रारंभ करण्यापूर्वी, आपल्या वेबसाइटवर ` id` आपल्याकडे एक चित्र आणि संबंधित CSS ब्लॉक जो `width` सेट करतो ते `100px` असल्याची खात्री करा. मी पूर्वीपासून टिटोच्या चित्रासह जात आहे, आणि माझा CSS (सीएसएस) ब्लॉक असे दिसते:

```css
    #titoPicture {
        border-radius: 100%;
        width: 100px;
    }
```

+ आपल्या CSS फाईलच्या तळाशी जा आणि खालील कोड जोडा:

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

हा कोड `myFirstAnimation` नावाचा अ‍ॅनिमेशन तयार करतो जे आपण आपल्या वेबसाइटवरील कोणत्याही घटकास जोडू शकता. आपणास काय वाटते की ते काय करेल?

+ चित्रासाठी आपले CSS नियम शोधा आणि खालील तीन गुणधर्म जोडा:

```css
    animation-name: myFirstAnimation;
    animation-duration: 2s;
    animation-iteration-count: 1;
```

+ आता आपल्या वेब पृष्ठावर काय होते ते पहा! `animation-iteration-count` साठी भिन्न मूल्ये वापरून ते काय करते ते पहा.

+ चला आणखी एक अ‍ॅनिमेशन वापरुया! CSS फाईलमधे सघल्यात शेवटी हे खालील कोड जोडा:

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

+ आता पूर्वीचे CSS नियम `#myCoolText` शोधा आणि अ‍ॅनिमेशन कोडमध्ये जोडा:

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

जेहवा आपण `from` आणि `to` च्याऐवजी **percentage values** वापरता तेव्हा, आपण फक्त प्रारंभ आणि अंत मूल्ये मध्येच मूल्ये सेट करू शकता. आपण `0` पासून `100` पर्यंत जे तुम्हाला आवडतील ते भिन्न टक्केवारी मूल्ये अंतर्भूत मूल्ये म्हणून सेट करू शकता.

+ `animation-iteration-count` चे मूल्य `infinite` असे बदला. आपण चाचणी घेण्यापूर्वी काय होईल याचा अंदाज लावू शकता का ते पहा!

+ आपले अ‍ॅनिमेशन वेग किंवा कमी करण्यासाठी `animation-duration` ची भिन्न मूल्ये वापरून पहा.

+ एक अंतिम युक्ती! हा अ‍ॅनिमेशन कोड जोडा:

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

+ आता आपण आधी लिहिलेले CSS नियम `#frontPage` शोधा आणि त्यांना असे बदला:

```css
    #frontPage {
        background: repeating-linear-gradient(-45deg, red 0%, yellow 7.14%, lime 14.28%, cyan 21.42%, cyan 28.56%, blue 35.7%, magenta 42.84%, red 50%);
        background-size: 600vw 600vw;
        animation: slide 10s infinite linear forwards;
    }
```

वरील सर्व कोड समजून घेण्याची चिंता करू नका ... फक्त बसून आनंद घ्या!!

अ‍ॅनिमेशनसह आपण आणखी काय गोष्टी शकता हे जाणून घेण्यासाठी, [this web page](http://dojo.soy/html2-css-animation){:target="_blank"} वर जा. मजा करा!

पुढील कार्डावर तुम्ही शिकाल की आपण जेव्हा गोष्टींवर माउस कर्सर फिरवतो तेव्हा मजेदार गोष्टी कशा घडवायच्या!