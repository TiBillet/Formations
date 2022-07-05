Commençons par définir les champs dont nous avons besoin :

-   un nom ;
    
-   un prénom ;
    
-   un e-mail ;
    
-   un message ;
    
-   un bouton “Envoyer”.
    

Comme à notre habitude maintenant, commençons par nous rendre sur la [documentation de Bootstrap 5,](https://getbootstrap.com/docs/5.0/forms/overview/) dans la rubrique “Forms”.

En cliquant sur “Overview”, nous pouvons voir la structure d’un formulaire classique.

```html
<form>
    <div class="mb-3">
        <label for="exampleInputEmail1" class="form-label">Email address</label>
        <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp">
        <div id="emailHelp" class="form-text">We'll never share your email with anyone else.</div>
    </div>
    <div class="mb-3">
        <label for="exampleInputPassword1" class="form-label">Password</label>
        <input type="password" class="form-control" id="exampleInputPassword1">
    </div>
    <div class="mb-3 form-check">
        <input type="checkbox" class="form-check-input" id="exampleCheck1">
        <label class="form-check-label" for="exampleCheck1">Check me out</label>
    </div>
    <button type="submit" class="btn btn-primary">Submit</button>
</form>
```

Nous observons deux éléments récurrents dans cet exemple : les classes  `.form-control`  et  `.form-label`. Ce sont les deux classes qui permettront à nos  `input`  d’être mis en page et d'accéder aux affichages alternatifs s’ils sont  `disabled`  ou en  `readonly`.

![[inputs.png]](./img/inputs.png)


# example :

```html

<section id="contact" class="py-5 bg-light">
	<div class="container">
		<h2 class="mb-0">Un projet de création web ?</h2>
		<h3 class="fw-light fs-5">Allons en discuter autour d'un café</h3>

		<div class="row gy-4 mt-4">
			<div class="col-12 col-md-5">
				<img src="../img/grab-a-coffee.jpg" alt="Image d'une tasse de café" width="100%">
			</div>
			<div class="col-12 offset-md-1 col-md-6">

				<!-- Formulaire -->
				<form class="row">
					<div class="col-6 my-2">
						<label for="firstname" class="form-label">Prénom</label>
						<input name="firstname" type="text" class="form-control" id="firstname">
					</div>
					<div class="col-6 my-2">
						<label for="name" class="form-label">Nom</label>
						<input name="name" type="text" class="form-control" id="name">
					</div>
					<div class="col-12 my-2">
						<label for="email" class="form-label">Email address</label>
						<input name="email" type="email" class="form-control" id="email">
					</div>
					<div class="col-12 my-2">
						<label for="message" class="form-label">Message</label>
						<textarea name="message" class="form-control" id="message" rows="3"></textarea>
					</div>
					<div class="col-12 my-2">
						<button type="submit" class="btn btn-primary w-100">Envoyer</button>
					</div>
				</form>

			</div>
		</div>
	</div>
</section>
```