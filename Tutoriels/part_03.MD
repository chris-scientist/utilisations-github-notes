
# Les branches - Partagez votre code source sur GitHub

v0.0.2

## Introduction

Avant de vous présenter ce qu'est une branche faisons un petit point ! Ce tutoriel suppose que vous avez les connaissance de bases sur Git, dans le cas contraire reportez vous à la [partie 1](part_01.MD). Je présente ici une notion avancée de la gestion des sources.

Qu'est-ce qu'une branche ? En réalité, lors de la partie 1 vous avez travaillé sur une branche, qui se nomme "master". Vous pouvez par exemple avoir les branches suivante :
* master : pour le code de la dernière version stable ;
* dev : pour le code relatif à vos améliorations ;
* v1.0 : pour appliquer des modifications à la version 1.0 de votre projet.

J'espère qu'avec cette exemple vous avez compris l'intérêt des branches.

## Pratique

### Créer une branche et l'utiliser

Pour créer la branche nommée "dev", la commande est `git branch dev`.

Pour travailler sur cette branche "dev" (faire des commits), la commande est `git checkout dev`.

### Envoyer une branche sur GitHub

Après avoir committer votre travail sur la branche "dev", pour envoyer celle-ci sur GitHub utiliser la commande `git push --set-upstream origin dev`.

### Fusionner deux branche

Nous allons rappatrier la branche "dev" sur "master".

Pour ce faire, il faut sélectionner la branche "master", avec la commande que vous connaissez déjà `git checkout master`.

Pour fusionner les branches "master" et "dev", voici la commande `git merge dev`.

Penser à pousser votre code sur GitHub via `git push`.

### Supprimer la branche

Lorsque vous avez fini de travailler avec votre branche, vous pouvez la supprier avec la commande `git branch -d dev`.

Si vous utilisez une version de git supérieur ou égale à 1.7.0, pour pousser la suppression vers le dépôt distant utilisez la commande `git push origin --delete dev`.

## Conclusion

Je vous ai fait une brève présentation des branches, en cas de conflits je vous conseil la [lecture suivante](https://git-scm.com/book/fr/v1/Les-branches-avec-Git).
