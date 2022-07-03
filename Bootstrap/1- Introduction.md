# Introduction

#### L'importance du mobile

Les navigateurs peuvent prendre en charge des standards du web, tels que HTML et CSS, de manière différente. Cette prise en charge complexe peut même parfois différer entre deux versions d’un même navigateur. Cela implique que vous devez prendre en compte ces variations lors de la création des pages web, pour vous assurer qu'elles s'affichent et fonctionnent correctement.

En tant que développeur front-end, vous devez garder ces différences de périphérique et de navigateur à l'esprit lorsque vous créez un site web. Heureusement, de nombreux **frameworks CSS** front-end ont été développés afin que vous puissiez passer plus de temps sur l'implémentation et les fonctionnalités de vos sites, et moins de temps sur le débugging et la refactorisation pour prendre en compte toutes ces variations.

Bootstrap est le framework CSS le plus connu, mais il en existe plein d’autres qui ont tous une approche de conception ou un design différents.

Voici d’autres exemples de framework CSS connus : [Materialize CSS](https://materializecss.com/), [Foundation](https://get.foundation/), [Bulma](https://bulma.io/), et [Tailwind CSS](https://tailwindcss.com/).


#### Open source !

Bootstrap est un framework CSS qui permet de **prototyper** vos idées et de créer un site web entier à l'aide de HTML, CSS et JavaScript.

Depuis sa première publication par Twitter en 2011, Bootstrap est un choix populaire parmi les développeurs web. Selon [builtwith.com](https://trends.builtwith.com/docinfo), il est utilisé sur plus de 21 millions de sites. De nombreux développeurs pensent qu'il constitue un choix évident pour leurs projets.

Tout ce dont vous avez besoin pour débuter avec Bootstrap 5 est un lien vers le **fichier CSS minifié**, c’est-à-dire un fichier le plus léger possible, du framework dans votre document HTML, et de connaissances de base en HTML, CSS et JavaScript. Il existe [plusieurs manières](https://getbootstrap.com/docs/5.1/getting-started/introduction/) d'inclure Bootstrap dans votre projet, mais la plus rapide et la plus simple est d’utiliser un lien vers le fichier CSS minifié hébergé sur [BootstrapCDN](https://www.bootstrapcdn.com/).

	CDN signifie **_content delivery network_** **(réseau de distribution de contenu)​​**. Il s'agit d'un système de serveurs distribués géographiquement. Ils fournissent le contenu web à un utilisateur en fonction de différents facteurs qui garantissent un débit plus élevé et une meilleure disponibilité.

Pour utiliser Bootstrap de cette façon, vous devrez ajouter cette ligne à la section   `<head>`  de votre fichier HTML :

```html
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-EVSTQN3/azprG1Anm3QDgpJLIm9Nao0Yz1ztcQTwFspd3yD65VohhpuuCOmLASjC" crossorigin="anonymous">
```

Il faut l'ajouter avant les autres fichiers CSS, afin que vos styles remplacent ceux de Bootstrap par défaut.

Certains composants de Bootstrap utilisent **JavaScript (JS)**, en particulier la **bibliothèque** **Popper.js**, ainsi que la bibliothèque JavaScript de Bootstrap. Pour vous assurer que tout fonctionne comme prévu, vous allez utiliser la version **bundle** pour importer la bibliothèque. Pour ce faire, il suffit d’ajouter cette ligne de code au bas de votre page juste avant la fermeture de la balise  `</body>`  :

```html
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-MrcW6ZMFYlzcLA8Nl+NtUVF0sA7MsXsP1UyJoMp4YLEuNSfAP+JcXn/tWtIaxVXM" crossorigin="anonymous"></script>
```

####  Communauté nombreuse et active

En tant que projet en **open source** populaire, Bootstrap comprend une communauté en ligne active et utile, avec de nombreuses discussions disponibles pour vous aider à trouver des solutions à vos problèmes, ou pour vous donner des conseils sur la manière de mieux utiliser le framework. Par exemple, [Stack Overflow](https://stackoverflow.com/) _(célèbre site communautaire d’entraide entre développeurs)_ comptabilise plus de 100 000 questions liées à Bootstrap en utilisant les mots clés “twitter-bootstrap” ou “bootstrap-5."

#### Personnalisable

De nombreux thèmes personnalisés sont utilisables pour vous aider à rendre votre site unique. En plus des [thèmes disponibles sur le site Bootstrap](https://themes.getbootstrap.com/), vous pouvez rapidement rechercher les thèmes proposés par d'autres fournisseurs. 

Étant donné qu'il est en open source et personnalisable, vous pouvez créer entièrement un thème, ou apporter des modifications aux autres.

#### Similarité

Le fait que Bootstrap soit simple d'utilisation peut être un désavantage si vous utilisez le thème et les couleurs par défaut. Vous risqueriez de trouver le thème que vous avez choisi sur d'autres sites.

Comme avec tout autre framework front-end, vous devrez le personnaliser en ajoutant des composants ou des styles, si vous souhaitez intégrer à votre site des conceptions uniques.