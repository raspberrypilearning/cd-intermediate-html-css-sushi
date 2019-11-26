## Ajuster automatiquement la taille

Jusqu'à présent, tu utilisais **pixels** pour définir la taille des objets, par exemple `10 pixels`. Sur cette carte, tu apprendras d’autres mesures que tu peux utiliser.

+ Va sur `index.html` et trouve l'élément `img` avec l’image de Tito, ou trouve une autre balise `img` sur ton site web.

+ Supprime l'attribut `width` si c'est là, et donne à l'élément un `id` s'il n'en a pas déjà un.

```html
  <img src="tito.png" id="titoPicture" alt="Tito the dog" />
```

+ Dans ton fichier CSS, définis la propriété `width` de ton image, comme indiqué ci-dessous (tu devrais peut-être créer le bloc CSS avec le sélecteur `id` si tu ne l'as pas déjà fait sur une carte précédente).

```css
  #titoPicture {
    width: 50%;
    border-radius: 100%;
  }
```

Note : 50% (50 pour cent) est la **moitié**.

+ Essaie de redimensionner la fenêtre de ton navigateur et observe ce qu'il advient de l'image.

Tu devrais voir que l'image devient plus grande et plus petite lorsque tu rends la fenêtre plus grande et plus petite. C’est parce qu’il occupe 50% de la largeur de l'élément **main** (qui correspond approximativement à la largeur de la page).

## \--- collapse \---

## title: Comment ça marche?

Lorsque tu définis la taille d'un élément en pixels, tu définis une taille exacte qui ne change pas. Ceci s'appelle une mesure **absolue**.

Une autre façon de définir la taille des choses consiste à utiliser des mesures **relatives**, de sorte que la taille dépend de la taille des éléments comparés les uns aux autres. Ensuite, chaque fois que quelque chose change de taille, tout le reste changera automatiquement de manière à garder les mêmes **proportions**.

Lorsque tu utilises les mesures **relatives**, il est important de savoir ce que le **parent** de ton élément est. Le parent est ce dont ton élément est à l'intérieur et c'est ce à quoi la mesure se rapportera. Par exemple, le parent de l'image ci-dessus est l'élément `article` , car l'élément `img` se situe entre les balises `<article></article>`.

Si tu définis le `width` d'un élément à `100%` , cela lui donnera la même largeur que le conteneur parent dans lequel il se trouve.

\--- /collapse \---

+ Expérimente avec différents nombres devant le `%`.