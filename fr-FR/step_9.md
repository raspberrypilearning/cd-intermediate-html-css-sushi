## Animation

Savais-tu que tu peux utiliser CSS pour faire bouger les choses? Tu apprendras comment sur cette carte!

+ Avant de commencer, assure-toi d’avoir une photo sur ton site Web avec un `id` et un bloc CSS correspondant qui définit le `width` à `100px` . J'y vais avec l'image de Tito d'avant, et mon bloc CSS ressemble à ceci :

```css
    #titoPicture {
        border-radius: 100%;
        width: 100px;
    }
```

+ Va au bas de ton fichier CSS et ajoute le code suivant:

```css
    @keyframes myFirstAnimation {
        from {
            width: 100px;
        }
        to {
            width: 300px;
        }
    }
```

Ce code crée une animation appelée `myFirstAnimation` que tu peux ajouter à n’importe quel élément de ton site Web. Que penses-tu que ça fera?

+ Recherche tes règles CSS pour l'image et ajoute les trois propriétés suivantes:

```css
    animation-name: myFirstAnimation;
    animation-duration: 2s;
    animation-iteration-count: 1;
```

+ Maintenant, regarde ce qui se passe sur ta page Web! Essaie différentes valeurs pour `animation-iteration-count` pour voir ce qu'il fait.

+ Essayons une autre animation! Ajoute le code suivant à la fin de ton fichier CSS:

```css
    @keyframes rainbowGlow {
        0% {
            color: #FFD700;
        }
        50% {
            color: #663399;
        }
        100% {
            color: #FFD700;
        }
    }
```

+ Maintenant, trouve les règles CSS `#myCoolText` précédemment et ajoute dans le code d'animation:

```css
    #myCoolText {        
        color: #003366;
        border: 2px ridge #ccffff;
        padding: 15px;
        text-align: center;
        animation-name: rainbowGlow;
        animation-duration: 1.5s;
        animation-iteration-count: 1;
    }
```

Lorsque tu utilises les **valeurs en pourcentage** au lieu de `from` et `to` , tu peux définir des valeurs intermédiaires ainsi que des valeurs de début et de fin. Tu peux définir autant de valeurs intermédiaires que tu le souhaites en utilisant différentes valeurs de pourcentage de `0` jusqu'à `100`.

+ Change la valeur de `animation-iteration-count` sur`infini`. Vois si tu peux deviner ce qui se passera avant de le tester!

+ Essaie différentes valeurs pour `animation-duration` pour accélérer ou ralentir ton animation.

+ Un dernier tour! Ajoute ce code d'animation:

```css
    @keyframes slide {
        0% {
            background-position-x: 0;
        }
        100% {
            background-position-x: 600vw;
        }
    }
```

+ Maintenant, trouve les règles CSS `#frontPage` que tu as écrites précédemment et les changer en:

```css
    #frontPage {
        background: repeating-linear-gradient(-45deg, red 0%, yellow 7.14%, lime 14.28%, cyan 21.42%, cyan 28.56%, blue 35.7%, magenta 42.84%, red 50%);
        background-size: 600vw 600vw;
        animation: slide 10s infinite linear forwards;
    }
```

Ne t’inquiète pas de comprendre tout le code ci-dessus... assieds-toi et profite !!

Pour en savoir plus sur l’animation, visite [cette page Web](http://dojo.soy/html2-css-animation) {:target= "_ blank"}. Amuse-toi bien!

Sur la carte suivante, tu apprendras à créer des choses intéressantes quand tu survoles des objets avec le curseur de ta souris!