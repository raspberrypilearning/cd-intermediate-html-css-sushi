## Toutes les couleurs!

Comme vous l'avez déjà vu, vous pouvez saisir de nombreux noms de couleurs différents sous forme de mots, et le navigateur les reconnaîtra. Mais un moyen plus commun de définir les couleurs est d'utiliser quelque chose appelé **hex codes** ('hex' est court pour **hexadécimal**, une manière spéciale de compter).

+ Jetez un oeil à votre feuille de style ****. C'est le fichier qui a `.css` dans le nom.

+ A l' intérieur des règles CSS `corps`, définir la couleur d'arrière - plan le code hexadécimal `n 7B68EE`:

```html
  couleur de fond: # 7B68EE;
```

Remarque: Si vous utilisez un Mac, vous pouvez taper `#` en appuyant sur les touches <kbd>alt</kbd> et <kbd>3</kbd> en même temps.

Votre site Web devrait maintenant avoir un fond violet.

![](images/HexColourFirst.png) ![](images/HexColourFirstResult.png)

+ Pas un fan de violet? Aller à [cette page Web](http://dojo.soy/html2-colors){: target = "_ blank"} et choisissez une autre couleur pour votre feuille de style - au lieu de taper le nom de la couleur, tapez le code hexadécimal. 

![](images/ColorNamesHex.png)

Les codes de couleur vous permettent de créer n'importe quelle couleur, même si elle n'apparaît sur aucune liste de noms de couleurs.

+ Essayez de composer votre propre code de couleur. Il doit commencer par un `#`. Cela indique au navigateur qu'il s'agit d'un code hexadécimal au lieu d'un nom de couleur. Le reste du code est composé de six caractères. Ils peuvent être n'importe quel nombre de **0 à 9** et n'importe quelle lettre de **A à F**.

## \--- effondrer \---

## title: Comment ça marche?

Chaque couleur est faite en mélangeant différentes quantités de **rouge**, **vert**et **bleu**. Vous verrez parfois ceci écrit comme **RGB**. Chacune de ces couleurs est représentée par deux des six chiffres de votre code HEX. `00` est le minimum, et `FF` est le maximum.

**hexadécimal** est une méthode de comptage qui rend les nombres plus courts à écrire en utilisant les lettres AF comme chiffres supplémentaires. Le nombre `255` est écrit comme `FF` en hexadécimal. Vous n'avez pas besoin de vous soucier d'apprendre à compter avec des nombres hexadécimaux. Au lieu de cela, expérimentez avec différents codes hexadécimaux pour vous habituer à les utiliser.

+ Voici quelques couleurs de base à essayer sur votre site Web. Essayez de mettre en plus petits nombres au lieu de `FF` pour voir comment les nuances changent.

|      | R  | g  | B  |   Résultat    |
| ---- | -- | -- | -- |:-------------:|
| \ # | FF | 00 | 00 |     rouge     |
| \ # | 00 | FF | 00 |     vert      |
| \ # | 00 | 00 | FF |     Bleu      |
| \ # | FF | FF | 00 |     Jaune     |
| \ # | FF | 00 | FF |    Magenta    |
| \ # | 00 | FF | FF |     Cyan      |
| \ # | FF | 8c | 00 | Orange sombre |

\--- /effondrer \---

Mélanger la couleur parfaite peut demander beaucoup d'expérimentation. Heureusement, il existe de nombreux outils de sélection de couleur en ligne qui vous aident à obtenir le code hexadécimal pour la couleur que vous voulez.

![](images/W3ColorPicker.png)

+ Essayez [ce sélecteur de couleur](http://dojo.soy/html2-color-picker){: target = "_ blank"} pour choisir des codes de couleur hexadécimaux à utiliser pour le reste des styles sur votre site Web.