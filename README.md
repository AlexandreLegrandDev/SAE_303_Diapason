Diapason - Visualisation et Analyse de data

![Uploading logo-diapason.png…]()

Diapason est un tableau de bord de visualisation de données permettant d’analyser les performances de différents solveurs de problèmes SAT.  
Le projet met l’accent sur la capacité de résolution (SAT / UNSAT / UNKNOWN) ainsi que sur les temps de calcul, à partir d’un fichier de résultats au format JSON.


Composition de l’équipe

LEGRAND Alexandre
BAL Matéo
MMI2C - Spé Dev Web

Description de la visualisation

La visualisation proposée s’organise sous la forme d’un dashboard interactif, construit avec Chart.js et une interface inspirée de Material Dashboard (le projet reprend l'arborescence d'un projet Material Dashboard).

Les principales visualisations sont :

- Échelles de données par famille de solveurs
  Une visualisation horizontale permet de représenter la répartition des solveurs selon leurs familles algorithmiques, offrant une vue d’ensemble de la diversité des approches.

- Répartition des résultats (SAT / UNSAT / UNKNOWN)  
  Un graphique circulaire permet d’avoir une vue globale de l’état des problèmes traités par les solveurs.

- Efficacité des solveurs  
  Un graphique en barres empilées montre, pour chaque solveur, le nombre de problèmes résolus (SAT et UNSAT), ce qui permet de comparer leur efficacité.

- Temps de résolution moyen  
  Un graphique en barres présente le temps moyen de calcul par solveur, afin d’évaluer leurs performances temporelles.

L’ensemble des graphiques est **responsive** et s’adapte à la taille de l’écran.

Problèmes rencontrés et solutions apportées

- Chargement du fichier JSON : le chargement initial des données ne fonctionnait pas à cause de chemins incorrects et de noms de champs non adaptés.  
  --> Solution : vérification de l’arborescence du projet et adaptation du code JavaScript aux champs du fichier JSON.

- Graphiques invisibles malgré des données valides : certains graphiques n’étaient pas affichés correctement dans Material Dashboard.  
  --> Solution : définition explicite de la hauteur des conteneurs et utilisation des options Chart.js `responsive: true` et `maintainAspectRatio: false`.

- Problèmes de mise en page responsive : les graphiques ne s’adaptaient pas correctement aux différentes tailles d’écran.  
  --> Solution : encapsulation des canvas dans des conteneurs dédiés et ajustements CSS.

- Petits problèmes de git au début du projet (changement de l'arborescence et fork)
  --> Création d'un fork et de nouvelles branches pour assurer d'avoir au moins une backup en cas de mauvaise manipulation / mauvais push (ce n'est pas arrivé). 

- Style peu adapté à notre application : création d'une identité graphique
  --> CSS complétement refait

Choix du nom « Diapason »

Le diapason est un instrument servant de référence pour accorder et mesurer une fréquence.  
Ce nom fait écho à l’objectif du projet : mesurer, comparer et accorder les performances de solveurs à partir de données objectives.
À l'origine, ce nom a été choisi de manière totalement aléatoire mais nous l'avons gardé pour son originalité et sa justification vis à vis du projet...


Technologies utilisées

- HTML / CSS / JavaScript
- Chart.js
- Material Dashboard (Surtout pour l'interface)
- IA Générative
- Photoshop (retouche du diapason)

Accès au projet

Accès à l'ensemble des fichiers sur le github --> possibilité de cloner le projet.
