# holbertonschool-shell
# Shell - Init files, variables and expansions

This project explores the configuration of the Shell environment, the creation and usage of variables (both local and environment), and the expansion mechanisms of Bash. The core objective is to understand how to customize the terminal and dynamically manipulate data directly on the command line.

## 📝 Key Concepts

* **Initialization Files:** Understanding the purpose and execution order of configuration files such as `/etc/profile`, `~/.bash_profile`, `~/.bashrc`, and `~/.bash_logout`.
* **Variables & Environment:** Distinguishing between local variables and environment variables (`export`), and utilizing special shell variables (`$?`, `$$`, `$#`).
* **Bash Expansions:** Mastering arithmetic expansions, aliases, and parameter expansion.

## 🛠️ Specifications and Constraints

* **Command Interpreter:** Scripts written exclusively for `bash` (tested and validated on Ubuntu 20.04 LTS).
* **Formatting:** Every file must contain the `#!/bin/bash` shebang on the very first line and end with a new line.
* **Executability:** All scripts must be made executable (`chmod u+x`).

## 📁 File List & Tasks

| File | Concept / Command | Description |
| :--- | :--- | :--- |
| `0-alias` | `alias` | Creates an alias named `ls` that executes `rm *` (for testing purposes). |
| `1-hello_you` | Variable | Prints `hello ` followed by the name of the currently logged-in user. |
| `2-path` | `PATH` | Appends a new directory to the beginning of the `PATH` environment variable. |
| `3-paths` | `PATH` / Loop | Counts and displays the total number of directories specified in the `PATH` variable. |
| `4-global_variables` | `env` | Lists all local and global environment variables. |
| `5-local_variables` | `set` | Lists all local variables, environment variables, and Shell functions. |
| `6-create_local_variable` | Assignment | Creates a new local variable named `BEST` with the value `School`. |
| `7-create_global_variable` | `export` | Creates a new environment variable named `BEST` with the value `School`. |
| `8-true_knowledge` | Arithmetic expansion | Divise the `TRUE_KNOWLEDGE` variable by 128 and prints the result using `$((...))`. |
| `9-divide_and_rule` | Arithmetic expansion | Prints the result of the division of `POWER` by `DIVIDE`. |
| `10-love_exponent_the_stars` | Power | Prints the result of `BREATH` raised to the power of `LOVE`. |
| `11-binary_to_decimal` | Base conversion | Converts a binary number stored in `BINARY` into base 10. |
| `12-combinations` | Brace expansion | Displays all possible combinations of two letters from `a` to `z`, excluding `oo`. |
| `13-print_float` | `printf` | Prints a floating-point number stored in `NUM` with exactly two decimal places. |

## 🚀 Usage

To test a script that manipulates variables:

```bash
chmod u+x 7-create_global_variable
./7-create_global_variable