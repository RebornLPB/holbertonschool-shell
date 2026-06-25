# Shell - I/O Redirections and Filters

Ce projet est dédié à la maîtrise des entrées/sorties standards sous Unix, des mécanismes de redirection (`>`, `>>`, `<`, `|`) et de l'utilisation des filtres de texte en ligne de commande. L'objectif est d'apprendre à chaîner des commandes simples pour effectuer des traitements de données complexes et manipuler des fichiers efficacement.

## 📝 Concepts Clés

* **Flux Standards :** Compréhension de l'Entrée standard (`stdin` - descripteur 0), la Sortie standard (`stdout` - descripteur 1) et la Sortie d'erreur standard (`stderr` - descripteur 2).
* **Redirections :** Rediriger la sortie d'une commande vers un fichier (écrasement ou ajout) ou lire l'entrée depuis un fichier.
* **Pipelines (`|`) :** Connecter la sortie standard d'une commande directement à l'entrée standard d'une autre commande.
* **Filtres & Commandes Textes :** Utilisation de commandes fondamentales comme `head`, `tail`, `cat`, `grep`, `sed`, `sort`, `uniq`, `wc`, et `tr`.

## 🛠️ Spécifications et Contraintes

* **Interprète :** Scripts écrits exclusivement pour `bash` (testés sur Ubuntu 20.04 LTS).
* **Format :** Shebang `#!/bin/bash` requis sur la première ligne, fin de fichier par une nouvelle ligne.
* **Exécutabilité :** Tous les scripts doivent être rendus exécutables (`chmod u+x`).

## 📁 Liste des Fichiers & Tâches

| Fichier | Commande / Outil | Description |
| :--- | :--- | :--- |
| `0-hello_world` | `echo` | Affiche "Hello, World", suivi d'une nouvelle ligne. |
| `1-confused_smiley` | `echo` / Échappement | Affiche une émoticône confuse `"(ˆ_ˆ)"` contenant des caractères spéciaux. |
| `2-hellofile` | `cat` | Affiche le contenu du fichier `/etc/passwd`. |
| `3-twofiles` | `cat` | Affiche le contenu de deux fichiers distincts passés en paramètres. |
| `4-lastlines` | `tail` | Affiche les 10 dernières lignes du fichier `/etc/passwd`. |
| `5-firstlines` | `head` | Affiche les 10 premières lignes du fichier `/etc/passwd`. |
| `6-third_line` | `head` / `tail` / `|` | Affiche la troisième ligne du fichier `iacta`. |
| `7-file` | `echo` / `>` | Crée un fichier nommé `\*\\'"Best School"\'\\*$\?\*\*\*\*\*:)` contenant le texte `Best School`. |
| `8-cwd_state` | `ls` / `>` | Écrit le résultat de la commande `ls -la` dans un fichier nommé `ls_cwd_content`. |
| `9-duplicate_last_line` | `tail` / `>>` | Duplique la dernière ligne du fichier `iacta` et l'ajoute à la fin de ce même fichier. |
| `10-no_more_js` | `rm` / `find` | Supprime tous les fichiers réguliers se terminant par `.js` dans le répertoire courant et ses sous-dossiers. |
| `11-directories` | `find` / `wc` | Compte le nombre de répertoires et sous-répertoires dans le dossier courant (excluant `.`). |
| `12-newest_files` | `ls` / `head` | Affiche les 10 fichiers les plus récents du répertoire courant, triés par date de modification. |
| `13-unique` | `sort` / `uniq` | Prend une liste de mots en entrée et affiche uniquement les mots uniques (triés). |
| `14-findthatword` | `grep` | Cherche et affiche toutes les lignes contenant la chaîne de caractères "root" dans le fichier `/etc/passwd`. |
| `15-countthatword` | `grep` / `wc` | Compte le nombre de lignes contenant la chaîne de caractères "bin" dans le fichier `/etc/passwd`. |
| `16-whatsnext` | `grep` | Affiche les lignes contenant "root" ainsi que les 3 lignes suivantes dans `/etc/passwd`. |
| `17-hidethatword` | `grep -v` | Affiche toutes les lignes du fichier `/etc/passwd` qui ne contiennent pas la chaîne "bin". |
| `18-letteronly` | `grep` | Affiche toutes les lignes de `/etc/passwd` commençant par une lettre de l'alphabet. |
| `19-AZ` | `tr` | Remplace toutes les lettres majuscules d'un flux par des minuscules (ou inversement). |
| `20-hi` | `tr` | Supprime toutes les occurrences des lettres `c` et `C` d'une entrée. |
| `21-reverse` | `rev` | Inverse l'ordre des caractères de chaque ligne lue sur l'entrée standard. |
| `22-users_and_homes` | `cut` | Extrait et affiche les noms d'utilisateurs et leurs répertoires personnels depuis `/etc/passwd` (triés par ordre alphabétique). |

## 🚀 Utilisation

Pour exécuter un script nécessitant de filtrer un flux :

```bash
chmod u+x 14-findthatword
./14-findthatword