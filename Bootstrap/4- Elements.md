# Retour sur les classes utilitaires

Quand on observe les classes utilitaires de Bootstrap, on remarque qu’elles ne sont pas construites n’importe comment. Bien souvent, la classe utilitaire est composée des initiales de la propriété CSS qu’elle représente, **concaténées** (collées) à la valeur qu’elle ajoute.

Pour les propriétés liées au texte, il existe plusieurs classes que vous pouvez utiliser pour modifier l’épaisseur (  `font-weight`  ) ou le style (  `font-style`  ) du texte :

Vous remarquez que comme pour toute autre classe utilitaire, nous pouvons ajouter des breakpoints (points d’arrêt) pour rendre le texte responsive.

Dans le cas de notre   `h1`, nous allons lui ajouter la classe   `.fw-bold`, ce qui veut dire  `font-weight: bold;`. En suivant cette logique, on peut ajouter la classe suivante,  `.fw-light`, à notre  `h2`, ce qui a pour effet de réduire l’épaisseur de la police d’écriture.

```
<h1 class="fw-bold">Je suis John Doe Développeur et Designer Web</h1>
```

```
<h2 class="fw-light">Bienvenue dans mon univers créatif</h2>
```

Vous pouvez voir toutes les classes utilitaires liées aux propriétés du texte dans [la documentation Bootstrap](https://getbootstrap.com/docs/5.0/utilities/text/#font-weight-and-italics).

![[font.png]]

### Typographie responsive

Toujours dans la même logique que les colonnes, il est possible d’ajouter des modificateurs de classes liés aux breakpoints de Bootstrap.

Pas de panique, Bootstrap a fait ça bien, et vous les connaissez déjà ! Il s’agit des   `{-xs, -sm, -md, -xl, -xxl}`. Et comme pour les colonnes, la construction suit la même logique :   `.{propriété}-{modificateur}-{valeur}`.

Par exemple, vous ajoutez les classes  `.fs-3 .fs-md-2`  à vos  `h3`  pour diminuer leur taille sur mobile et l’augmenter à partir des écrans moyens.

#### Alignement :

```html
<p class="text-start">Start aligned text on all viewport sizes.</p>
<p class="text-center">Center aligned text on all viewport sizes.</p>
<p class="text-end">End aligned text on all viewport sizes.</p>

<p class="text-sm-start">Start aligned text on viewports sized SM (small) or wider.</p>
<p class="text-md-start">Start aligned text on viewports sized MD (medium) or wider.</p>
<p class="text-lg-start">Start aligned text on viewports sized LG (large) or wider.</p>
<p class="text-xl-start">Start aligned text on viewports sized XL (extra-large) or wider.</p>
```

Wrapping, overfllow, word break :

https://getbootstrap.com/docs/5.0/utilities/text/#text-alignment

## Les boutons

![[button.png]]

```html
<button type="button" class="btn btn-primary">Bouton</button>
<a class="btn btn-primary" href="#" role="button">Lien</a>
```


## Les icones

https://icons.getbootstrap.com/

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.5.0/font/bootstrap-icons.css">
```

## On continu le portfolio ? :)