
# Rebase

v0.0.1

## Introduction

Dans cette partie nous parlerons d'un unique rebase, pour être plus précis : admettons que vous ayez une branche de développment, nommons la simplement `dev`. Et deux branches de features, nommons les `feature-auth` et `feature-dashboard`, ces deux branches sont basés sur `dev` (sur laquelle nous pouvons admettre qu'il y a déjà du code / commits).

Vos branches `feature-auth` et `feature-dashboard` peuvent avancer en parallèle.

Admettons, que les développements de la branche `feature-auth` soit achevés. Vous mergé donc cette dernière avec `dev`.

Le développeur sur la branche `feature-dashboard` ne voit pas la nouvelle fonctionnalités qui ont été ajouté sur `dev`.

C'est là que le rebase entre en jeu !

### Processus

#### Assurez-vous que la branche d'origine soit à jour

```
git checkout dev
git pull
```

#### Repasser sur la branche à mettre à jour

`git checkout feature-dashboard`

#### Faire le rebase

`git rebase dev`

#### Valider le rebase

Si vous n'avez pas de conflits, tant mieux pour vous, dans le cas contraire soyez prudent avant de saisir la commande suivante et bon courage pour la résolution des conflits.

Lorsque vous êtes prêts validez le processus avec la commande suivante :

`git push -f`
