## Organiser votre page

Jusqu'à présent , vous avez utilisé **titres** et **paragraphes** à rendre votre **contenu** regard bien rangé et facile à lire. Rendons-le encore plus organisé en regroupant les choses ensemble.

## \--- effondrer \---

## title: Qu'est-ce que le contenu?

**Contenu** est tout ce qui se trouve sur votre page Web, comme le texte et les textes.

\--- /effondrer \---

+ Allez dans le fichier `attractions.html` (ou l'une de vos propres pages si vous n'utilisez pas l'exemple de projet) et, près du sommet, juste **sous** l'étiquette d'ouverture `<main>` , tapez ce qui suit sur une nouvelle ligne : 

```html
  <main>
    <article>
```

+ Si votre éditeur a automatiquement ajouté une balise de fermeture `</article>` pour vous, supprimez-la.

+ Au bas du fichier, juste **au-dessus de** la balise de fermeture `</main>` , ajoutez une nouvelle ligne et fermez l'élément `article`:

```html
    </article>
  </main>
```

Votre `principal` élément devrait ressembler à quelque chose comme ceci maintenant (vous pourriez avoir un contenu différent entre les `étiquettes de l'article` bien sûr):

```html
  <main>
    <article>
      <h1>Mes endroits préférés à voir en Irlande</h1>
        <h2>Les falaises de Moher</h2>
        <p>
        Les falaises de Moher se trouvent dans le comté de Clare, d'où je viens. Regardez comme ils sont cool!</p>
        <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
        <h2>Île d'Achill</h2>
        <p>Il s'agit d'une grande île au large des côtes du comté de Mayo. Il a un paysage sauvage et magnifique de montagnes, de tourbières et de falaises.
        </p>
        <img src="achill.JPG" width="200px" />
    </article>
  </main>
```

+ Maintenant, regardez le contenu de votre `article` et essayez de le diviser en sections. Mettez cette nouvelle paire d'étiquettes autour de chaque bit: `<section> </section>`. Voici un exemple de ce à quoi cela pourrait ressembler:

```html
  <article>
    <h1>Mes endroits préférés à voir en Irlande</h1>
    <section>
      <h2>Les falaises de Moher</h2>
      <p>
      Les falaises de Moher se trouvent dans le comté de Clare, d'où je viens. Regardez comme ils sont cool!</p>
      <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
    </section>
    <section>
      <h2>Île d'Achill</h2>
      <p>Il s'agit d'une grande île au large des côtes du comté de Mayo. Il a un paysage sauvage et magnifique de montagnes, de tourbières et de falaises.
      </p>
      <img src="achill.JPG" width="200px" />
    </section>
  </article>
```

## \--- effondrer \---

## title: Quels sont les nouveaux tags?

Pensez à ces nouveaux éléments comme **conteneurs**. Ils sont utilisés pour regrouper les choses ensemble. C'est un peu comme organiser des choses dans des boîtes et des étagères dans votre maison!

Cela rend votre site convivial pour les lecteurs d'écran, vous donne plus de contrôle sur la mise en page, et, comme vous le verrez, il vous permet de vraiment faire preuve de créativité avec le style.

Tout peut aller entre les balises. Habituellement, ce sera plus d'un élément, mais ce n'est pas obligatoire. Il peut s'agir d'éléments HTML de toute sorte. Ce que vous faites est de dire au navigateur que tout ce qui se trouve entre ces balises appartient ensemble.

### Article

L'élément `article` est un conteneur pour tout un contenu, dans ce cas un ensemble d'informations sur les attractions en Irlande. Si vous avez différents éléments de contenu qui ne sont pas liés, vous devez placer chacun d'eux dans son propre élément `article` au lieu de placer un ensemble de balises autour du lot entier.

### Section

L'élément `section` vous permet de diviser le contenu associé en morceaux plus petits et de placer chaque morceau dans son propre conteneur.

### D'autres existent aussi!

Ce ne sont pas les seuls éléments de conteneur en HTML. Si vous avez déjà créé un menu et que vous l'avez mis entre `<nav> </nav>` , c'est un autre exemple de type de conteneur. Donc, sont `<main> </main>` et `<header> </header>` - pouvez-vous penser à plus?

\--- /effondrer \---

\--- défi \---

Votre page Web n'a peut-être pas encore l'air différente, mais une fois que le contenu a été organisé en balises de conteneur, vous serez en mesure de faire des choses intéressantes avec CSS. Rappelez-vous que le HTML contrôle l'organisation de votre site Web et que le contrôle CSS en détermine l'apparence.

## Défi: organisez votre site web

+ Essayez d'organiser tout le contenu de votre site Web en utilisant les conteneurs `article` et `section` de cette façon. 

\--- astuces \---

\--- indice \---

Regardez la page Food du projet exemple. Vous verrez que j'ai ajouté un `article` avec un tas de `étiquettes de section` dans le fichier `food.html`:

```html
  <main>
    <article>
      <h1>Food in Ireland</h1>
      <p>
        Voici quelques uns de mes plats irlandais préférés!
      </p>  
      <section>
        <h2>Petit-déjeuner irlandais traditionnel</h2>
        <p>
          Un petit-déjeuner «irlandais complet» se compose de saucisses, de rashers (bacon), d'œufs, de boudin noir, de boudin blanc et de pain grillé.
        </p>
        <p>
          Souvent, il y aura une tomate grillée ainsi que des champignons et des fèves au lard.
        </p>
        <p>
          Et bien sûr, pas de petit-déjeuner complet sans une bonne tasse de thé!
        </p>
      </section>

      <section>
        <h2>Bangers and Mash</h2>
        <p>
          Ce classique des saucisses, de la purée de pommes de terre et de la sauce n'est pas unique en Irlande, mais ce qui le rend spécial, ce sont les saucisses irlandaises. La plupart des pays ont leur propre façon de faire des saucisses, et c'est une chose qui me manque à la maison si je pars en voyage!
        </p>
      </section>

      <section>
        <h2>Bacon et chou</h2>
        <p>
          Je ne pouvais pas faire une liste de plats irlandais sans inclure ce plat très traditionnel!
        </p>
        <p>
          Cela peut ne pas sembler très intéressant, mais ce repas copieux de jambon bouilli, de pommes de terre et de chou vert est savoureux et copieux.
          J'aime étouffer les pommes de terre dans le beurre, et j'aime aussi un peu de moutarde avec le bacon.
        </p>
        <p>
          Ma mère a toujours fait un cadeau spécial en faisant cuire le chou dans l'eau dans laquelle le jambon était bouilli.
        </p>
        <p>
          S'il y a des restes, vous pouvez en faire un autre de mes favoris: <strong>chou frit</strong>!
        </p>
      </section>
    </article>     
  </main>
```

\--- / indice \---

\--- /astuces \---

Sur la prochaine carte, vous allez créer un thème différent pour chaque page organisée en articles et sections!

\--- /défi \---