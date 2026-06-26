# Holberton School - System Engineering & DevOps: Shell

This repository centralizes all projects dedicated to mastering the Unix operating system, the command-line interface, and Bash scripting, completed as part of the **Holberton School** curriculum. The primary goal is to establish essential foundations in system engineering and DevOps practices.

## 📝 Shell Curriculum Overview

The pathway is designed to transform terminal manipulation into a powerful automation tool through three major axes:
* **Navigation & Foundations:** Understanding the Unix directory tree and rigorous file management.
* **I/O Streams & Filtering:** Mastering input/output redirections and on-the-fly text data processing.
* **Environment & Security:** Configuring system variables and finely tuning multi-user access permissions.

## 🛠️ Requirements & General Constraints

Every script included in this repository strictly adheres to the school's high standards:
* **Environment:** Tested and validated on Ubuntu 20.04 LTS.
* **Shebang:** The first line of every script is exactly `#!/bin/bash`.
* **Formatting:** All files must end with a new line (`\n`) and remain free of unnecessary comments.
* **Executability:** All scripts are made executable using the `chmod u+x` command.

## 📁 Repository Structure

The repository is organized into specific modules, each targeting a core Shell competency:

| Directory | Description | Key Concepts |
| :--- | :--- | :--- |
| `basics` | Core system manipulation | `pwd`, `ls`, `cd`, `mkdir`, `cp`, `mv`, `rm` |
| `io_redirections_and_filters` | Stream management and text filters | `>`, `>>`, `\|`, `grep`, `sed`, `awk`, `head`, `tail` |
| `init_files_variables_and_expansions` | Initialization files, configuration & arithmetic | `~/.bashrc`, `export`, `$((...))` expansions, aliases |
| `permissions` | Security and access rights | `chmod`, `chown`, `chgrp`, octal vs. symbolic notation |

---

## 🚀 Quick Start Guide

### Making a script executable
```bash
chmod u+x <directory_name>/<script_name>