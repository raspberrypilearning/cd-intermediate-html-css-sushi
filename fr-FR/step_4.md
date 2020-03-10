## Organiser ta page

Jusqu'à présent, tu as utilisé **en-têtes** et **paragraphes** pour rendre ton **contenu** plus organisé et facile à lire. Rendons cela encore plus organisé en regroupant les choses.

--- collapse ---
---
title: Qu'est-ce que le contenu?
---

**Le contenu** contient tout ce qui se trouve sur ta page Web, par exemple du texte et des images.

--- /collapse ---

+ Va au fichier `attractions.html` (ou à l'une de tes propres pages si tu n'utilises pas le projet exemple) et, tout en haut, **sous** la balise d'ouverture `<main>`, tape ce qui suit sur une nouvelle ligne: 

```html
  <main>
    <article>
```

+ Si ton éditeur a ajouté automatiquement dans une balise de fermeture `</article>` pour toi, supprime-la.

+ Au bas du fichier, juste **au dessus** la balise de fermeture `</main>`, ajoute une nouvelle ligne et ferme l'élément `article`:

```html
    </article>
  </main>
```

Ton élément `main` devrait ressembler à ceci maintenant (tu pourrais avoir un contenu différent entre les balises `article` bien sûr):

```html
  <main>
    <article>
      <h1>Mes endroits favoris à voir en Irlande</h1>
        <h2>Les Falaises de Mother</h2>
        <p>
        Les Falaises de Mother se trouvent dans le comté de Clare, d'où je viens. Regarde comme ils sont cool!</p>
        <1 />
        <h2>Île Achill</h2>
        <p>Il s’agit d’une grande île au large du comté de Mayo. Il y a un magnifique
        paysage sauvage de montagnes, de tourbières et de falaises.
        </p>
        <img src="achill.JPG" width="200px" />
    </article>
  </main>
```

+ Maintenant, regarde le contenu de ton `article` et essaie de le diviser en sections. Place cette nouvelle paire de balises autour de chaque bit: `<section> </section>`. Voici un exemple de ce à quoi cela pourrait ressembler:

```html
  <article>
    <h1>Mes endroits favoris à voir en Irlande</h1>
    <section>
      <h2>Les Falaises de Mother</h2>
      <p>
      Les Falaises de Mother se trouvent dans le comté de Clare, d'où de viens. Regarde comme elles sont cool!</p>
      <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px" />
    </section>
    <section>
      <h2>Île Achill</h2>
      <p>Il s'agit d'une grande île au large de la côte du compté de Mayo. Il y a un magnifique
        paysage sauvage de montagnes, de tourbières et de falaises.
      </p>
      <img src="achill.JPG" width="200px" />
    </section>
  </article>
```

--- collapse ---
---
title: À quoi servent les nouvelles balises?
---

Pense à ces nouveaux éléments en tant que **conteneurs**. Ils sont utilisés pour regrouper les choses ensemble. C'est un peu comme organiser des choses dans des boîtes et des étagères chez toi!

Cela rend ton site Web convivial pour les lecteurs d'écran, te donne plus de contrôle sur la mise en page et, comme tu le verras, il te permet d'être vraiment créatif avec le style.

Tout peut aller entre les balises. Habituellement, il y aura plus d'un élément, mais ce n'est pas obligatoire. Il peut s'agir d'éléments HTML de tout type. Ce que tu fais, c'est dire au navigateur que tout ce qui est entre ces balises appartient ensemble.

### Article

L'élément `article` est un conteneur pour un contenu entier, dans ce cas un ensemble d'informations sur les attractions en Irlande. Si tu as des bits de contenu différents qui ne sont pas liés, tu devrais mettre chacun dans son propre élément `article` au lieu de mettre un ensemble de balises autour du lot.

### Section

L'élément `section` te permet de diviser le contenu lié en petits morceaux et de mettre chaque morceau dans son propre conteneur.

### D'autres existent aussi!

Ce ne sont pas les seuls éléments conteneurs en HTML. Si tu as déjà créé un menu, puis le placer entre les balises `<nav> </nav>`, c'est un autre exemple d'un type de conteneur. Voici `<main> </main>` et `<header> </header>` — peux-tu m'en donner plus?

--- /collapse ---

--- challenge ---

Ta page Web ne sera peut-être pas si différente, mais une fois que le contenu aura été organisé en balises de conteneur, tu pourras faire des choses intéressantes avec CSS. N'oublie pas que HTML contrôle l'organisation de ton site Web et que CSS en définit l'apparence.

## Défi: organiser ton site web

+ Essaie d'organiser tout le contenu de ton site Web à l'aide des conteneurs `article` et `section` comme ceci. 

--- hints ---


--- hint ---

Regarde la page Nourriture du projet exemple. Tu verras que j'ai ajouté un `article` avec un tas de balises `section` dans le fichier `food.html`:

```html
  <main>
    <article>
      <h1>Nourriture en Irlande</h1>
      <p>
        Ce sont mes aliments irlandais préférés!
      </p>  
      <section>
        <h2>Petit déjeuner irlandais traditionnel</h2>
        <p>
          Un petit déjeuner "complet irlandais" est composé de saucisses, lards (bacon),
          œufs, boudin noir, boudin blanc et pain grillé.
        </p>
        <p>
          Souvent, il y aura une tomate grillée ainsi que des champignons,
          et des haricots cuits.
        </p>
        <p>
          Et bien sûr, aucun petit déjeuner n'est complet sans une bonne tasse
          de thé!
        </p>
      </section>

      <section>
        <h2>Saucisses-purée</h2>
        <p>
          Ce classique de saucisses, de purée de pommes de terre et sauce n'est pas
          unique à l'Irlande, mais ce qui le rend spécial ce sont les saucisses irlandaises
          . La plupart des pays ont leur propre façon de faire des saucisses,
        et c'est une chose qui me manque chez moi si je suis en voyage!
        </p>
      </section>

      <section>
        <h2>Bacon et Choux</h2>
        <p>
          Je ne pourrais pas faire une liste de nourriture irlandaise sans inclure
          ce plat très traditionnel!
        </p>
        <p>
          ça ne parait pas très intéressant, mais ce repas copieux de
          jambon bouilli, pommes de terre et chou vert est savoureux et nourrissant.
          J'adore étouffer les pommes de terre au beurre et j'aime aussi un
             peu de moutarde avec le bacon.
        </p>
        <p>
          Ma maman l'a toujours rendu plus spécial en cuisant le chou dans
          l'eau dans laquelle le jambon a été bouilli.
        </p>
        <p>
          S'il y a des restes, tu peux en faire un autre de mes
          favoris: <strong>chou frit</strong>!
        </p>
      </section>
    </article>     
  </main>
```

--- /hint ---

--- /hints ---

Sur la carte suivante, tu vas concevoir un thème différent pour chaque page, organisé en articles et en sections!

--- /challenge ---