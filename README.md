Analyse du marché automobile américain (USA Car Sales)

Description du projet

Ce projet de Data Analysis a été réalisé dans le cadre d'un exercice consistant à analyser un jeu de données contenant plus de 558 000 transactions de ventes de véhicules aux États-Unis.

L'objectif est de se mettre dans la peau d'un directeur commercial d'un revendeur automobile souhaitant mieux comprendre le marché automobile américain à partir des données disponibles.

Les principales missions du projet sont :

Nettoyer et préparer les données.
Identifier les problèmes de qualité des données.
Traiter les valeurs manquantes et les incohérences.
Réaliser des analyses descriptives quantitatives et qualitatives.
Répondre à des questions métiers pertinentes à l'aide de statistiques et de visualisations.
Dataset

Le jeu de données contient notamment les variables suivantes :

Variable	Description
year	Année du véhicule
make	Marque du véhicule
model	Modèle du véhicule
trim	Version du modèle
body	Type de carrosserie
transmission	Type de transmission
vin	Numéro de châssis (identifiant unique)
state	État américain de la vente
condition	État du véhicule
odometer	Kilométrage du véhicule
color	Couleur extérieure
interior	Couleur intérieure
seller	Vendeur
mmr	Valeur estimée du marché
sellingprice	Prix de vente final
saledate	Date de vente
Technologies utilisées
Python
Pandas
Matplotlib
Jupyter Notebook / Google Colab

Étapes réalisées

1. Exploration des données
Analyse des types de variables.
Analyse des dimensions du dataset.
Analyse des valeurs manquantes.
Analyse des modalités des variables qualitatives.
Analyse descriptive des variables quantitatives.

2. Nettoyage des données
Variables quantitatives

Les variables suivantes ont été étudiées :

condition
odometer
mmr
sellingprice

Les traitements réalisés incluent :

Analyse des valeurs manquantes.
Analyse des valeurs extrêmes (outliers).
Utilisation des statistiques descriptives.
Remplacement des valeurs manquantes lorsque cela était pertinent.

Un travail particulier a été réalisé sur la variable odometer afin d'identifier certaines valeurs exceptionnellement élevées et de décider si elles étaient plausibles ou non.

Variables qualitatives

Les variables suivantes ont été étudiées individuellement :

make
model
body
transmission
color
interior
state
seller
trim
vin

Les traitements effectués comprennent :

Analyse des modalités.
Analyse des fréquences avec value_counts().
Recherche des valeurs manquantes.
Utilisation du mode des variables.
Uniformisation des catégories lorsque cela était nécessaire.
Création de la catégorie "Unknown" lorsque les valeurs manquantes ne pouvaient pas être imputées de manière fiable.

Exemples :

Transformation de la modalité "—" en valeur manquante pour certaines variables.
Regroupement des catégories écrites différemment (SUV et suv, Sedan et sedan).
Conservation des observations lorsque l'information n'était pas connue plutôt que d'introduire un biais statistique.

3. Analyse des données

Les analyses portent notamment sur :

Les marques les plus vendues.
Les modèles les plus populaires.
La répartition des types de carrosserie.
Les prix de vente des véhicules.
Le kilométrage des véhicules.
La valeur de marché (MMR).
La relation entre le kilométrage et le prix.
Les véhicules les plus chers.
Les États réalisant le plus grand nombre de ventes.
Les caractéristiques générales du marché automobile américain.
4. Visualisations

Les graphiques ont été réalisés uniquement avec :

Pandas
Matplotlib

Parmi les visualisations utilisées :

Histogrammes
Diagrammes en barres
Boxplots
Graphiques de distribution
Graphiques comparatifs
Traitement de la variable saledate

La variable saledate a été convertie au format datetime.

Après conversion, une partie importante des observations n'a pas pu être interprétée correctement et a été transformée en valeurs manquantes (NaT).

Cette variable n'a pas été utilisée dans les analyses principales du projet, car :

elle n'est pas indispensable pour répondre aux objectifs métiers ;
la période couverte est relativement courte ;
les analyses principales concernent les caractéristiques des véhicules et les prix de vente.
Structure du projet
.
├── data/
│   └── car_prices.csv
│
├── notebooks/
│   └── Analyse_Marche_Automobile_USA.ipynb
│
├── images/
│   └── graphiques
│
├── README.md
│
└── requirements.txt


Objectifs pédagogiques

Ce projet m'a permis de travailler sur :

le nettoyage des données ;
la gestion des valeurs manquantes ;
l'analyse exploratoire des données (EDA) ;
les statistiques descriptives ;
la visualisation des données avec Pandas et Matplotlib ;
la prise de décision en Data Analysis ;
la documentation d'un projet GitHub.
Conclusion

L'analyse met en évidence plusieurs caractéristiques intéressantes du marché automobile américain, notamment la popularité de certaines marques et modèles, l'importance du kilométrage dans la valorisation des véhicules ainsi que la diversité des carrosseries et des prix observés.

Une attention particulière a été portée au nettoyage des données afin de limiter les biais statistiques et de conserver un maximum d'informations pertinentes pour l'analyse.

Ce projet illustre une démarche complète de Data Analysis allant de l'exploration des données jusqu'à l'interprétation des résultats.

