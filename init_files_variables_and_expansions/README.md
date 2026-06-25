# holbertonschool-shell
# Shell - Init files, variables and expansions

Ce projet explore la configuration de l'environnement Shell, la création et l'utilisation des variables (locales et d'environnement), ainsi que les mécanismes d'expansion de Bash. L'objectif est de comprendre comment personnaliser son terminal et manipuler dynamiquement les données en ligne de commande.

## 📝 Concepts Clés

* **Fichiers d'Initialisation :** Rôle et ordre d'exécution des fichiers de configuration comme `/etc/profile`, `~/.bash_profile`, `~/.bashrc` et `~/.bash_logout`.
* **Variables & Environnement :** Différence entre variables locales et variables d'environnement (`export`), et utilisation de variables spéciales (`$?`, `$$`, `$#`).
* **Expansions Bash :** Fonctionnement des expansions arithmétiques, des alias, et de l'expansion des paramètres.

## 🛠️ Spécifications et Contraintes

* **Interprète de commandes :** Scripts écrits exclusivement pour `bash` (testés sur Ubuntu 20.04 LTS).
* **Format :** Chaque fichier doit contenir le Shebang `#!/bin/bash` sur la première ligne et se terminer par un retour à la ligne.
* **Exécutabilité :** Tous les scripts doivent être rendus exécutables (`chmod u+x`).

## 📁 Liste des Fichiers & Tâches

| Fichier | Concept / Commande | Description |
| :--- | :--- | :--- |
| `0-alias` | `alias` | Crée un alias nommé `ls` qui exécute `rm *` (à des fins de test). |
| `1-hello_you` | Variable | Affiche `hello ` suivi du nom de l'utilisateur actuel connecté. |
| `2-path` | `PATH` | Ajoute un nouveau répertoire au début de la variable d'environnement `PATH`. |
| `3-paths` | `PATH` / Boucle | Compte et affiche le nombre de répertoires présents dans la variable `PATH`. |
| `4-global_variables` | `env` | Liste toutes les variables d'environnement locales et globales. |
| `5-local_variables` | `set` | Liste toutes les variables locales, d'environnement ainsi que les fonctions Shell. |
| `6-create_local_variable` | Assignation | Crée une nouvelle variable locale nommée `BEST` avec pour valeur `School`. |
| `7-create_global_variable` | `export` | Crée une nouvelle variable d'environnement nommée `BEST` avec pour valeur `School`. |
| `8-true_knowledge` | Expansion arithmétique | Divise la variable `TRUE_KNOWLEDGE` par 128 et affiche le résultat (`$((...))`). |
| `9-divide_and_rule` | Expansion arithmétique | Affiche le résultat de la division de `POWER` par `DIVIDE`. |
| `10-love_exponent_the_stars` | Puissance | Affiche le résultat de `BREATH` élevé à la puissance `LOVE`. |
| `11-binary_to_decimal` | Base conversion | Convertit un nombre binaire stocké dans `BINARY` en base 10. |
| `12-combinations` | Expansions de blocs | Affiche toutes les combinaisons possibles de deux lettres de `a` à `z`, sauf `oo`. |
| `13-print_float` | `printf` | Affiche un nombre flottant stocké dans `NUM` avec exactement deux décimales. |

## 🚀 Utilisation

Pour tester un script manipulant des variables :

```bash
chmod u+x 7-create_global_variable
./7-create_global_variable