# Les conteneurs

## Ex : Un portfolio en ligne.

On va utiliser l'exercice du cours d'Open Class Room ( site génial, d'ou je tire la plupart de mes cours, allez y, foncez y ! )

https://openclassrooms.com/fr/courses/7542506-creez-des-sites-web-responsives-avec-bootstrap-5/7546687-decomposez-la-structure-des-pages

Analysons cette maquette :

![[portfolio.png]]

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
