# Shell - Basics

This project serves as an introduction to the Unix operating system and command-line manipulation using the Shell (Bash). The primary objective is to understand the command interpreter environment, navigate the Unix file system structure, and master foundational file and directory manipulations.

## 📝 Key Concepts

* **Navigation:** Fluidly moving through the Unix directory tree using absolute vs. relative paths.
* **File Management:** Creating, deleting, copying, moving, and renaming files and directories.
* **Permissions & Inspection:** Viewing file contents and understanding basic metadata directly from the terminal.

## 🛠️ Specifications and Constraints

* **Command Interpreter:** All scripts are written for `bash` and tested/validated on Ubuntu 20.04 LTS.
* **Script Formatting:** * All files must end with a new line.
  * The first line of every file must contain exactly the shebang: `#!/bin/bash`.
  * Scripts must be fully functional and free of unnecessary non-executable text.
* **Executability:** All files must be made executable using the `chmod u+x` command.

## 📁 File List & Tasks

| File | Core Command | Description |
| :--- | :--- | :--- |
| `0-current_working_directory` | `pwd` | Prints the absolute path of the current working directory. |
| `1-listit` | `ls` | Lists the contents of the current working directory. |
| `2-change_directory` | `cd` | Changes the working directory to the user's home directory (`~`). |
| `3-listfiles` | `ls -l` | Lists the contents of the current directory in long format (showing permissions, sizes, etc.). |
| `4-listallfiles` | `ls -la` | Lists all contents of the current directory, including hidden files (starting with `.`). |
| `5-listfilesdigitonly` | `ls -laN` or variant | Lists the contents of the current directory showing user and group IDs numerically. |
| `6-firstdirectory` | `mkdir` | Creates a directory named `my_first_directory` inside the `/tmp/` folder. |
| `7-movetmp` | `mv` | Moves a specific file from the current directory into the `/tmp/` folder. |
| `8-firstdelete` | `rm` | Deletes a specific file located in the current directory. |
| `9-firstdirdeletion` | `rmdir` or `rm -r` | Deletes a specific directory located inside the `/tmp/` folder. |
| `10-back` | `cd -` | Changes the working directory back to the previously occupied directory. |
| `11-lists` | Multiple `ls` | Lists the files in the current directory, the parent directory, and the `/boot` directory simultaneously. |
| `12-file_type` | `file` | Prints the type of a given file (e.g., ASCII text, executable, directory). |
| `13-symbolic_link` | `ln -s` | Creates a symbolic link pointing to a targeted file. |
| `14-copy_html` | `cp` | Copies all HTML files from the current working directory to the parent directory, only if they do not exist or are newer. |

## 🚀 Usage

To make a script executable and run it:

```bash
chmod u+x 0-current_working_directory
./0-current_working_directory