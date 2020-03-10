## Apprends à Tito à se retourner!

Tu peux rendre ton site plus **interactif** en créant des trucs sympas lorsque tu survoles des objets avec le curseur de la souris!

+ Trouve tes règles CSS pour les éléments `img`, ou crée quelques un si tu n'en as pas. Ajoute une bordure, puis ajoute un nouveau bloc de règles juste en dessous:

```css
  img {
    border: 2px solid White;
  }
  img:hover {
    border: 2px dashed Navy;
  }
```

Tu viens d'utiliser un type spécial de bloc CSS appelé **pseudo-classe**.

--- collapse ---
---
title: Comment ça marche?
---

Une **pseudo-classe** est un peu différente d'une **classe** que tu peux créer toi-même. Tu peux la reconnaître par le `:`.

Les pseudo-classes sont intégrées aux éléments HTML: tu peux ajouter les règles de style `:hover` pour tout élément, classe ou sélecteur d' `id` dans ta feuille de style sans avoir besoin d'ajouter quoi que ce soit dans ton code HTML.

--- /collapse ---

+ Que penses-tu qu'il va se passer? Vérifie quelles pages de ton site Web contiennent des images (ajoute une image s'il n'y en a pas!), Puis déplace ton curseur sur une image pour le découvrir!

+ Utilisons cette nouvelles pseudo-classe `:hover` avec une classe CSS pour faire briller les liens lorsque tu les survoles! Ajoute un lien vers ta page Web et inclus un attribut pour spécifier le nom de la classe. N'oublie pas que les liens sont définis à l'aide de la balise `<a>`, comme suit:

```html
    <p>
      Visite la <a class="niceLinks" href="https://en.wikipedia.org/wiki/Ireland">page Wikipédia</a> pour en savoir plus sur l'Irlande!
    </p>
```

+ Ajoute le code suivant à ta feuille de style, puis exécute-le pour voir tes jolis liens en action.

```css
  .niceLinks {
    text-decoration: none;
    color: #FFFAF0;
  }
  .niceLinks:hover {
    color: #00FF7F;
  }
```

+ Pourquoi ne pas ajouter aussi l'attribut `class="niceLinks"` à tous les liens dans ta barre de menu?

Tu peux également combiner toutes ces astuces avec des animations!

+ Trouve le bloc CSS pour l'image de Tito à nouveau (ou l'image avec laquelle tu as travaillé tout à l'heure). Ajoute le code suivant à ton fichier de feuille de style:

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

+ Peux-tu deviner ce qui va arriver?

+ Maintenant crie "rouler !" lorsque tu déplaces le curseur sur l'image!

--- challenge ---

## Défi: faire des liens arc-en-ciel lumineux

+ Peux-tu utiliser l'animation `rainbowGlow` de la carte précédente pour que les liens de ton menu ne cessent de changer de couleur lorsque le curseur les survole?

--- hints ---


--- hint ---

Ci-dessous le code pour l'animation `rainbowGlow`. Il comporte cinq étapes définies et définit une couleur de texte différente à chaque étape. Tu peux en ajouter ou les modifier à ta guise!

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

Pour animer quelque chose, tu ajoutes les trois propriétés `animations` à ses règles de style comme tu l'as fait ci-dessus. Assure-toi toujours que le `animation-name` correspond au nom de l'animation que tu souhaites utiliser.

--- /hint ---

--- hint ---

Tu peux ajouter les effets `hover` directement au menu `nav` comme ceci:

```css
  nav ul li a:hover {
    animation-name: rainbowGlow;
    animation-duration: 1.5s;
    animation-iteration-count: infinite;
  }
```

Ou, si tu souhaites ajouter d'autres liens sur ton site Web couleurs clignotantes arc-en-ciel , tu peux ajouter l'animation à la classe `.niceLinks` à la place, comme ceci:

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


***
Ce projet a été traduit par des bénévoles:

Jonathan Vannieuwkerke

Michel Arnols

Grâce aux bénévoles, nous pouvons donner aux gens du monde entier la chance d'apprendre dans leur propre langue. Vous pouvez nous aider à atteindre plus de personnes en vous portant volontaire pour la traduction - plus d'informations sur [rpf.io/translate](https://rpf.io/translate).