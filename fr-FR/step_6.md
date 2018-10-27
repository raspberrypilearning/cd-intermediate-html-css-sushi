## Concevoir des thèmes

Ecrire des règles CSS pour des éléments tels que `section` et `p` est super, mais que faire si vous voulez que certains d'entre eux soient différents des autres? Sur cette carte, vous apprendrez à appliquer différents ensembles de règles de style à des éléments du même type et à créer un thème différent pour chaque page de votre site Web!

+ Accédez à votre feuille de style et ajoutez ce qui suit - assurez-vous d'inclure le point devant!

```css
  .topDivider {border-top-style: solide; border-top-width: 2px; border-top-color: # F5FFFA; rembourrage-fond: 10px; }
```

+ Maintenant , allez à `attractions.html` (ou le fichier HTML que vous travaillez sur si vous utilisez votre propre projet), et ajouter les éléments suivants **attribut** à chaque `section` tag:

```html
  <section class="topDivider">
```

Vous devriez voir apparaître une ligne au-dessus de chaque section de la page. Félicitations - vous venez d'utiliser votre premier **CSS classe**!

![Page avec des lignes entre les sections](images/sectionsWithTopBorder.png)

+ Regardez à quoi ressemble votre page Web et comparez-la aux autres pages qui contiennent `élément de la section`. Vous verrez que seuls ceux où vous avez ajouté l'attribut `class = "topDivider"` auront la ligne en haut.

## \--- effondrer \---

## title: Comment ça marche?

Rappelez - vous que lorsque vous utilisez un CSS **sélecteur** tel que `section` ou `p` ou `nav ul`, les règles de style s'appliquent à **tous les** éléments de ce type sur votre site.

Avec CSS **classes**, vous êtes en mesure de changer le style de seulement **** des éléments.

Mettre un point devant votre sélecteur en fait un sélecteur de classe ****. Une classe peut avoir n'importe quel nom, il ne doit donc pas être le nom d'un élément HTML. Par exemple:

```css
  .myAwesomeClass {/ * mes règles de style cool vont ici * /}
```

Pour choisir quels éléments les règles de style s'appliquent, vous ajoutez la `classe` **attribut** à ces éléments dans le code HTML: mettre le nom de la classe en tant que valeur de l'attribut, **sans** le point, comme celui - ci:

```html
  class = "myAwesomeClass"
```

\--- /effondrer \---

+ Prêt à essayer un autre cours? Ajoutez le code CSS suivant à `styles.css`:

```css
  .stylishBox {background-color: # 87CEFA; couleur: # A52A2A; style de bordure: solide; border-width: 2px; border-color: # F5FFFA; border-radius: 10px; }
```

+ Ensuite, sur une autre page de votre site Web, ajoutez la classe à certains éléments. Je vais l'ajouter aux `éléments de la section` sur la page Food de mon site web, comme ceci: `<section class="stylishBox">`.

Ça a l'air génial, mais maintenant mes sections sont toutes écrasées.

![Belles sections à la recherche écrasée](images/squashedSections.png)

Vous pouvez appliquer autant de classes CSS à un élément que vous le souhaitez. Il suffit d'écrire le nom de toutes les classes que vous voulez utiliser dans l'attribut `class` (souvenez-vous, sans le point!), En les séparant par des espaces.

+ Faisons une autre classe CSS pour donner une marge et un remplissage aux sections. Dans le fichier `styles.css` , créez la classe CSS suivante:

```css
  .someSpacing {padding: 10px; marge supérieure: 20px; }
```

+ Dans votre code `html` , ajoutez la nouvelle classe à chacun des éléments sur lesquels vous travailliez, comme ceci:

```html
  <section class="stylishBox someSpacing">
```

![Sections avec marge et remplissage ajoutés](images/sectionsWithSpacing.png)

Ainsi , les classes CSS vous permettent de **choisir** quels éléments de style, et ils vous permettent de **réutiliser** le même ensemble de règles de style sur tous les éléments que vous voulez.

+ Aller à `index.html` et ajouter le `stylishBox` classe au `principal` élément ou un autre élément sur la page. Vous pouvez l'enlever à nouveau après!

```html
    <main class="stylishBox">   
```

Voici à quoi ressemble ma page d'accueil avec la classe CSS. J'ai également ajouté la classe `topDivider` à la balise `img` avec l'image de Tito.

![Classes CSS utilisées sur la page d'accueil](images/homePageWithClasses.png)

\--- défi \---

## Défi: faire de nouvelles classes

+ Utilisez CSS **classes** pour définir quelques tailles d'image différentes pour votre site Web, par exemple `.smallPictures` et `.mediumPictures`. Ensuite, supprimez l'attribut `largeur` de chacun de vos `éléments img` et ajoutez la classe appropriée à la place.

\--- astuces \---

\--- indice \---

Vous pouvez créer une classe CSS qui ne définit que la largeur d'un élément comme celui-ci:

```css
  .smallPictures {width: 100px; }
```

\--- / indice \---

\--- indice \---

Voici une balise `img` avec un attribut `width`:

```html
  <img src="tito.png" alt="Tito the dog" width="100px" />       
```

Lorsque vous supprimez l'attribut `largeur` et contrôlez la taille avec la classe CSS à la place, il ressemble à ceci:

```html
  <img src="tito.png" class="smallPictures" alt="Tito the dog" />       
```

En utilisant une classe CSS, vous pouvez facilement changer la largeur de toutes les images à la fois en changeant une seule ligne de code dans votre feuille de style!

\--- / indice \---

\--- /astuces \---

\--- /défi \---