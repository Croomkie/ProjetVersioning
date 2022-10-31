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
