## एनीमेशन

क्या आप जानते हैं कि आप चीजों को घूमने के लिए CSS का उपयोग कर सकते हैं? आप इस कार्ड से यही सीखेंगे!

+ आरंभ करने से पहले, सुनिश्चित करें कि आपके पास `id` के साथ आपकी वेबसाइट पर एक तस्वीर है और एक संगत CSS ब्लॉक जो की `चौड़ाई` को `100px` निर्धारित करता है। मैं पहले से टीटो की तस्वीर के साथ जा रहा हूं, और मेरा CSS ब्लॉक इस तरह दिखता है:

```css
    #titoPicture {
        border-radius: 100%;
        width: 100px;
    }
```

+ स्क्रिप्ट के नीचे जाएँ और निम्न कोड जोड़ें:

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

यह कोड `myFirstAnimation` नामक एक एनीमेशन बनाता है जिसको आप अपनी वेबसाइट पर किसी भी तत्व से जोड़ सकते हैं। आपको क्या लगता है क्या होगा?

+ चित्र के लिए अपने CSS नियम खोजें और निम्नलिखित तीन गुण जोड़ें:

```css
    animation-name: myFirstAnimation;
    animation-duration: 2s;
    animation-iteration-count: 1;
```

+ अब देखें कि आपके वेब पेज पर क्या होता है! `animation-iteration-count` के लिए अलग-अलग मान आज़माएं और देखिऐ कि यह क्या करता है।

+ चलो एक और एनीमेशन की कोशिश करो! निम्नलिखित कोड को अपनी स्क्रिप्ट के आखिर में जोड़ें:

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

+ अब ` #myCoolText ` ढूंढें पहले से है CSS नियम और एनीमेशन कोड में जोड़ें:

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

जब आप **प्रतिशत मान** का उपयोग करते हैं `से` और `को ` के बजाय, आप मूल्यों के बीच में और साथ ही शुरू और अंत मूल्यों सेट करने में सक्षम हैं। आप `0` से अलग-अलग प्रतिशत मानों का उपयोग करते हुए जितने चाहें उतने मूल्य के बीच सेट कर सकते हैं `100` तक सभी तरह से ।

+ `animation-iteration-count` के मान को `infinite` में बदलें। देखें कि क्या आप अनुमान लगा सकते हैं कि आपके परीक्षण करने से पहले क्या होगा!

+ अपने एनीमेशन को गति देने या धीमा करने के लिए `animation-duration` के लिए अलग-अलग मान आज़माएं।

+ एक अंतिम चाल! इस एनीमेशन कोड को जोड़ें:

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

+ अब `#frontPage` CSS नियम जो आपने पहले लिखे थे ढूंढें और उन्हें इसमें बदलें:

```css
    #frontPage {
        background: repeating-linear-gradient(-45deg, red 0%, yellow 7.14%, lime 14.28%, cyan 21.42%, cyan 28.56%, blue 35.7%, magenta 42.84%, red 50%);
        background-size: 600vw 600vw;
        animation: slide 10s infinite linear forwards;
    }
```

उपरोक्त सभी कोड को समझने की चिंता न करें ... बस वापस बैठो और आनंद लें !!

और अधिक चीज़ें एनीमेशन के साथ आप कर सकते हैं उनके बारे में जानने के लिए, इस वेब पेज [पर जाएं](http://dojo.soy/html2-css-animation){:target="_blank"}। आनंद लें!

अगले कार्ड पर आप सीखेंगे कि जब आप चीजों पर माउस कर्सर घुमाते हैं तो रोचक चीजें कैसे होती हैं!