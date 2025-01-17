# ProjetVersioning

Groupe de 4

## Bonne pratique

Nous avons créer une clé SSH chacun de notre côté et nous avons cloner le projet en SSH.

## Syntaxe

Pour chaque nouvelle branche pour son nom ‘type de branche/date/nom de la branche’
exemple : git branch ‘feature/27102022/ajout d’une navbar’

## Fonctionnement git flow :

Pour chaque nouvelles fonctionnalités créé une branche avec le nom de la feature,
une fois la feature terminé on la déplace sur la branche develop comme ça tous
le monde pourras tester la nouvelle feature,
ensuite on créé une release, une fois quelle sera validé on la push sur la branche principale

## Choix du workflow

Nous avons choisi le workflow git flow pour réaliser notre projet, mais nous avons hésité à utiliser le workflow basé sur le tronc qui aujourd’hui est considéré comme une meilleure pratique.

## Modèle de notre projet

Comme nous avons choisi le workflow git flow nous commençons par créer une branche “develop” sur laquelle on ajoutera des branches “feature” qui seront nos nouveauté en cours de développement. Puis nous créerons une branche “release” dans le “develop” qui aura pour vocation de tester que le code fonctionne correctement avant de l’ajouter au “main”.

## Mise en place de l’espace de travail :

```
git branch develop // Création de la branche
git push origin develop // Envoie de la branch en ligne

```

## Création des issues

Avant de développer, on créé une tâche sur github dans l'onglet issues on l'insère dans la milestone correspondantes (ensemble de tâches qui sont sur le même thème)
Ensuite, ranger la tâche en fonction de si elle est à faire (To do), si elle est en cours (In progress) et si elle est terminé (Done)

## Push votre issues fini sur le repo github

Commencez par commit sur votre feature, en pensant bien à spécifier le # de votre issue, ensuite déplacer vous sur la branche main 
- checkout branch main, puis faites un pull pour récuperer ce qu'il y a actuellement sur le repo github
ensuite faites un merge entre la branche master et votre feature, gérer les conflits et enfin vous pouvez Push.

## Pour accéder au site en ligne

Lien netlify : https://projetversioning.netlify.app/

## Nouveau fonctionnement :

Avant, nous fonctionnions de manière à merge le travail réalisé sur nos features directement sur la main. 
Dorénavant, nous allons, nous déplacer sur la branche develop puis merge nos features a partir de celle-ci, avant de merge nous faisons un pull, puis nous faisons un merge en gérant les conflits. 
Puis on push directement à partir de celle-ci. Enfin, nous créons des pull request sur le repo pour merge le travail réalisé sur la develop avec la branche main.