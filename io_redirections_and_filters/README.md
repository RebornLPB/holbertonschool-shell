# Shell - I/O Redirections and Filters

This project is dedicated to mastering standard inputs and outputs in Unix, redirection mechanisms (`>`, `>>`, `<`, `|`), and utilizing command-line text filters. The objective is to learn how to chain simple commands together to perform complex data processing and manipulate files efficiently.

## 📝 Key Concepts

* **Standard Streams:** Understanding Standard Input (`stdin` - descriptor 0), Standard Output (`stdout` - descriptor 1), and Standard Error (`stderr` - descriptor 2).
* **Redirections:** Redirecting the output of a command to a file (overwriting or appending) or reading input from a file.
* **Pipelines (`|`):** Connecting the standard output of one command directly to the standard input of another command.
* **Filters & Text Commands:** Utilizing foundational commands such as `head`, `tail`, `cat`, `grep`, `sed`, `sort`, `uniq`, `wc`, and `tr`.

## 🛠️ Specifications and Constraints

* **Interpreter:** Scripts written exclusively for `bash` (tested and validated on Ubuntu 20.04 LTS).
* **Formatting:** Standard `#!/bin/bash` shebang required on the very first line; all files must end with a new line.
* **Executability:** All scripts must be made executable (`chmod u+x`).

## 📁 File List & Tasks

| File | Command / Tool | Description |
| :--- | :--- | :--- |
| `0-hello_world` | `echo` | Prints "Hello, World", followed by a new line. |
| `1-confused_smiley` | `echo` / Escaping | Prints a confused smiley `"(ˆ_ˆ)"` containing special characters. |
| `2-hellofile` | `cat` | Displays the content of the `/etc/passwd` file. |
| `3-twofiles` | `cat` | Displays the content of two distinct files passed as parameters. |
| `4-lastlines` | `tail` | Displays the last 10 lines of the `/etc/passwd` file. |
| `5-firstlines` | `head` | Displays the first 10 lines of the `/etc/passwd` file. |
| `6-third_line` | `head` / `tail` / `|` | Displays the third line of the file `iacta`. |
| `7-file` | `echo` / `>` | Creates a file named `\*\\'"Best School"\'\\*$\?\*\*\*\*\*:)` containing the text `Best School`. |
| `8-cwd_state` | `ls` / `>` | Writes the result of the `ls -la` command into a file named `ls_cwd_content`. |
| `9-duplicate_last_line` | `tail` / `>>` | Duplicates the last line of the file `iacta` and appends it to the end of the same file. |
| `10-no_more_js` | `rm` / `find` | Deletes all regular files with a `.js` extension in the current directory and its subfolders. |
| `11-directories` | `find` / `wc` | Counts the number of directories and subdirectories in the current directory (excluding `.`). |
| `12-newest_files` | `ls` / `head` | Displays the 10 newest files in the current directory, sorted by modification date. |
| `13-unique` | `sort` / `uniq` | Takes a list of words as input and prints only unique words (sorted). |
| `14-findthatword` | `grep` | Searches and displays all lines containing the string "root" in the `/etc/passwd` file. |
| `15-countthatword` | `grep` / `wc` | Counts the number of lines containing the string "bin" in the `/etc/passwd` file. |
| `16-whatsnext` | `grep` | Displays lines containing "root" along with the 3 following lines in `/etc/passwd`. |
| `17-hidethatword` | `grep -v` | Displays all lines in the `/etc/passwd` file that do not contain the string "bin". |
| `18-letteronly` | `grep` | Displays all lines of `/etc/passwd` starting with a letter of the alphabet. |
| `19-AZ` | `tr` | Replaces all uppercase letters in a stream with lowercase letters (or vice versa). |
| `20-hi` | `tr` | Removes all occurrences of the letters `c` and `C` from an input. |
| `21-reverse` | `rev` | Reverses the character order of each line read from standard input. |
| `22-users_and_homes` | `cut` | Extracts and displays usernames and their home directories from `/etc/passwd` (sorted alphabetically). |

## 🚀 Usage

To execute a script that requires filtering a stream:

```bash
chmod u+x 14-findthatword
./14-findthatword