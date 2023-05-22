# COURS GIT

## 1, Introduction

Git et GitHUB permettent de créer des version d'un projet, cela permet de revenir à une version antérieure du projet si besoin. L'avantage de de GitHUB est qu'il permet de travailler à plusieurs sur un même projet, de créer des branches pour travailler su run efonctionnalité sans impacter le projet principal.

### GIT
GIT  est un 'VCS' (Version Control System) qui permet de créer des versions d'un projet. Avec GIT, les versions de notre projet sont stockées caché nommé '.git'. Ce dossier contient l'historique des modifications apportées au projet.

### GITHUB
GITHUB est un service en ligne qui permet d'héberger des projets GIT. Donc, grâce à GITHUB, on peu théberger nos projets en ligne, afin de pouvoir y accéder depuis n'importe quel ordinateur.

## 2, les commandes de base
### Dépot local
Pour initialiser git sur un projet, il faut avoir le projet dans le terminal en faisant : 'cd chemin/vers/le/projet' => qui va pointer dans le dossier du projet.

Ensuite, il faut faire 'git init' pour initialiser git sur le projet.
Par défaut git ne vas pas prendre en compte tous les fichiers du projet.
Pour ajouter un fichier au suivi de git, il faut faire 'git add nomDuFichier'.
Pour ajouter tous les fichiers du projet, il faut faire 'git add .' ou 'git add -A'.
Pour vérifier l'état du projet, vous faite 'git status' qui va afficher les fichiers qui sont dans le suivi de git et ceux qui ne le sont pas.

## TODO 1 : 
Créer un fichier 'about.html' et faites en sorte que ce fichier et le fichier 'contact.html' soit pris en compte par git.

Pour ne pas tracker un fichier, il faut créer un fichier '.gitignore' et y mettre le nom du fichier à l'ignorer. Si le fichier se trouve dans un sous-dossier, il faut mettre le chemin vers le fichier à ignorer.

### Mon premier commit
Avant de faire un commit (Une version), il faut configurer git. Pour cela, il faut faire 'git config --global user.name "votre nom" et
                                                                                         'git config --global user.email "Votre email"
Pour créer un commit, il faut faire
'git commit -m "Message du commit", soyez le plus précis possible dans le message du commit afin de pouvoir retrouver le commi que vous cherchez.

Pour voir l'historique des commits, il faut faire 'Git log'.
Pour modifier le messgae du dernier commit, il faut faire : 'git commit --amend'. Cela va ouvrir l'éditeur 'vim' et pour ajouter les modifications, il faut appuyer sur la touche 'i' pour passer en mode insertion, faire les modifications puis appuyer sur la touche 'echape' et taper ':wq!' pour enregistrer et quitter.

VIM
':' => permet d'entrer une commande
'q' => permet de quitter sans enregistrer
'q!' => permet de forcer la fermeture sans enregistrer
'w' => permet d'enregistrer


git config --global --unset-all
git config --unset-all credential.helper

git config --global --unset-all user.name
git config --global --unset-all user.email

git config --list