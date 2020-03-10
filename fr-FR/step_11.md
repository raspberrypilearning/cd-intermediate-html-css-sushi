## Apprenez à Tito à rouler!

Vous pouvez rendre votre site plus **interactif** en faisant des trucs cool se produire lorsque vous passez la souris sur les choses avec le curseur de la souris!

+ Trouvez vos règles CSS pour les éléments `img`, ou créez-en si vous n'en avez pas. Ajoutez une bordure, puis ajoutez un nouveau bloc de règles juste en dessous:

```css
  img {
    border: 2px solid White;
  }
  img:hover {
    border: 2px dashed Navy;
  }
```

Vous venez d'utiliser un type spécial de bloc CSS appelé **pseudo-classe**.

--- collapse ---
---
title: Comment ça marche?
---

A **pseudo-classe** est un peu différent d'une **classe** que vous créez. Vous pouvez le reconnaître par le `:`.

Les pseudo-classes sont intégrées aux éléments HTML: vous pouvez ajouter des règles de style `: hover` à n'importe quel élément, classe ou sélecteur `id` dans votre feuille de style sans avoir besoin d'ajouter quelque chose supplémentaire dans votre code HTML.

--- /collapse ---

+ Que penses-tu qu'il va se passer? Vérifiez quelles pages de votre site Web ont des photos sur eux (ajoutez une image s'il n'y en a pas!), Puis déplacez votre curseur sur une image pour le savoir!

+ Utilisons cette nouvelle pseudo-classe `: hover` avec une classe CSS pour faire briller les liens quand vous les survolez! Ajoutez un lien vers votre page Web et incluez un attribut pour spécifier le nom de la classe. Rappelez-vous, les liens sont définis en utilisant la balise `<a>` , comme ceci:

```html
    <p>
      Visitez la page <a class="niceLinks" href="https://en.wikipedia.org/wiki/Ireland">Wikipedia</a> pour en savoir encore plus sur l'Irlande!
    </p>
```

+ Ajoutez le code suivant à votre feuille de style, puis exécutez votre code pour voir vos jolis liens en action.

```css
  .niceLinks {
    text-decoration: none;
    color: #FFFAF0;
  }
  .niceLinks:hover {
    color: #00FF7F;
  }
```

+ Pourquoi ne pas ajouter l'attribut `class = "niceLinks"` à tous les liens de votre barre de menu?

Vous pouvez combiner toutes ces astuces avec des animations aussi!

+ Trouvez le bloc CSS pour l'image de Tito à nouveau (ou quelle que soit l'image sur laquelle vous travailliez plus tôt). Ajoutez le code suivant à votre fichier de feuille de style:

```css
  #titoPicture {
    border-radius: 100%;
    width: 100px;
  }
  #titoPicture:hover {
    animation-name: rollOver;
    animation-duration: 1s;
    animation-iteration-count: 1;
  }
  @keyframes rollOver {
    0% {
      transform: rotate(0deg);
    }
    100% {
      transform: rotate(-360deg);
    }
  }
```

+ Pouvez-vous deviner ce qui va se passer?

+ Maintenant, criez "Roll over!" lorsque vous déplacez le curseur sur l'image!

--- challenge ---

## Défi: faire des liens arc-en-ciel lumineux

+ Pouvez-vous utiliser l'animation `rainbowGlow` de la carte précédente pour que les liens de votre menu continuent à changer de couleur lorsque le curseur les survole?

--- hints ---

--- hint ---

Voici le code de l'animation `rainbowGlow`. Il comporte cinq étapes définies et définit une couleur de texte différente à chaque étape. Vous pouvez en ajouter plus ou les modifier comme vous le souhaitez!


```css
    @keyframes rainbowGlow {
        0% {
            color: #00BFFF;
        }
        25% {
            color: #00FF7F;
        }
        50% {
            color: #eeeeaf;
        }
        75% {
            color: #eeafee;
        }
        100% {
            color: #00BFFF;
        }
    }
```

--- /hint ---

--- hint ---

Pour animer quelque chose, vous ajoutez les trois propriétés `animation` à ses règles de style comme vous l'avez fait ci-dessus. Assurez-vous toujours que le nom `animation` correspond au nom de l'animation que vous souhaitez utiliser.

--- /hint ---

--- hint ---

Vous pouvez ajouter `effets hover` directement au menu `nav` comme ceci:


```css
  nav ul li a:hover {
    animation-name: rainbowGlow;
    animation-duration: 1.5s;
    animation-iteration-count: infinite;
  }
```

Ou, si vous voulez faire d' autres liens sur votre site Web couleurs arc -en -flash trop, vous pouvez ajouter l'animation au `.niceLinks` classe à la place, comme ceci:

```css
  .niceLinks:hover {
    color: #00BFFF;
    animation-name: rainbowGlow;
    animation-duration: 1.5s;
    animation-iteration-count: infinite;
  }
```

--- /hint ---

--- /hints ---

--- /challenge ---

![](images/badge-footer-image-html-intermed.png)