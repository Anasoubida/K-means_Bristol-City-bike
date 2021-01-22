## K-means_Bristol-City-bike

![8e](https://user-images.githubusercontent.com/71134465/105554899-92dcd680-5d08-11eb-826b-dd68448c05d9.jpg)

# Objectif de l'étude 

L'objectif principal de ce projet est de regrouper l'emplacement des stations vélos à l'aide de l'algorithme de KMeans. 

# Description des fichiers

* Le dossier Data contient la base de données de Brisbane-City-Bike (Bristol-city-bike.json) ;
* Le dossier Exported comporte les résultats du clustering dans un tableau excel ;
* le fichier Properties.conf contient les raccourcis de nos fichiers utilisés ;
* Le code python ;
* Le Readme qui résume nos résultats ;

# Description de la base de données

La base de données (Bristol-city-bike.json) contient l’emplacement des vélos à Bristol. 

| address            | latitude | longitude| name	              | number |
|--------------------|----------|----------|--------------------|--------|
|Lower River Tce /...|-27.482279|153.028723|122 - LOWER RIVER...|	  122  |
|Main St / Darragh St| -27.47059|153.036046|91 - MAIN ST / DA...|    91  |
|Sydney St Ferry T...|-27.474531|153.042728|88 - SYDNEY ST FE...|    88  |

La base de données ci-dessus est composée de 5 variables : 

* Adresse (de l'emplacement du vélo)
* Latitude (de l'emplacement du vélo) 
* Longitude (de l'emplacement du vélo)  
* name : Le nombre + l'adresse du vélo
* number : numéro du vélo 

# Résultat du K-means
Pour regrouper nos données de façon géographique, nous avons décidé de garder uniquement les variables longitude et latitude comme variables d'entrées pour la réalisation du K-means. 
L'algorithme du k-means a permis d'avoir 3 cluster, premier groupe à l'est, le second groupe au centre et le troisième groupe à l'ouest 

|Cluster   |       moy_latitude|     moy_longitude|
|----------|-------------------|------------------|
|EST       |-27.460240636363633|153.04186302272726|
|CENTRE    | -27.47255990624999|   153.02594553125|
|Ouest     |-27.481218536585374|153.00572882926832|

Voici la map qui illustre nos résultats de clustering :
![MAP](https://user-images.githubusercontent.com/71135204/105554940-a5efa680-5d08-11eb-9b4b-5d3185051aee.PNG)
