# Les conteneurs

## Ex : Un portfolio en ligne.

On va utiliser l'exercice du cours d'Open Class Room ( site génial, d'ou je tire la plupart de mes cours, allez y, foncez y ! )

https://openclassrooms.com/fr/courses/7542506-creez-des-sites-web-responsives-avec-bootstrap-5/7546687-decomposez-la-structure-des-pages

Analysons cette maquette :


![[portfolio.png]](./img/portfolio.png)

En résumé, notre structure est composée de :

-   un menu ;    
-   une première section de présentation ;
-   une seconde concernant les compétences techniques ;    
-   une troisième section pour présenter des projets ;    
-   une dernière section avec la possibilité d'une prise de contact ;    
-   un footer.

## Doc' 

Ayez la doc toujours sous la main :
https://getbootstrap.com/docs/5.1/layout/containers/

## container

Commençons par l'élément de mise en page le plus basique dans Bootstrap, le **conteneur** (_container_). Envelopper vos contenus dans un élément   `<div>`  avec la classe   `.container`  permet de centrer votre contenu à l’écran en y ajoutant des marges horizontales automatiques. 

De ce fait, la classe   `.container`  permet d’aérer la lecture horizontale du contenu de votre site web.

Si vous voulez que le contenu occupe toujours 100 % de la largeur de l’écran, vous pouvez utiliser la classe   `.container-fluid`    à la place. Cela permet d’enlever les marges horizontales appliquées par défaut par le framework.

Depuis Bootstrap 5, de nouveaux containers sont arrivés :  `.container-{breakpoint}`  (exemple :   `.container-lg`). Ils permettent d’adapter votre “container” en fonction de la taille d’écran de l’utilisateur. Rendez-vous sur la [documentation Bootstrap 5](https://getbootstrap.com/docs/5.0/layout/containers/) : 

	Bootstrap vient avec trois différents containers:

	-   `.container`, qui indique une largeur maximale `max-width` pour chaque 'responsive breakpoint'
	-   `.container-fluid`, qui est `width: 100%` pour tous les breakpoints
	-   `.container-{breakpoint}`, qui est `width: 100%` jusqu'a ce qu'on arrive au breakpoint désiré
	
Autrement dit, on peut lui dire : Sur un grand écran, je veux de belles marges. Sur un téléphone, on colle tout au bords des écrans.

### Les grilles

Bootstrap 5 possède un système de grille puissant et flexible qui permet de créer tous les types de mise en page. 

Cette grille utilise une série de **lignes** (en anglais, _row_) et de **colonnes** (en anglais, _column_) pour mettre en page le contenu. Une ligne permet d’envelopper une ou plusieurs colonnes qui intègrent du contenu.

```html
<div class="container">
  <div class="row">
    <div class="col">
      Première colonne
    </div>
    <div class="col">
      Deuxième colonne
    </div>
  </div>
</div>
```

Bootstrap 5 possède une grille à 12 colonnes. Dans ce cas précis, Bootstrap attribuera **automatiquement** la moitié des colonnes à chacun des éléments   `<div>`  de classe   `.col`, donnant alors une largeur de 6 colonnes par  `<div>`.

![[12col.jpg]]

Vous pouvez avoir une mise en page qui ne possède pas de colonnes de taille égale. Supposons que vous disposiez d'une ligne, que vous vouliez qu'une colonne de cette ligne occupe deux tiers de sa largeur, et qu'une autre colonne occupe le tiers restant.

![[2tiers.jpg]]

```html
<div class="container">
  <div class="row">
    <div class="col-8">
      Première colonne
    </div>
    <div class="col-4">
      Deuxième colonne
    </div>
  </div>
</div>
```

### Classes utilitaires

Les classes utilitaires sont des classes créées par Bootstrap 5, qui permettent d’ajouter des propriétés CSS à vos éléments, telles que des :

-   `background-color`  (comme  `.bg-light`) ;
-   `margin`  (comme  `.m-5`) ;
-   `padding`  (comme  `.p-5`) ;
-   `border`  (comme  `.border-top`).
    
Entre autres ! Vous pouvez consulter toutes les classes sous la liste “Utilities” dans la [documentation de Bootstrap](https://getbootstrap.com/docs/5.0/utilities/).


### A vous de jouer !

![[first_exo.jpg]]