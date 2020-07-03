## अपने पृष्ठ का आयोजन

अब तक आपने ** कन्टेन्ट** देखने और पढ़ने में आसान बनाने के लिए ** शीर्षकों **और ** पैराग्राफ ** का उपयोग किया है। आइए इसे एक साथ चीजों को समूहीकृत करके और भी व्यवस्थित करें।

## \--- collapse \---

## title: कन्टेन्ट क्या है?

** कन्टेन्ट** आपके वेब पेज पर सभी सामान है, इस तरह के एस्टेक्स्ट और चित्र।

\--- /collapse \---

+ `attractions.html` फ़ाइल में जाएं। (या यदि आप उदाहरण प्रोजैक्ट का उपयोग नहीं कर रहे हैं तो अपने स्वयं के पृष्ठों में से एक) और, शीर्ष के पास, बस ** नीचे ** उद्घाटन टैग `<main>`, नई लाइन पर निम्नलिखित टाइप करें: 

```html
  <main>
    <article>
```

+ यदि आपका संपादक स्वचालित रूप से एक समापन टैग `</article>` जोड़ा गया है, इसे हटाएं।

+ फ़ाइल के निचले भाग में, बस ** ऊपर ** समापन ` </main>` टैग, एक नई पंक्ति जोड़ें और ` article` तत्व: बंद करें

```html
    </article>
  </main>
```

आपका `main` को अब इस तरह से देखना चाहिए (आपके पास `article` टैग के बीच भिन्न सामग्री हो सकती है):

```html
  <main>
    <article>
      <h1>My favourite places to see in Ireland</h1>
        <h2>The Cliffs of Moher</h2>
        <p>
        The Cliffs of Moher are found in County Clare, where I am from. Look how cool they are!</p>
        <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
        <h2>Achill Island</h2>
        <p>This is a large island off the coast of County Mayo. It has a wild and
        beautiful landscape of mountains, bogs and cliffs.
        </p>
        <img src="achill.JPG" width="200px" />
    </article>
  </main>
```

+ अब अपने `article` में कन्टेन्ट को देखें और इसे खंडों में तोड़ने का प्रयास करें। टैग की इस नई जोड़ी को प्रत्येक बिट के आसपास रखें: `<section> </section>` । यहाँ एक उदाहरण है कि यह कैसा दिख सकता है:

```html
  <article>
    <h1>My favourite places to see in Ireland</h1>
    <section>
      <h2>The Cliffs of Moher</h2>
      <p>
      The Cliffs of Moher are found in County Clare, where I am from. Look how cool they are!</p>
      <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
    </section>
    <section>
      <h2>Achill Island</h2>
      <p>This is a large island off the coast of County Mayo. It has a wild and
      beautiful landscape of mountains, bogs and cliffs.
      </p>
      <img src="achill.JPG" width="200px" />
    </section>
  </article>
```

## \--- collapse \---

## title: नए टैग क्या हैं?

इन नए तत्वों को ** कंटेनरों ** के रूप में सोचें। उनका उपयोग चीजों को एक साथ समूहित करने के लिए किया जाता है। यह आपके घर में बक्से और अलमारियों में चीजों को व्यवस्थित करने जैसा है!

यह आपकी वेबसाइट को स्क्रीन रीडर्स के लिए अनुकूल बनाता है, आपको लेआउट पर अधिक नियंत्रण देता है, और, जैसा कि आप देखेंगे, यह आपको स्टाइल के साथ वास्तव में रचनात्मक बनाने की अनुमति देता है।

टैग के बीच में कुछ भी जा सकता है। आमतौर पर यह एक से अधिक तत्व होगा, लेकिन यह होना जरूरी नहीं है। यह किसी भी तरह का HTML एलिमेंट हो सकता है। आप जो कर रहे हैं वह ब्राउज़र को बता रहा है कि इन टैगों के बीच सब कुछ एक साथ है।

### आर्टिकल

`article` तत्व सामग्री के एक पूरे टुकड़े के लिए एक कंटेनर है, इस मामले में आयरलैंड में आकर्षण के बारे में जानकारी का एक सेट है। यदि आपके पास अलग-अलग कन्टेन्ट है जो संबंधित नहीं हैं, तो आपको प्रत्येक को अपने `article` तत्व में डालना चाहिए पूरे लॉट के चारों ओर टैग का एक सेट लगाने के बजाय।

### अनुच्छेद

`section` तत्व आपको संबंधित कन्टेन्ट को छोटे चंक्स में विभाजित करने और प्रत्येक चंक को अपने कंटेनर में रखने की सुविधा देता है।

### अन्य भी मौजूद हैं!

ये HTML में केवल कंटेनर तत्व नहीं हैं। यदि आपने कभी मेनू बनाया है और फिर उसे `<nav></nav>` टैग के बीच में रखा है, यह एक और प्रकार का कंटेनर है। वैसे ही `<main> </main>` और `<header> </header>` हैं- क्या आप किसी और के बारे में सोच सकते हैं?

\--- /collapse \---

\--- challenge \---

हो सकता है कि आपका वेब पेज अभी अलग न दिखे, लेकिन एक बार कंटेंट कंटेनर टैग में व्यवस्थित हो जाने के बाद, आप इसे CSS के साथ कुछ अच्छी चीजें करने में सक्षम होंगे। याद रखें, HTML नियंत्रित करता है कि आपकी वेबसाइट कैसे व्यवस्थित है, और CSS यह कैसे दिखता है।

## चुनौती: अपनी वेबसाइट व्यवस्थित करें

+ इस तरह से `article` और `section` कंटेनर का उपयोग करके अपनी वेबसाइट की सभी कन्टेन्ट को व्यवस्थित करने पर ध्यान दें। 

\--- hints \---

\--- hint \---

उदाहरण प्रोजैक्ट के खाद्य पृष्ठ को देखें। आप देखेंगे कि मैंने ` food.html ` फ़ाइल में कई ` article ` और </code>section ` टैग जोड़ा है:</p>

<pre><code class="html">  <main>
    <article>
      <h1>Food in Ireland</h1>
      <p>
        These are some of my favourite Irish foods!
      </p>  
      <section>
        <h2>Traditional Irish Breakfast</h2>
        <p>
          A "Full Irish" breakfast consists of sausages, rashers (bacon),
          eggs, black pudding, white pudding and toast.
        </p>
        <p>
          Often there will be a grilled tomato as well as mushrooms,
          and baked beans.
        </p>
        <p>
          And of course, no breakfast is complete without a lovely pot 
          of tea!
        </p>
      </section>

      <section>
        <h2>Bangers and Mash</h2>
        <p>
          This classic of sausages, mashed potato and gravy is not
          unique to Ireland, but what makes it special is the Irish
          sausages. Most countries have their own way of making sausages,
          and they are one thing I miss from home if I'm away travelling!
        </p>
      </section>

      <section>
        <h2>Bacon and Cabbage</h2>
        <p>
          I couldn't possibly make a list of Irish food without including
          this very traditional dish!
        </p>
        <p>
          It might not sound very interesting, but this hearty meal of
          boiled ham, potatoes and green cabbage is tasty and filling.
          I love to smother the potatoes in butter, and I also like a
          little mustard with the bacon.
        </p>
        <p>
          My mum always made it extra special by cooking the cabbage in
          the water that the ham was boiled in.
        </p>
        <p>
          If there are any leftovers you can make another one of my
          favourites: <strong>fried cabbage</strong>!
        </p>
      </section>
    </article>     
  </main>
`</pre> 

\--- /hint \---

\--- /hints \---

अगले कार्ड पर, आप प्रत्येक पृष्ठ के लिए एक अलग थीम डिज़ाइन करेंगे जो लेखों और अनुभागों में व्यवस्थित है!

\--- /challenge \---