# Le composant card

Les _cards_ en anglais (“cartes” en français) sont un type d’élément d’**interface utilisateur** très populaire. Presque tous les frameworks CSS ont leur propre système de cards pour permettre aux développeurs de proposer un **affichage structuré** des informations de leur site.

https://getbootstrap.com/docs/5.0/components/card/

En parcourant rapidement la page, nous pouvons voir qu’il existe plusieurs types de cartes sur Bootstrap 5. La diversité des affichages permet de répondre à une multitude de **besoins** et de **cas d’usage spécifiques** (galerie photo, résumé de produits e-commerce, etc). Et comme d’habitude, il est toujours possible de pousser les composants encore plus loin grâce aux classes utilitaires.

Dans notre cas, nous allons utiliser l’affichage le plus populaire, c'est-à-dire le premier exemple de la doc Bootstrap : image, titre, texte, bouton.

```html
<div class="card">
    <img src="..." class="card-img-top" alt="...">
    <div class="card-body">
        <h5 class="card-title">Card title</h5>
        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
        <a href="#" class="btn btn-primary">Go somewhere</a>
    </div>
</div>
```

Nous pouvons voir que le composant suit une architecture donnée :

-   Une `div`  globale avec une classe du nom du composant (l’attribut style de l’exemple Bootstrap n’est pas à garder). 
    
-   À l’intérieur de cette `div`, nous trouvons une  `img`  ainsi qu’une autre  `div`  avec la classe  `card-body`. 
    
-   Ce dernier `div.card-body`  indique l’emplacement du corps de la carte, dans lequel on retrouve le  `card-title`, le  `card-text`  et notre bouton.
    

Il est très important de **respecter** cette structure pour obtenir le résultat escompté.

## Images aléatoires :

https://picsum.photos/300/150?random=1

## Example :

```html

	<section class="my-5">
		<div class="container">
			<div class="row">
					
				<div class="card col-12 col-md-6 col-lg-4 p-1">
				  <img src="card1-300.jpg" class="card-img-top rounded-3" alt="...">
				  <div class="card-body">
				    <h5 class="card-title">Card title</h5>
				    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
				    <a href="#" class="btn btn-primary">Go somewhere</a>
				  </div>
				</div>

				<div class="card col-12 col-md-6 col-lg-4 p-1">
					<img src="card2-300.jpg" class="card-img-top rounded-3" alt="...">
					<div class="card-body">
						<h5 class="card-title">Card title</h5>
						<p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
						<a href="#" class="btn btn-primary">Go somewhere</a>
					</div>
				</div>

				<div class="card col-12 col-md-6 col-lg-4 p-1">
					<img src="card2-300.jpg" class="card-img-top rounded-3" alt="...">
					<div class="card-body">
						<h5 class="card-title">Card title</h5>
						<p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
						<a href="#" class="btn btn-primary">Go somewhere</a>
					</div>
				</div>
			</div>
		</div>
	</section>
```