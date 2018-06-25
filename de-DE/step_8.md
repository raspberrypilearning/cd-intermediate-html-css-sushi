## Siehe den Code auf anderen Websites!

**Hinweis:** Um diesen Schritt auszuführen, müssen Sie einen dieser Webbrowser verwenden: Chrome, Firefox oder Internet Explorer / Edge. Wenn Sie keinen Zugriff auf einen von ihnen haben, können Sie einfach mit der nächsten Karte fortfahren.

Auf dieser Karte erfahren Sie, wie Sie mithilfe des **Inspector-Tools**den Code einer Website ansehen können. Außerdem erfahren Sie, wie Sie Änderungen vornehmen können, die nur Sie sehen können!

+ Bevor Sie beginnen, vergewissern Sie sich, dass Ihr Projekt gespeichert ist. Aktualisieren Sie dann Ihre Website, indem Sie auf das Aktualisierungssymbol in Ihrem Browser klicken.

+ Markieren Sie auf Ihrer Webseite (die tatsächliche Seite, nicht den Code) den Text mit dem Rahmen, den Sie auf der vorherigen Karte hinzugefügt haben, klicken Sie dann mit der rechten Maustaste darauf und wählen Sie die Option **Inspect** aus dem angezeigten Menü. (Je nachdem, welchen Browser Sie verwenden, lautet die Option "Element prüfen" oder Ähnliches. Wenn du Probleme hast, eine Menüoption zu finden, frage einfach jemanden in deinem Dojo um Hilfe.)

![Auswählen der Option "Prüfen" für markierten Text](images/highlightTextAndInspect.png)

In Ihrem Webbrowser wird eine ganz neue Box mit vielen Tabs und Code erscheinen: die **Entwicklerwerkzeuge**oder **Entwicklerwerkzeuge** kurz. Hier sehen Sie den Code für die Sache, auf die Sie geklickt haben, sowie den Code für die ganze Seite!

### Überprüfen des HTML-Codes

+ Suchen Sie nach dem Tab, der Ihnen den HTML-Code für die Seite anzeigt (er könnte "Elemente" oder "Inspektor" heißen). Der Code sollte so aussehen, wie Sie ihn in Ihre HTML-Datei eingegeben haben! Sie können auf die kleinen Dreiecke auf der rechten Seite klicken, um den versteckten Code zu erweitern.

![Inspektor, der ein Textelement zeigt](images/inspectTextHtml.png)

+ Doppelklicken Sie auf den Text zwischen den Tags. Sie sollten es jetzt bearbeiten können! Geben Sie etwas ein und drücken Sie <kbd>Enter</kbd>.

![Bearbeiten von Text mit dem Inspektor-Tool](images/inspectEditHtmlText.png)

+ Siehst du den Text auf deiner Website aktualisieren? Hinweis: Nur Sie können diese Änderungen sehen.

![Website mit bearbeitetem Text](images/inspectEditHtmlTextResult.png)

+ Jetzt **reload** die Seite und beobachten , was passiert. Deine Änderungen sollten verschwinden!

+ Klicken Sie in der oberen linken Ecke der Dev Tools-Box auf das Symbol, das wie ein kleines Rechteck mit einem Pfeil aussieht. Jetzt können Sie den Cursor über die Webseite bewegen, und der HTML-Inspektor zeigt Ihnen den Code, der ihn beschreibt.

![Das Symbol zum Auswählen von Elementen](images/inspectorSelectIcon.png) ![Auswählen eines Elements](images/inspectorSelectElement.png)

### Überprüfung des CSS-Codes

+ Schauen wir uns den CSS-Code als nächstes an. Suchen Sie in den Entwicklertools nach der Registerkarte **Styles** (möglicherweise "Style Editor" oder ähnlich). Sie sollten eine Reihe von CSS-Regeln sehen, einschließlich derjenigen, die Sie für diesen Absatz erstellt haben, `#myCoolText`.

![Anzeigen des CSS-Codes für ein Element](images/inspectCssBlock.png)

+ Klicken Sie in den `#myCoolText` Regeln auf den Wert neben der Eigenschaft `Farbe`. Tippe einen anderen Wert ein. Beobachten Sie den Text auf Ihrer Webseite und ändern Sie die Farbe sofort! 

![Bearbeiten der Textfarbe mit dem CSS-Inspektor](images/inspectEditCssColor.png)

Hinweis: Sie können auch auf das farbige Quadrat klicken, um die Farbe mit einem Farbauswahlwerkzeug zu ändern.

+ Klicken Sie in das Feld hinter der Farbe. Eine neue Zeile beginnt, in der Sie mehr CSS eingeben können. Geben Sie Folgendes ein und drücken Sie <kbd>Enter</kbd>:

```css
  Hintergrundfarbe: # 660066;
```

Sie sollten sehen, dass sich der Hintergrund für diesen Text ändert.

![Hinzufügen der Hintergrundfarbeneigenschaft](images/inspectorEditingBgCol.png) ![Die neue Hintergrundfarbe](images/inspectorEditBgResult.png)

## \--- Einsturz \---

## Titel: Wie funktioniert es?

Wenn Sie Website - Code unter Verwendung der Entwickler - Tool zu ändern, sind Sie **vorübergehend** ändern , was es sieht aus wie **in Ihrem Browser**. Sie ändern nicht wirklich die Dateien, aus denen die Website besteht.

Wenn Sie die Seite aktualisieren, laden Sie die Website erneut aus ihren Dateien (im Internet oder auf Ihrem Computer). Deshalb verschwinden deine Änderungen.

Nun, da Sie das wissen, können Sie Spaß mit dem Code auf anderen Websites haben!

\--- / einklappen \---

+ Verwenden Sie diese Tools, um den Code auf einer anderen Website anzuzeigen. Sie können sogar Änderungen vornehmen, wenn Sie möchten! Denken Sie daran, dass nur Sie die Änderungen sehen können, die Sie vornehmen, und alles wird zurückgesetzt, wenn Sie die Seite aktualisieren.