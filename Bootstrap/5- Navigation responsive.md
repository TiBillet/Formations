# Nav
Bootstrap donne une structure a respecter pour faire un menu tout seul comme un grand, automatique, responsive et très très classique.


```html
<nav class="navbar navbar-expand">

</nav>
```

On peut rajouter une marque.
Bootstrap propose une classe   `.navbar-brand`  prévue à cet effet dans le composant de la barre de navigation. Ajoutez le nom du site dans l'élément prévu à cet effet, comme ci-dessous :

```html
<nav class="navbar navbar-expand">
    <a class="navbar-brand" href="#">Prénom Nom</a>
	
</nav>
```

Dans notre cas, nous allons ajouter les classes  `.text-uppercase .fw-bold`  (texte en majuscules + texte en gras) à notre  `a.navbar-brand`. Ensuite, nous allons entourer notre prénom d’une balise  `span`  afin de lui donner d'autres propriétés de mise en page. Pour ce faire, nous ajoutons ces classes à notre élément  `span`,  `.bg-primary .bg-gradient .p-1 .rounded-3 .text-light`  :

```html
<a class="navbar-brand text-uppercase fw-bold" href="/index.html">
    <span class="bg-primary bg-gradient p-1 rounded-3 text-light">John</span> Doe
</a>
```

Passons maintenant aux liens de navigation. Les éléments de navigation doivent être placés dans une liste non ordonnée contenant les éléments  `<ul>`,   `<li>`  et   `<a>`, selon les classes indiquées dans cet extrait :

```html
<nav class="navbar navbar-expand">
    <div class="container">
        <a class="navbar-brand text-uppercase fw-bold" href="/index.html">
            <span class="bg-primary bg-gradient p-1 rounded-3 text-light">John</span> Doe
        </a>
        <ul class="navbar-nav">
            <li class="nav-item active">
                <a class="nav-link" href="#johndoe">Qui suis-je ?</a>
            </li>
            <li class="nav-item">
                <a class="nav-link" href="#expertise">Expertises</a>
            </li>
            <li class="nav-item">
                <a class="nav-link" href="#portfolio">Portfolio</a>
            </li>
            <li class="nav-item">
                <a class="nav-link" href="#contact">Contact</a>
            </li>
        </ul>
  </div>
</nav>
```

Vous remarquerez que le premier élément   `<li>`  dans l'extrait de code comprend une classe   `.active`. Cela permet d'indiquer l'un des éléments de navigation comme l'élément “actif”, actuellement sélectionné. Vous pouvez créer le code HTML de votre barre de navigation afin de vous assurer qu’un seul élément utilise cette classe.

Il y a un autre élément que vous devez bien connaître maintenant, il s’agit du  `div.container`. L’effet est exactement le même que partout ailleurs dans la page, il sert à contenir les éléments de la  `navbar`.

Désormais, votre barre de navigation est personnalisée avec le nom du site et les liens de navigation. Ensuite, ajoutons de la couleur !

Les classes   `.navbar-light`  et   `.navbar-dark`  constituent un autre ensemble pratique dans la gestion des couleurs Bootstrap. Ces classes ajustent la couleur des éléments de la barre de navigation, comme la marque et les liens de navigation, pour offrir un contraste à l'arrière-plan choisi. Lorsque vous utilisez une barre de navigation de couleur foncée, il vous suffit d’ajouter la classe   `.navbar-dark`. À l’inverse, comme dans le cas de notre site, ajoutez la classe   `.navbar-light`  à une barre de navigation de couleur claire.


```html
<nav class="navbar navbar-expand bg-light navbar-light">

</nav>
```

## Navbar Responsive

On va faire en sorte que navbar-expand ne s'applique qu'a partir de md. 

En dessous, on va ajouter un bouton collapse.

Première étape, rajouter md 

```html
<nav class="navbar navbar-expand-md bg-light navbar-light">
	
</nav>
```

Ensuite, rajouter un bouton collapse

```html
<button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
</button>

```

Comme vous pouvez le constater, le bouton comprend une classe   `.navbar-toggler`, ainsi que des attributs data tels que   `data-bs-toggle="collapse"`  et   `data-bs-target="#navbarNav"`. Ces attributs permettent de cibler le bon élément   `<div>`  utilisant la classe   `.collapse`  et l’identifiant  `#navbarNav`, sans écrire une seule ligne de JavaScript.

Pour ce faire, ajoutez les classes   `.collapse`  et   `.navbar-collapse`  à la `<div>`  qui enveloppe la liste des liens de navigation.

Enfin, ajoutez l’attribut identifiant ayant la même valeur que celle de l'attribut  `data-bs-target`  du bouton Bascule, dans ce cas   `navbarNav`  :

```html
<div class="collapse navbar-collapse justify-content-end" id="navbarNav">
    <ul class="navbar-nav">
        <li class="nav-item">
            <a class="nav-link" href="#johndoe">Qui suis-je ?</a>
        </li>
        <li class="nav-item">
            <a class="nav-link" href="#expertise">Expertises</a>
        </li>
        <li class="nav-item">
            <a class="nav-link" href="#portfolio">Portfolio</a>
        </li>
        <li class="nav-item">
            <a class="nav-link" href="#contact">Contact</a>
        </li>
    </ul>
</div>
```

Vous remarquerez peut-être la classe  `justify-content-end`  : encore une fois, c’est une [classe utilitaire de Bootstrap 5](https://getbootstrap.com/docs/5.0/utilities/flex/) permettant d’ajouter la propriété  `flex justify-content: flex-end`.

En effet, la navigation Boostrap 5 est par défaut en display  `flex`, ce qui fait que nous pouvons utiliser les propriétés  `flex`  sur les éléments enfants de la  `nav`  pour les placer à droite, à gauche, au centre...


# On essayer d'arriver à ça ? 

```html
<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-EVSTQN3/azprG1Anm3QDgpJLIm9Nao0Yz1ztcQTwFspd3yD65VohhpuuCOmLASjC" crossorigin="anonymous">
	<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.5.0/font/bootstrap-icons.css">
	<title>Bootstrap Courses</title>
</head>
<body>
	<header>
		<nav class="navbar navbar-expand-md bg-dark navbar-dark">
			<div class="container">
				<a class="navbar-brand text-uppercase fw-bold" href="#">
					<span class="bg-primary bg-gradient p-1 rounded-3 text-light">John</span> Doe
				</a>

				<button class="navbar-toggler" type="button" 

				aria-controls="navbarNav" 
				aria-expanded="false" 
				aria-label="Toggle navigation"

				data-bs-toggle="collapse" 
				data-bs-target="#navbarNav" 
				>

					<span class="navbar-toggler-icon"></span>
				</button>

				<div class="collapse navbar-collapse justify-content-end" id="navbarNav">

				<ul class="navbar-nav">
					<li class="nav-item">
						<a class="nav-link" href="#johndoe">Qui suis-je ?</a>
					</li>
					<li class="nav-item">
						<a class="nav-link" href="#expertise">Expertises</a>
					</li>
					<li class="nav-item">
						<a class="nav-link" href="#portfolio">Portfolio</a>
					</li>
					<li class="nav-item">
						<a class="nav-link" href="#contact">Contact</a>
					</li>
				</ul>
				</div>

			</div>
		</nav>
	</header>

	<section class="">
		<div class="container text-center text-sm-start fs-2">
			<div class="row my-1 ">
				<div class="bg-danger bg-gradient col-sm-6 offset-lg-3 col-lg-6 my-sm-0 my-1 ">
					1ère Ligne - Première colonne
				</div>
				<div class="bg-success bg-gradient col-sm-6 col-lg-3">
					1ère Ligne - Deuxième colonne
				</div>
			</div>

			<div class="row my-1">
				<div class="bg-success bg-gradient col-sm-6 col-lg-3 my-sm-0 my-1">
					2eme Ligne - Première colonne
				</div>
				<div class="bg-success bg-gradient col-sm-6 offset-lg-6 col-lg-3">
					2eme Ligne - Deuxième colonne
				</div>
			</div>

			<div class="row my-1 ">
				<div class="col-sm-3 bg-primary bg-gradient offset-lg-6 my-sm-0 my-1">
					3eme Ligne - Première colonne
				</div>
				<div class="col-sm-3 offset-sm-6 offset-lg-0 bg-primary bg-gradient">
					3eme Ligne - Deuxième colonne
				</div>
			</div>

		</div>
	</section>
	<section>
		<div class="container">
			
			<button type="button" class="btn btn-primary" action="submit">Bouton</button>
			<a class="btn btn-primary" href="/index.html" role="button">Lien</a>


			<a href=”mon lien linkedin” target=”_blank”>
				<i class="bi bi-envelope-open"></i>
			</a>

		</div>
	</section>

</body>
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-MrcW6ZMFYlzcLA8Nl+NtUVF0sA7MsXsP1UyJoMp4YLEuNSfAP+JcXn/tWtIaxVXM" crossorigin="anonymous"></script>
</html>

```