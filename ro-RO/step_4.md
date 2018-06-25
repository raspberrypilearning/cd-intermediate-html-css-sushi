## Toate culorile!

Așa cum ați văzut mai devreme, puteți să tastați numeroase nume de culori ca cuvinte, iar browserul le va recunoaște. Dar o modalitate mai obișnuită de a seta culorile este de a folosi ceva numit **hex cod** ('hex' este scurt pentru **hexazecimal**, un mod special de numărare).

+ Uitați-vă la foaia dvs. de stil ****. Acesta este fișierul care are `.css` în nume.

+ În interiorul regulilor CSS pentru `corp`, setați culoarea de fundal la codul hexazecimal `# 7B68EE`:

```html
  fundal-culoare: # 7B68EE;
```

Notă: Dacă utilizați un Mac, puteți introduce `#` apăsând simultan tastele <kbd>alt</kbd> și <kbd>3</kbd>.

Site-ul dvs. Web trebuie să aibă acum un fundal purpuriu.

![](images/HexColourFirst.png) ![](images/HexColourFirstResult.png)

+ Nu e un fan al purpurii? Mergeți la [această pagină web](http://dojo.soy/html2-colors){: target = "_ blank"} și alegeți o altă culoare pentru foaia de stil - în loc să tastați numele culorii, introduceți codul hexagonal. 

![](images/ColorNamesHex.png)

Codurile de culori vă permit să creați orice culoare, chiar dacă nu este pe o listă de nume de culori.

+ Încercați să creați propriul cod de culoare. Trebuie să înceapă cu `#`. Acest lucru spune browser-ului că este un cod hexazecimal în locul unui nume de culoare. Restul codului este format din șase caractere. Ele pot fi orice număr de la **0 la 9** și orice literă de la **A la F**.

## \--- colaps \---

## titlu: Cum funcționează?

Fiecare culoare se face amestecând cantități diferite de **roșu**, **verde**și **albastru**. Veți vedea uneori acest lucru scris ca **RGB**. Fiecare dintre aceste culori este reprezentată de două din cele șase cifre din codul dvs. HEX. `00` este minimul, iar `FF` este maximul.

**Hexadecimal** este o modalitate de numărare care face ca numerele să fie mai scurte pentru a scrie utilizând literele AF ca cifre suplimentare. Numărul `255` este scris ca `FF` în hexazecimal. Nu trebuie să vă faceți griji că ați învățat să numărați numerele hexazecimale. În schimb, experimentați cu diferite coduri hexagonale pentru a vă obișnuiți să le folosiți.

+ Iată câteva culori de bază pentru a încerca pe site-ul dvs. Încercați să puneți în număr mai mic în loc de `FF` pentru a vedea cum se schimbă nuanțele.

|      | R  | G  | B  |     Rezultat      |
| ---- | -- | -- | -- |:-----------------:|
| \ # | FF | 00 | 00 |       roșu        |
| \ # | 00 | FF | 00 |       Verde       |
| \ # | 00 | 00 | FF |     Albastru      |
| \ # | FF | FF | 00 |      Galben       |
| \ # | FF | 00 | FF |     purpuriu      |
| \ # | 00 | FF | FF |       Cyan        |
| \ # | FF | 8c | 00 | Portocaliu închis |

\--- / colaps \---

Amestecarea culorii perfecte poate face o multime de experimente. Din fericire, există o mulțime de instrumente de colorare online care vă ajută să obțineți codul hexagonal pentru orice culoare dorită.

![](images/W3ColorPicker.png)

+ Încercați [acest selector de culori](http://dojo.soy/html2-color-picker){: target = "_ blank"} pentru a alege unele coduri de culoare hexagonale pentru a fi utilizate pentru restul stilurilor de pe site-ul dvs. Web.