# Choisir où ouvrir un café à Avignon

Un petit projet d'analyse spatiale. Je cherche le meilleur emplacement pour ouvrir un café à Avignon, à partir des lieux qui existent déjà dans la ville, avec deux méthodes de machine learning spatial, DBSCAN et KMeans.

Je fais ce genre de projet parce que j'aime mon métier de géomaticienne et que j'aime transformer une ville en données, puis des données en décision claire.

## Le problème

Un café ne marche pas n'importe où. Il lui faut du passage, de la vie, un quartier qui va avec. On répond souvent à ça à l'intuition. Ici je réponds avec la donnée.

## La méthode, en trois temps

D'abord la donnée. J'extrais tous les points d'intérêt d'Avignon depuis OpenStreetMap, des données ouvertes, et je les range en six familles, restauration, commerce, services, santé, éducation, vie nocturne. Plus de deux mille lieux.

Ensuite les centres. Je fais ressortir les vrais pôles d'activité de la ville avec un clustering spatial, la méthode DBSCAN. Elle regroupe les lieux proches les uns des autres et révèle les centres réels. Quatorze pôles ressortent à Avignon, chacun avec sa spécialité.

Enfin les quartiers. Je découpe la ville en une grille fine et je dresse une typologie avec la méthode KMeans. Elle range chaque case dans une famille de quartier. Huit profils ressortent.

Pour finir, je croise ces trois lectures dans un entonnoir, le bon type de case, dans un vrai pôle, du bon caractère. De près de quatre cents cases, je descends à une cinquantaine d'emplacements solides.

## Le résultat

Une carte des meilleurs emplacements pour un café à Avignon, classés et justifiés. Le premier tombe en plein cœur de ville. Pas une intuition, une liste appuyée sur la donnée.

## Lecture humaine et environnementale

Sur le plan humain, la méthode place l'activité là où les gens vivent et circulent déjà, au plus près des services du quotidien.

Sur le plan environnemental, elle favorise les centres denses et marchables, donc des trajets courts à pied et moins de dépendance à la voiture. C'est l'esprit de la ville du quart d'heure.

Et surtout, la méthode est reproductible. On garde le moteur, on change la cible, et elle sert aussi bien à placer un commerce qu'à choisir où implanter des bornes de recharge.


## Les données

Points d'intérêt et réseau issus d'OpenStreetMap, via OSMnx. Données ouvertes, sous licence ODbL. Le dossier `data` n'est pas versionné, il se remplit tout seul au premier lancement.


## Moi

Victorine Maximilienne Djetcheu Toko, géomaticienne.

Portfolio, https://portfolio-victorine-djetcheu.netlify.app
LinkedIn, https://www.linkedin.com/in/victorine-maximilienne-djetcheu-toko
GitHub, https://github.com/VictorinM
