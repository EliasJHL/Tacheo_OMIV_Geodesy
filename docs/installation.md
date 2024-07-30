## Installation des packages R

Pour une application golem, il est important de s'assurer que tous les packages sont installés et dans la bonne version

###  1. Préparation des outils nécessaires

Tous les packages nécessaires se trouvent dans le fichier `DESCRIPTION`, pour correctement installer les bonnes version vous pouvez utiliser le package `devtools`. Vous pouvez l'installer via cette commande : 

```R
install.packages("devtools")
```

Si vous venez à ajouter des packages ou autres configurations il sera important que tout soit spécifié dans le fichier `DESCRIPTION` qui est généré par *golem*

### 2. Installation des packages

Pour installer les dépendances listés vous pouvez utiliser `devtools::install_deps()` il installera tous les packages à la bonne version.

```R
devtools::install_deps()
```

### 3. Vérification de l'intégrité de l'application

Vous pouvez utiliser `devtools::check()` pour vérifier que tout est correctement installé et configuré

```R
devtools::check()
```

### 4. Lancement de l'application

Pour lancer l'application en local, vous pouvez utiliser la commande *golem* :

```R
golem::run_dev()
```