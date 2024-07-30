# Bienvenue à la documentation Tachéo


L’application est divisé en deux parties différentes : Le module de calcul écrit en Python hébergé sur le serveur et le module de visualisation écrit en R

Le module de calcul traite les données sous format brut (coordonnées ECEF) pour le convertir en coordonnées géographique et projetées qui sont intégrés dans une base de données Postgresql

Le module de visualisation récupère ces données pour afficher des cartes et des graphiques via un serveur web, ce module permet également de télécharger les données brutes et traitées d’un site au format CSV.

## Structure du projet

    | 
    |-- app.R
    |-- DESCRIPTION
    |-- inst
    |     `-- app
    |          `-- www
    |               |-- img
    |               |    `-- # Images utilisés dans l'application
    |               |-- favicon.ico
    |               |-- main.css
    |               `-- tiles_config.json # Map tiles configuration file
    |-- R
    |   `-- # R scripts
    |-- tests
    |   `-- # Test unitaires automatisés
    |-- vignettes
    |   `-- # fusen files
    |-- dev
        `-- # Golem files


Pour ce qui concerne l’application, le contact est **Xavier WANNER** `x.wanner@quadrilaterre.fr` qui en est l’auteur