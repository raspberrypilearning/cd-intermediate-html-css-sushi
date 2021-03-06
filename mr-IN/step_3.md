## सर्व रंग!

आपण आधी पाहिल्याप्रमाणे, आपण बर्‍याच वेगवेगळ्या रंगांची नावे शब्दांसारखी टाइप करू शकता आणि ब्राउझर त्यास ओळखेल. रंग निश्चित करण्याचा अधिक सामान्य मार्ग म्हणजे **hex codes** नावाची एखादी गोष्ट वापरणे ('hex' हे **hexadecimal** लहानसे रूप, मोजणीचा एक विशेष मार्ग आहे).

+ आपल्या **style sheet** वर एक नजर टाका. हीच ती फाइल आहे ज्याच्या नावात `.css` आहे.

+ CSS नियमांच्या आत `body` साठी, पार्श्वभूमी रंग हेक्स कोड `#7B68EE` वर सेट करा:

```html
  background-color: #7B68EE;
```

टीप: आपण Mac वापरत असल्यास, `#` टाइप करण्यासाठी <kbd>alt</kbd> आणि <kbd>3</kbd> की एकाच वेळी दाबा.

आपल्या वेबसाइटला आता जांभळी पार्श्वभूमी असावी.

![](images/HexColourFirst.png) ![](images/HexColourFirstResult.png)

+ जांभळ्या रंगाचे चाहते नाही? या [हे वेब पृष्ठ](http://dojo.soy/html2-colors){:target="_blank"} वर जा आणि आपल्या स्टईल शीट साठी त्याऐवजी दुसरा रंग निवडा - रंगाचं नाव टाइप करण्याऐवेजी, हेक्स कोड टाइपकरा. 

![](images/ColorNamesHex.png)

रंग कोड आपल्याला कोणत्याही रंग तयार करण्याची अनुमती देतात, जरी ते रंगांच्या नावांच्या सूचीत नसले तरीही.

+ आपला स्वतःचा रंग कोड बनविण्याचा प्रयत्न करा. त्याची सुरुवात `#` चिन्ह ने व्हावी. हे ब्राउझरला सांगते की रंगाच्या नावाऐवजी हा हेक्स कोड आहे. उर्वरित कोड सहा वर्णांनी बनलेला आहे. ते **0 to 9** आणि **A to F**पर्यंतचे कोणतेही अक्षर असू शकतात.

--- collapse ---
---
title: हे कसं काम करतं?
---

प्रत्येक रंग **red**, **green**, आणि **blue**, वेगवेगळ्या प्रमाणात मिसळून बनविला जातो. आपल्याला हे कधीकधी **RGB** असे लिहिलेले दिसेल. यापैकी प्रत्येक रंग आपल्या हेक्स कोडमधील सहा पैकी दोन अंकांद्वारे दर्शविला जातो. `00` किमान आहे आणि `FF` कमाल आहे.

**Hexadecimal** हा मोजणीचा एक मार्ग आहे ज्यामुळे अतिरिक्त अक्षरे म्हणून ए-एफ(A-F) अक्षरे वापरुन संख्या लिहिण्यास लहान केले जाते. संख्या `255` हेक्साडेसिमलमध्ये `FF` म्हणून लिहिलेली आहे. हेक्साडेसिमल संख्यांसह मोजणे शिकण्याची आपल्याला चिंता करण्याची आवश्यकता नाही. त्याऐवजी, हेक्स कोड वापरण्याची सवय लावण्यासाठी त्यांच्या विविध प्रकारांचा प्रयोग करा.

+ आपल्या वेबसाइटवर पाहण्यासाठी येथे काही मूलभूत रंग आहेत. शेड्स कसे बदलतात हे पाहण्यासाठी `FF` ऐवजी लहान संख्या ठेवण्याचा प्रयत्न करा.

|      | R  | G  | B  |  परिणाम   |
| ---- | -- | -- | -- |:---------:|
| \# | FF | 00 | 00 |    लाल    |
| \# | 00 | FF | 00 |   हिरवा   |
| \# | 00 | 00 | FF |   निळा    |
| \# | FF | FF | 00 |   पिवळा   |
| \# | FF | 00 | FF | मॅजेन्टा  |
| \# | 00 | FF | FF |   निळसर   |
| \# | FF | 8c | 00 | गडद केशरी |

--- /collapse ---

परिपूर्ण रंग मिसळण्या करिता बरेच प्रयोग करावे लागू शकते. सुदैवाने, बरीच ऑनलाईन कलर पिकिंग टूल्स आहेत जी तुम्हाला हव्या त्या रंगाचा हेक्स कोड मिळविण्यात मदत करतात.

![](images/W3ColorPicker.png)

+ आपल्या वेबसाइटवरील उर्वरित शैलींसाठी वापरण्यासाठी काही हेक्स रंग कोड निवडण्यासाठी [हा कलर पिकिंग टूल](http://dojo.soy/html2-color-picker){:target="_blank"} वापरून पहा.