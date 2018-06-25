## Style individuel

Amusons un peu la page d'accueil! With another kind of CSS selector, you can apply a unique set of CSS rules to just **one specific element**.

+ Aller à `index.html` et trouver un élément de paragraphe (`p`), ou en ajouter un si vous n'en avez pas. Ajoutez les lignes suivantes **attribut** à la balise:

```html
    <p id="myCoolText">
        Mon site Web concerne l'Irlande.
    </p> 
```

Le `id` est un nom que vous donnez un élément particulier à **identifier** elle. Deux éléments sur une page ne devrait jamais avoir le même `id`!

+ Maintenant, allez sur votre feuille de style et ajoutez le code suivant:

```css
    #myCoolText {color: # 003366; frontière: 2px ridge #ccffff; rembourrage: 15px; text-align: centre; }
```

Votre texte devrait ressembler à ceci maintenant:

![Texte avec une couleur différente et une bordure autour](images/paragraphIdStyle.png)

Un sélecteur précédé d'un `#` est utilisé pour appliquer les règles CSS à un élément spécifique de votre site Web. Vous spécifiez l'élément à l'aide du nom que vous avez attribué à l'attribut `id` l'élément.

+ Faisons-en un pour le `corps` de la page d'accueil. Aller à `index.html` et ajouter un `id` à l'étiquette `corps`.

```html
    <body id="frontPage">
```

+ Dans la feuille de style, ajoutez les règles CSS suivantes:

```css
    #frontPage {background: # 48D1CC; arrière-plan: gradient linéaire (# fea3aa, # f8b88b, # faf884, # baed91, # baed91, # b2cefe, # f2a2e8, # fea3aa); }
```

Vous devriez obtenir quelque chose qui ressemble à ceci:

![Fond dégradé arc-en-ciel](images/frontPageIdStyles.png)

Vous venez d'utiliser un **gradient**! C'est le nom donné à l'effet où une couleur se fond dans une autre. Remarque: La première propriété `arrière-plan` au-dessus du dégradé détermine une couleur par défaut pour les navigateurs qui ne prennent pas en charge les dégradés.

Si vous avez tapé le code parfaitement et que vous n'avez pas obtenu le bel effet arc-en-ciel ci-dessus, il se peut que votre navigateur ne prenne pas en charge les dégradés.

Vous pouvez faire beaucoup d'effets différents avec des dégradés. Si vous voulez en savoir plus, allez [ici](http://dojo.soy/html2-css-gradients){: target = "_ blank"}.

\--- défi \---

## Défi: styliser d'autres éléments

+ Essayez de donner à un autre élément un `id` et de styliser cet élément en utilisant le sélecteur d'ID avec un `#` comme ci-dessus. Que diriez-vous de faire une image avoir un `frontière-rayon` de `100%` sorte qu'il est entièrement arrondi? Toutes les autres images sur le site resteront les mêmes. 

\--- astuces \---

\--- indice \---

Vous attribuez un `élément` en ajoutant l'attribut `id` à la balise HTML, comme ceci:

```html
  <img src="tito.png" id="titoPicture" alt="Tito the dog" />        
```

Choisissez n'importe quel `id` nom que vous aimez.

\--- / indice \---

\--- indice \---

Pour définir des règles de style pour un élément spécifique, vous utilisez le `#` symbole et le nom que vous avez donné l'élément comme `id`.

```css
  #titoPicture {border-radius: 100%; }
```

Remarque: le nom que vous tapez devant les règles CSS doit **exactement** Faites correspondre le nom que vous mettez dans l'élément `id` attribut.

\--- / indice \---

\--- /astuces \---

![Une image ronde de Tito avec une bordure blanche](images/titoPictureIdStyle.png)

\--- /défi \---