# Shell - Permissions

Ce projet est dédié à la compréhension et à la manipulation des permissions d'accès aux fichiers et répertoires sous les systèmes d'exploitation Unix/Linux. L'objectif est de maîtriser le modèle de sécurité multi-utilisateurs, de comprendre les rôles (`owner`, `group`, `others`) et d'apprendre à modifier les droits et les propriétés des fichiers.

## 📝 Concepts Clés

* **Classes d'Utilisateurs :** Définition des droits pour le Propriétaire (`u`), le Groupe (`g`) et les Autres (`o`).
* **Types de Droits :** Lecture (`r` = 4), Écriture (`w` = 2) et Exécution (`x` = 1).
* **Notations des Permissions :** Manipulation via la notation symbolique (ex: `u+x,g-w`) et la notation octale/numérique (ex: `755`, `644`).
* **Commandes de Gestion :** Utilisation de `chmod` (changement de mode), `chown` (changement de propriétaire) et `chgrp` (changement de groupe).

## 🛠️ Spécifications et Contraintes

* **Interprète :** Scripts écrits exclusivement pour `bash` (testés sur Ubuntu 20.04 LTS).
* **Format :** Shebang `#!/bin/bash` requis sur la première ligne, fin de fichier par une nouvelle ligne.
* **Exécutabilité :** Tous les scripts doivent être rendus exécutables (`chmod u+x`).

## 📁 Liste des Fichiers & Tâches

| Fichier | Commande / Action | Description |
| :--- | :--- | :--- |
| `0-iam_betty` | `su` | Script qui bascule l'utilisateur actuel vers l'utilisateur `betty`. |
| `1-who_am_i` | `whoami` | Affiche l'identifiant de l'utilisateur effectif actuel. |
| `2-groups` | `groups` | Affiche tous les groupes auxquels appartient l'utilisateur actuel. |
| `3-new_owner` | `chown` | Modifie le propriétaire d'un fichier spécifique pour le remplacer par `betty`. |
| `4-empty` | `touch` | Crée un fichier vide nommé `hello`. |
| `5-execute` | `chmod` | Ajoute la permission d'exécution au propriétaire du fichier `hello`. |
| `6-multiple_permissions` | `chmod` | Ajoute l'exécution pour le propriétaire et le groupe, et la lecture pour les autres sur `hello`. |
| `7-everybody` | `chmod` | Donne la permission d'exécution à tout le monde (`u`, `g`, `o`) sur le fichier `hello`. |
| `8-James_Bond` | `chmod` octal | Modifie les permissions de `hello` pour que personne n'ait de droits, sauf les autres (mode `007`). |
| `9-John_Doe` | `chmod` octal | Donne les droits complets au propriétaire, lecture/exécution au groupe, et rien aux autres (`750`). |
| `10-mirror_permissions` | `chmod --reference` | Définit les permissions du fichier `hello` pour qu'elles soient identiques à celles de `olleh`. |
| `11-directories_permissions` | `chmod -R` | Ajoute des droits de lecture à tous les sous-répertoires du dossier courant pour tout le monde. |
| `12-directory_permissions` | `mkdir -m` | Crée un répertoire nommé `my_dir` avec les permissions `751` en une seule commande. |
| `13-change_group` | `chgrp` | Modifie le groupe propriétaire du fichier `hello` pour le passer à `school`. |

## 🚀 Utilisation

Exemple pour appliquer un script de modification de droits :

```bash
chmod u+x 5-execute
./5-execute