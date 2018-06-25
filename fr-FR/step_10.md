## Animation

Saviez-vous que vous pouvez utiliser CSS pour faire bouger les choses? Vous apprendrez comment sur cette carte!

+ Avant de commencer, assurez-vous que vous avez une image sur votre site Web avec un `id` et un bloc CSS correspondant qui définit les `largeur` à `100px`. Je vais avec l'image de Tito d'avant, et mon bloc CSS ressemble à ceci:

```css
    #titoPicture {border-radius: 100%; largeur: 100px; }
```

+ Allez au bas de votre fichier CSS et ajoutez le code suivant:

```css
    @keyframes myFirstAnimation {de {width: 100px; } à {width: 300px; }}
```

Ce code crée une animation appelée `myFirstAnimation` que vous pouvez ajouter à n'importe quel élément de votre site Web. Que pensez-vous qu'il va faire?

+ Trouvez vos règles CSS pour l'image et ajoutez les trois propriétés suivantes:

```css
    nom-animation: myFirstAnimation; animation-durée: 2s; animation-itération-compte: 1;
```

+ Maintenant, regardez ce qui se passe sur votre page web! Essayez différentes valeurs pour `animation-itération-count` pour voir ce qu'il fait.

+ Essayons une autre animation! Ajoutez le code suivant à la fin de votre fichier CSS:

```css
    @keyframes rainbowGlow {0% {color: # FFD700; } 50% {couleur: # 663399; } 100% {color: # FFD700; }}
```

+ Trouvez maintenant les règles CSS `#myCoolText` et ajoutez le code d'animation:

```css
    #myCoolText {color: # 003366; frontière: 2px ridge #ccffff; rembourrage: 15px; text-align: centre; nom-animation: rainbowGlow; animation-durée: 1.5s; animation-itération-compte: 1; }
```

Lorsque vous utilisez **pourcentage** au lieu de `de` et `à`, vous pouvez définir des valeurs intermédiaires ainsi que des valeurs de début et de fin. Vous pouvez définir autant de valeurs intermédiaires que vous le souhaitez en utilisant différentes valeurs de pourcentage allant de `0` à `100`.

+ Changez la valeur de `animation-itération-compte` à `infini`. Voyez si vous pouvez deviner ce qui va se passer avant de le tester!

+ Essayez différentes valeurs pour `animation-durée` pour accélérer ou ralentir votre animation.

+ Un dernier tour! Ajoutez ce code d'animation:

```css
    @keyframes slide {0% {background-position-x: 0; } 100% {background-position-x: 600vw; }}
```

+ Maintenant , trouver les `#frontPage` règles CSS que vous avez écrit plus tôt et de les changer pour:

```css
    # frontPage {arrière-plan: gradient-répétitif-linéaire (-45deg, rouge 0%, jaune 7,14%, lime 14,28%, cyan 21,42%, cyan 28,56%, bleu 35,7%, magenta 42,84%, rouge 50%); taille de fond: 600vw 600vw; animation: diapositive 10s infinie linéaire vers l'avant; }
```

Ne vous inquiétez pas de comprendre tout le code ci-dessus ... asseyez-vous et profitez-en !!

Pour en savoir plus sur les choses que vous pouvez faire avec l' animation, visitez [cette page web](http://dojo.soy/html2-css-animation){: target = "_ blank"}. S'amuser!

Sur la prochaine carte, vous apprendrez comment faire des choses cool quand vous passez le curseur de la souris sur les choses!