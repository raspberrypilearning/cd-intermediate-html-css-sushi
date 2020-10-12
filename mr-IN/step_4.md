## आपले पृष्ठ आयोजित करणे

आपली **सामग्री** नीटनेटके आणि वाचण्यास सुलभ करण्यासाठी आपण आतापर्यंत **शीर्षके** आणि **परिच्छेद** वापरली आहेत. गोष्टी एकत्रित करून त्यास अधिक व्यवस्थित बनवू या.

## \--- collapse \---

## title: मजकूर म्हणजे काय?

**सामग्री** ही आपल्या वेब पृष्ठावरील सर्व सामग्री आहे, जसे की पुढील गोष्टी आणि चित्रे.

\--- /collapse \---

+ `attractions.html`फाइलवर जा (किंवा आपल्या स्वत: च्या पृष्ठावर जर आपण उदाहरणार्थ प्रोजेक्ट वापरत नसल्यास) आणि वर, एकदम सुरुवातीच्या `<main>`टॅगच्या **खाली**, एका नवीन लाइन वर, खालील टाइप करा: 

```html
  <main>
    <article>
```

+ जर आपला एडिटरने आपोआप एक बंद होणारा `</article>` टॅग जोडला असेल तर, ते हटवा.

+ फाईलच्या तळाशी, एकदुम बंद होणार्‍या `</main>` टॅग **वर**, एक नवीन ओळ जोडा आणि `article` घटक बंद करा:

```html
    </article>
  </main>
```

आपला `main` घटकाला आता यासारखे काहीतरी दिसले पाहिजे (`article` टॅग दरम्यान आपल्याकडे नक्कीच भिन्न मजकूर असू शकते):

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

+ आता आपल्या `article` मजकूर पहा आणि विभागांमध्ये तोडण्याचा प्रयत्न करा. ह्या नवीन टॅगची जोडी प्रत्येका तुकड्या भवती ठेवा: `<section></section>`. हे कसे दिसतील त्याचे उदाहरण येथे आहे:

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

## title: नवीन टॅग कष्याबद्दल आहेत?

या नवीन घटकांचा **कंटेनर** म्हणून विचार करा. ते गोष्टी एकत्र करण्यासाठी वापरले जातात. हे आपल्या घरामधील बॉक्स आणि शेल्फमध्ये गोष्टी आयोजित करण्यासारखे आहे!

हे आपली वेबसाइट स्क्रीन वाचकांसाठी अनुकूल बनवते, लेआउटवर आपल्याला अधिक नियंत्रण देते आणि जसे की आपण पहाल ते आपल्याला स्टाईलसह खरोखर सर्जनशील बनण्याची परवानगी देते.

टॅग दरम्यान काहीही जाऊ शकते. सामान्यत: ते एकापेक्षा जास्त घटक असतील, परंतु तसे होणे आवश्यक नाही. हे कोणत्याही प्रकारच्या HTML घटक असू शकतात. तुम्ही हे करतायेत की, तुम्ही ब्राऊजर ल सांगता आहेत की हे सघळे टॅग्ज एकत्र आहेत.

### लेख

`article` घटक संपूर्ण मजकुरासाठी एक कंटेनर आहे, या प्रकरणात आयर्लंडमधील आकर्षणांविषयी माहितीचा एक संच आहे. जर तुमच्याकडे मजकुराचे भिन्न अंश असतील जे संभंधित नाहीयेत, तर एक टॅग्जचा संच पूर्ण वाट्यात ठेवण्याच्या ऐवेजी, प्रत्येकी तेच्या स्वतःच्या `article` मध्ये ठेवा.

### विभाग

`section` घटक आपल्याला संबंधित मजकूर लहान भागांमध्ये विभागू देतो आणि प्रत्येक भाग त्याच्या स्वत: च्या कंटेनरमध्ये ठेवू देतो.

### इतरही अस्तित्वात आहेत!

HTML मधील हे केवळ कंटेनर घटक नाहीत. आपण कधी मेनू तयार केला असेल आणि नंतर त्यास दरम्यान `<nav></nav>`टॅग्ज ठेवला असेल, तर हे कंटेनरच्या प्रकाराचे आणखी एक उदाहरण आहे. त्यासारखे `<main> </main>` आणि `<header> </header>` आहेत - आणखी काही आहेत का हे आपण विचार करू शकता का?

\--- /collapse \---

\--- challenge \---

आपले वेबपृष्ठ अद्याप कदाचित भिन्न दिसत नाही परंतु कन्टेन्ट एकदा कंटेनर टॅगमध्ये व्यवस्थित केली गेल्यानंतर आपण त्यास CSS सह काही छान गोष्टी करण्यास सक्षम व्हाल. लक्षात ठेवा, आपली वेबसाइट कशी व्यवस्थित केली जाते हे HTML नियंत्रित करते आणि ती कशी दिसते हे CSS नियंत्रित करते.

## आव्हान: आपली वेबसाइट आयोजित करा

+ आपल्या वेबसाइटवरील सर्व मजकूर आयोजित करण्यासाठी `article` आणि `section` कंटेनरचा वापर अशा प्रकारे करुन पाहा. 

\--- hints \---

\--- hint \---

उदाहरणार्थ प्रोजेक्टचे फूड पेज पहा. आपल्याला हे दिसेल की `food.html` फाईलमध्ये `article` सोबत `section` चा घड जोडला आहे:

```html
  <main>
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
```

\--- /hint \---

\--- /hints \---

पुढील कार्डवर, लेख आणि विभागांमध्ये आयोजित केलेल्या प्रत्येक पृष्ठासाठी आपण एक भिन्न थीम डिझाइन कराल!

\--- /challenge \---