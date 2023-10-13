# Création d'un dépôt GIT

## Création d'un dépôt GIT en local

Dans la console, initialisation du dépôt:

```bash
git init
```
## Visualisation de l'état de GIT

```bash
git status
```
###pour les fichiers et dossiers unix 

```bash
ls -a
```

## pour ajouter un fichier a la future sauvegarde 
```bash
git add readme.md
````
## pour effectuer la sauvegarde 

les fichier en attentes de sauvegarde sont en vert>

les fichier non suivi sont en rouge.

seul les fichiers en **staging** seront sauves

``` bash
git commit -m "message du commit"

un commit est une sauvegarde , on peux y acceder
avec un `git log`(affichage des identifiants des sauvegardes
et `git show` (sans parametre,affichage du dernier commit)

##pour ajouter tout les fichiers en staging

```bash
git add .
```
##ajouter d'un serveur 

nous allons utuliser un depot que l'on va cree sur github.com
apres connextion .comme c'est un travaille personelle, sur URL sera 
de ce type: hhtp//: github.com /votre username /le project 

nous creons un new repository, puis nous copions la clefs ssh 

git@github.com:sebastien2506git@github.com:sebastien2506/exe1html.git/exo1html.git

nous retournons dans notre console :

```bash
git@github.com:sebastien2506/exe1html.git

pour voir si ca fonctionne:

```bash 
git remote -v


## envoi du projet

```bash
git push origin main 
```
##recuperation du projet 

si on souhaite recupere que le `.git`(donc l'historique sans les fichiers

```bash
git fetch origin main

si on souhaite recupere toute la branche `main`

```bash 
git pull origin main 
```

Si on a effectué des modifications en local non voulues ne permettant pas 
la récupération des fichiers (`merge error`).

On peut utiliser un `git stash` pour faire une pseudo sauvegarde et revenir au dernier commit
avant de refaire un `git pull`

