# Shell - Permissions

This project is dedicated to understanding and managing file and directory access permissions within Unix/Linux operating systems. The core objective is to master the multi-user security model, understand system roles (`owner`, `group`, `others`), and learn how to safely modify file permissions and ownership.

## 📝 Key Concepts

* **User Classes:** Defining permissions for the Owner (`u`), Group (`g`), and Others (`o`).
* **Permission Types:** Read (`r` = 4), Write (`w` = 2), and Execute (`x` = 1).
* **Permission Notations:** Utilizing both symbolic notation (e.g., `u+x,g-w`) and octal/numeric notation (e.g., `755`, `644`).
* **Management Commands:** Mastering `chmod` (change file mode bits), `chown` (change file owner and group), and `chgrp` (change group ownership).

## 🛠️ Specifications and Constraints

* **Interpreter:** Scripts written exclusively for `bash` (tested and validated on Ubuntu 20.04 LTS).
* **Formatting:** Standard `#!/bin/bash` shebang required on the very first line; all files must end with a new line.
* **Executability:** All scripts must be made executable (`chmod u+x`).

## 📁 File List & Tasks

| File | Command / Action | Description |
| :--- | :--- | :--- |
| `0-iam_betty` | `su` | Bash script that switches the current user to the user `betty`. |
| `1-who_am_i` | `whoami` | Prints the effective username of the current user. |
| `2-groups` | `groups` | Prints all the groups the current user belongs to. |
| `3-new_owner` | `chown` | Changes the owner of the file `hello` to the user `betty`. |
| `4-empty` | `touch` | Creates an empty file named `hello`. |
| `5-execute` | `chmod` | Adds execute permission to the owner of the file `hello`. |
| `6-multiple_permissions` | `chmod` | Adds execute permission to the owner and the group, and read permission to others for the file `hello`. |
| `7-everybody` | `chmod` | Adds execute permission to everybody (`u`, `g`, `o`) for the file `hello`. |
| `8-James_Bond` | Octal `chmod` | Sets the permissions of the file `hello` so that only others have full rights (mode `007`). |
| `9-John_Doe` | Octal `chmod` | Sets full permissions for the owner, read/execute for the group, and no permissions for others (`750`). |
| `10-mirror_permissions` | `chmod --reference` | Sets the permissions of the file `hello` to match exactly those of the file `olleh`. |
| `11-directories_permissions` | `chmod -R` | Adds read permission to all subdirectories of the current directory for everyone. |
| `12-directory_permissions` | `mkdir -m` | Creates a directory named `my_dir` with permissions set to `751` in a single command. |
| `13-change_group` | `chgrp` | Changes the group ownership of the file `hello` to `school`. |

## 🚀 Usage

Example of how to make a permission script executable and run it:

```bash
chmod u+x 5-execute
./5-execute