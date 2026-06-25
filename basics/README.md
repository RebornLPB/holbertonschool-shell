# Shell - Basics

Ce projet marque l'introduction au système d'exploitation Unix et à la manipulation de la ligne de commande via le Shell (Bash). L'objectif est de comprendre l'environnement de l'interprète de commandes, de naviguer dans le système de fichiers et de maîtriser les manipulations de base des fichiers et répertoires.

## 📝 Concepts Clés

* **Navigation :** Déplacement fluide dans l'arborescence des fichiers Unix (chemins absolus vs. relatifs).
* **Gestion des Fichiers :** Création, suppression, copie, déplacement et renommage de fichiers et de répertoires.
* **Permissions & Visualisation :** Lecture du contenu des fichiers et compréhension des métadonnées de base via le terminal.

## 🛠️ Spécifications et Contraintes

* **Interprète de commandes :** Tous les scripts sont écrits pour `bash` et testés sur Ubuntu 20.04 LTS.
* **Format des Scripts :** * Tous les fichiers doivent se terminer par une nouvelle ligne.
  * La première ligne de chaque fichier doit contenir exactement le Shebang : `#!/bin/bash`.
  * Les scripts doivent être fonctionnels et ne pas contenir de texte superflu non exécutable.
* **Exécutabilité :** Tous les fichiers doivent être rendus exécutables via la commande `chmod u+x`.

## 📁 Liste des Fichiers & Tâches

| Fichier | Commande Principale | Description |
| :--- | :--- | :--- |
| `0-current_working_directory` | `pwd` | Affiche le chemin absolu du répertoire de travail actuel. |
| `1-listit` | `ls` | Affiche le contenu du répertoire courant. |
| `2-change_directory` | `cd` | Modifie le répertoire de travail pour aller dans le répertoire personnel de l'utilisateur (`~`). |
| `3-listfiles` | `ls -l` | Affiche le contenu du répertoire courant au format long (détails des permissions/tailles). |
| `4-listallfiles` | `ls -la` | Affiche tout le contenu du répertoire courant, y compris les fichiers cachés (commençant par `.`). |
| `5-listfilesdigitonly` | `ls -laN` ou variant | Affiche le contenu du répertoire courant avec les IDs d'utilisateur et de groupe au format numérique. |
| `6-firstdirectory` | `mkdir` | Crée un répertoire nommé `my_first_directory` dans le dossier `/tmp/`. |
| `7-movetmp` | `mv` | Déplace un fichier spécifique du répertoire courant vers le dossier `/tmp/`. |
| `8-firstdelete` | `rm` | Supprime un fichier spécifique situé dans le répertoire courant. |
| `9-firstdirdeletion` | `rmdir` ou `rm -r` | Supprime un répertoire spécifique situé dans le dossier `/tmp/`. |
| `10-back` | `cd -` | Change le répertoire de travail pour revenir au répertoire précédent. |
| `11-lists` | `ls` pluriel | Liste les fichiers du répertoire courant, du répertoire parent, et du répertoire `/boot` simultanément. |
| `12-file_type` | `file` | Affiche le type d'un fichier donné (ex: texte, exécutable, répertoire). |
| `13-symbolic_link` | `ln -s` | Crée un lien symbolique vers un fichier ciblé. |
| `14-copy_html` | `cp` | Copie tous les fichiers HTML du répertoire de travail actuel vers le répertoire parent, uniquement s'ils n'existent pas ou sont plus récents. |

## 🚀 Utilisation

Pour rendre un script exécutable et le lancer :

```bash
chmod u+x 0-current_working_directory
./0-current_working_directory