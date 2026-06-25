# Holberton School - System Engineering & DevOps: Shell

Ce dépôt rassemble l'ensemble des projets dédiés à la maîtrise du système d'exploitation Unix, de la ligne de commande et des scripts Bash, réalisés dans le cadre du cursus **Holberton School**. L'objectif est d'acquérir les fondations essentielles en ingénierie système et pratiques DevOps.

## 📝 Présentation du Cursus Shell

Le parcours est conçu pour transformer la manipulation du terminal en un outil d'automatisation puissant à travers trois grands axes :
* **Navigation et Fondations :** Comprendre l'arborescence Unix et la gestion rigoureuse des fichiers.
* **Flux et Filtrage :** Maîtriser les redirections d'entrées/sorties et le traitement de données textuelles à la volée.
* **Environnement et Sécurité :** Configurer les variables système et gérer finement les droits d'accès multi-utilisateurs.

## 🛠️ Exigences & Contraintes Générales

Chaque script inclus dans ce dépôt respecte les standards stricts de l'école :
* **Environnement :** Testé et validé sur Ubuntu 20.04 LTS.
* **Shebang :** La première ligne de chaque script est exactement `#!/bin/bash`.
* **Format :** Tous les fichiers se terminent par un retour à la ligne (`\n`) et sont exempts de commentaires superflus.
* **Exécutabilité :** Tous les scripts sont rendus exécutables via la commande `chmod u+x`.

## 📁 Structure du Dépôt

Le dépôt est organisé en modules spécifiques, chacun ciblant une compétence clé du Shell :

| Répertoire | Description | Concepts Clés |
| :--- | :--- | :--- |
| `basics` | Manipulation de base du système | `pwd`, `ls`, `cd`, `mkdir`, `cp`, `mv`, `rm` |
| `io_redirections_and_filters` | Gestion des flux et filtres de texte | `>`, `>>`, `\|`, `grep`, `sed`, `awk`, `head`, `tail` |
| `init_files_variables_and_expansions` | Configuration et arithmétique | `~/.bashrc`, `export`, expansions `$((...))`, alias |
| `permissions` | Sécurité et droits d'accès | `chmod`, `chown`, `chgrp`, notation octale vs symbolique |

---

## 🚀 Guide Rapide

### Rendre un script exécutable
```bash
chmod u+x <nom_du_dossier>/<nom_du_script>