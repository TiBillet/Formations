## Les breakpoints

**une page responsive** est une page qui réagit à différentes tailles d'écran de l'utilisateur, en modifiant la mise en page des composants et du contenu à ajuster.

Une app ou un site web a besoin d'une mise en page pour des périphériques avec de grands écrans (ordinateurs de bureau), une autre pour des périphériques avec des écrans de taille moyenne (tablettes et petits ordinateurs portables) et enfin pour des périphériques plus petits (smartphones).

![[taille_breakpoints.png]](./img/taille_breakpoints.png)

**Un breakpoint (point d'arrêt)** est un point de discontinuité, modification ou interruption. Dans le contexte de conception et de développement frontend, un point d'arrêt est le point à partir duquel la mise en page change. Généralement, un nombre de pixels représente la largeur de la taille d’écran affichée à laquelle le point d'arrêt se produit.

![[breakscrean.jpg]](./img/breakscrean.jpg)

Pour appliquer les modificateurs de classes appropriés pour ces options de mise en page, il est important de comprendre qu'ils fonctionnent **par le haut**, c'est-à-dire de la plus petite taille d’écran vers la plus grande : C'est l'approche **mobile-first**.


Cela signifie que **si vous n'ajoutez pas de modificateur de classe relatif à une taille d’écran supérieure, Bootstrap affichera automatiquement** les éléments et composants de la grille dans les plus petits écrans, et conservera la même mise en page, même si la taille de l'écran augmente.

On commence par le plus petit, et on change si on indique plus grand.

```html
<div class="row">
      <div class="col-6 col-md-4 col-lg-3"></div>
      <div class="col-6 col-md-8 col-lg-9"></div>
</div>
```

## Gouttières
Les espacements entre les différentes colonnes de la grille sont appelés **gouttières** (_gutters_, en anglais).

![[gouttiere.jpg]](./img/gouttiere.jpg)

```html
<div class="container px-4">
    <div class="row gx-5">
        <div class="col">
            <div class="p-3 border bg-light">Custom column padding</div>
        </div>
        <div class="col">
            <div class="p-3 border bg-light">Custom column padding</div>
        </div>
    </div>
</div>
```

## Offset

Pour certains designs, vous aurez besoin de laisser l’équivalent d’une colonne (ou plus) vide entre 2 colonnes. Ce qui est le cas pour la partie Expertise de notre portfolio :

![[offset.png]](./img/offset.png)

```html
<div class="container">
    <div class="row">
        <div class=" col-md-4">.col-md-4</div>
        <div class="col-md-4 offset-md-4">.col-md-4 .offset-md-4</div>
    </div>
    <div class="row">
        <div class="col-md-3 offset-md-3">.col-md-3 .offset-md-3</div>
        <div class="col-md-3 offset-md-3">.col-md-3 .offset-md-3</div>
    </div>
    <div class="row">
        <div class="col-md-6 offset-md-3">.col-md-6 .offset-md-3</div>
    </div>
</div>
```


## A vous de jouer :)