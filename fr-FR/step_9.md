## Ajuster automatiquement la taille

Jusqu'à présent, vous utilisiez **pixel** pour définir la taille des objets, par exemple `10px`. Sur cette carte, vous apprendrez d'autres mesures que vous pouvez utiliser.

+ Aller à `index.html` et trouver l'élément `img` avec l'image de Tito, ou trouver un autre tag `img` sur votre site Web.

+ Supprimez l'attribut `width` s'il existe et donnez à l'élément un `id` s'il n'en a pas déjà un.

```html
  <img src="tito.png" id="titoPicture" alt="Tito the dog" />
```

+ Dans votre fichier CSS, définissez la propriété `width` pour votre image comme indiqué ci-dessous (vous devrez peut-être créer le bloc CSS avec le sélecteur `id` si vous ne l'avez pas déjà fait sur une carte précédente).

```css
  #titoPicture {width: 50%; border-radius: 100%; }
```

Note: 50% (50%) est **moitié**.

+ Essayez de redimensionner la fenêtre de votre navigateur et regardez ce qui arrive à l'image.

Vous devriez voir que l'image devient de plus en plus petite lorsque vous agrandissez et agrandissez la fenêtre. C'est parce qu'il occupe 50% de la largeur de l'élément **principal** (qui est à peu près la largeur de la page).

## \--- effondrer \---

## title: Comment ça marche?

Lorsque vous définissez la taille de quelque chose en pixels, vous définissez une taille exacte et elle ne change pas. Ceci est appelé une mesure **absolue**.

Une autre façon de définir la taille des choses est d'utiliser **mesures relatives à** , de sorte que la taille dépend de la façon dont les grands éléments sont comparés les uns aux autres. Ensuite, chaque fois qu'une chose change de taille, tout le reste changera automatiquement la taille et de garder les mêmes **proportions**.

Lorsque vous utilisez **par rapport** mesures, il est important de savoir ce que le **parent** de votre élément est. Le parent est la chose que votre élément est à l'intérieur de, et c'est ce que la mesure sera en relation avec. Par exemple, le parent de l'image ci-dessus est l'élément `article` , car l'élément `img` trouve entre les balises `<article></article>`.

Si vous définissez la `largeur` d'un élément à `100%`, qui fera ce soit la même largeur que le conteneur parent il se trouve.

\--- /effondrer \---

+ Expérimentez avec différents nombres devant le `%`.