# Cours GitHub

## Introduction

Git est un système de contrôle de version utilisé en programmation. Il permet aux développeurs de suivre et de gérer les changements dans leur code, pour faciliter la collaboration sur des projets complexes. Il va donc permettre de limiter les erreurs grâves et de pouvoir retourner en arrière. Il va aussi permettre de se partager des nouvelles versions plus facilement.

## Installation de git

Pour Linux : `sudo apt install git-all`

Pour Windows: Aller sur https://git-scm.com/download/win puis installer git 

Pour MacOS: Aller sur https://git-scm.com/download/mac puis suivre les instructions pour votre gestionnaire de paquets

## Commandes de bases

Les commandes de base de git peuvent être executé dans, plus ou moins cet ordre :

- `git init` : Démarre un nouveau dépôt Git dans le répertoire courant.

- `.gitignore` : Spécifie les fichiers à ignorer en les répertoriant dans ce fichier.

- `git status` : Affiche l'état actuel des fichiers dans l'espace de travail.

- ` git diff` : Compare les modifications entre l'espace de travail et la dernière version enregistrée.

- `git add` . : Ajoute les modifications en cours à la zone de préparation.

- `git commit -m "message du commit"` : Enregistre les modifications ajoutées dans un nouveau commit avec un message descriptif.

- `git log` : Présente l'historique des commits effectués dans le dépôt.

- `git show` [commit_hash] : Affiche les détails des modifications pour un commit spécifique.

- `git push` : Envoie les modifications locales vers le dépôt distant.

- `git pull` : Récupère les modifications du dépôt distant et les fusionne dans la branche locale.

- `git log --all --graph` : Affiche graphiquement l'historique de toutes les branches, y compris les fusions.

## Système de branches


Les branches sur GitHub sont comme des versions différentes de votre projet. Elles servent à travailler sur des modifications ou des nouvelles fonctionnalités sans toucher à la version de base. Vous créez donc une branche, y apportez des changements, puis une fois terminé, vous pouvez fusionner ces changements avec la version principale. Cela aide à garder le projet organisé et sûr.

- Créer et changer de branche : `git checkout -b <nomdebranche>`; `git checkout <nomdebranche>`

- Lister les branches : `git branch`

- Fusionner une branche : `git merge <nom_branche>`

- Supprimer une branche : `git branch -D <nombranche>`

- Stocker les changements : `git stash`

- Récupérer les changements `stockés : git stash pop`

- Annuler les changements : `git restore .`

- Nettoyer les fichiers qui ne sont pas suivi : `git clean -f`

- Modifier le dernier commit : `git commit --amend`

- Réinitialiser à un commit spécifique : `git reset <idcommit>`