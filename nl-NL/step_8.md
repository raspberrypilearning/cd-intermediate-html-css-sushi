## Bekijk de code van andere websites!

**Opmerking:** Om deze stap te voltooien, moet je een van deze webbrowsers gebruiken: Chrome, Firefox of Internet Explorer/Edge. Als je geen toegang hebt tot een van deze webbrowsers, kun je gewoon doorgaan naar de volgende kaart.

Op deze kaart leer je hoe je een kijkje kunt nemen in de code van een website met behulp van de **inspectie tool**, en je zult ook ontdekken hoe je enkele wijzigingen kunt aanbrengen die alleen jij kunt zien!

+ Zorg ervoor dat voordat je begint je project is opgeslagen. Vernieuw vervolgens je website door op het vernieuwingspictogram in je browser te klikken.

+ Op je webpagina (de eigenlijke pagina, niet de code) markeer je de tekst met rand die je op de vorige kaart hebt toegevoegd, klik er met de rechtermuisknop op en selecteer de optie **Inspecteren** vanuit het menu dat verschijnt. (De optie kan 'Inspect Element' of iets dergelijks worden genoemd, afhankelijk van welke browser je gebruikt. Als je problemen ondervindt bij het vinden van de menuoptie, vraag je gewoon iemand bij jouw Dojo om hulp.)

![Selecting the Inspect option on highlighted text](images/highlightTextAndInspect.png)

Er verschijnt een heel nieuw vak in je webbrowser met veel tabbladen en code: de **ontwikkelaarstools**, of **dev-tools** in het kort. Hier kunt je de code zien voor het gedeelte die je gemarkeerd hebt, maar ook de code voor de hele pagina!

### Doornemen van de HTML-code

+ Zoek naar het tabblad met de HTML-code voor de pagina (dit kan 'Elements' of 'Inspector' worden genoemd). De code moet er ongeveer hetzelfde uitzien als hoe je deze in jouw HTML-bestand hebt getypt! Je kunt op de kleine driehoekjes aan de linkerkant van het vak klikken om de verborgen code uit te vouwen.

![Inspector showing a text element](images/inspectTextHtml.png)

+ Dubbelklik op de tekst tussen de tags. Je zou het nu moeten kunnen bewerken! Type something in and press <kbd>Enter</kbd>.

![Editing text using the inspector tool](images/inspectEditHtmlText.png)

+ Do you see the text update on your website? Note: only you can see these changes.

![Website with edited text](images/inspectEditHtmlTextResult.png)

+ Now **reload** the page and watch what happens. Your changes should disappear!

+ In the top left-hand corner of the dev tools box, click the icon that looks like a tiny rectangle with an arrow. Now you can move your cursor over the web page, and the HTML inspector will show you the code describing it.

![The icon to select elements](images/inspectorSelectIcon.png) ![Selecting an element](images/inspectorSelectElement.png)

### Inspecting the CSS code

+ Let's have a look at the CSS code next. Look for the **Styles** tab in the developer tools (it might be called 'Style Editor' or similar). You should see a bunch of CSS rules, including the ones you created for that paragraph, `#myCoolText`.

![Viewing the CSS code for an element](images/inspectCssBlock.png)

+ In the `#myCoolText` rules, click on the value next to the `color` property. Try typing in a different value. Watch the text on your web page change colour straight away! 

![Editing the text colour using the CSS inspector](images/inspectEditCssColor.png)

Note: you can also click the coloured square to change the colour using a colour picker tool.

+ Click in the space after the colour. A new line starts, where you can type more CSS. Type the following and press <kbd>Enter</kbd>:

```css
  background-color: #660066;
```

You should see the background change on that piece of text.

![Adding the background colour property](images/inspectorEditingBgCol.png) ![The new background colour](images/inspectorEditBgResult.png)

## \--- collapse \---

## title: How does it work?

When you change website code using the developer tools, you are **temporarily** changing what it looks like **in your browser**. You aren't actually changing the files that make up the website.

When you refresh the page, you are loading up the website again from its files (on the internet or on your computer). That's why your changes disappear.

Now that you know that, you can have some fun messing with the code on other websites!

\--- /collapse \---

+ Try using these tools to look at the code on another website. You can even make changes if you like! Remember, only you can see the changes you make, and everything will reset when you refresh the page.