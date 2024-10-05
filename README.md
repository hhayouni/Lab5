# Lecture 5: Command Line Interface (CLI) - Shell Commands

**Course:** Open Source Software  
**Instructor:** JaKeoung Koo  
**Institution:** Gachon University  


## Assignment: Lab 5 - Lecture Note on Shell Commands

- There is no predefined structure nor length of note
- Make it help you remember the shell commands
- Feel free to choose any format such as markdown, pdf, docs

---

## I/O Redirection

- **Standard Output**: 
  - By default, output goes to the **screen**.
  - Use `>` to redirect output to a file.
    ls > file.txt
  - Use `>>` to append output to an existing file or create a new file.
    echo "New line" >> file.txt

- **Standard Input**:
  - By default, input comes from the **keyboard**.
  - Use `<` to redirect input from a file.
    sort < words.txt
  - Combine both input and output redirection:
    sort < words.txt > sorted_words.txt

## Pipelines (`|`)

- Pipelines feed the output of one command as input to another command:
  command1 | command2 | command3

- Example: 
  ls | grep "txt"

## Expansion

- Special characters can expand to filenames or directories.
  - Example: `echo *` lists all files in the current directory.
  - Example: `echo ~` prints the home directory path.

## Backslash (`\`)

- Use the backslash (`\`) to break long commands into multiple lines:
  command1 arg1 arg2 \
  arg3 arg4

## Permissions and Superuser

- **Permissions**: Linux assigns permissions to **owner**, **group**, and **others**.
  - Example to change permissions:
    chmod 644 word.txt
    - Owner can **read** and **write** (`rw-`).
    - Others can only **read** (`r--`).

- **Superuser**: Some commands require superuser privileges.
  - Use `sudo` to run commands as a superuser:
    sudo apt update
  - Exit superuser mode with:
    exit

## Text Editors

- CLI-based or GUI-based text editors can be used in Linux.
  
  | Editor  | Interface   | Description |
  |---------|-------------|-------------|
  | `vim`   | CLI         | Powerful, widely-used CLI editor |
  | `nano`  | CLI         | Simple, beginner-friendly editor |
  | `gedit` | GUI         | User-friendly graphical editor   |

## Shell Scripts

- Write and execute a shell script:
  nano myscript.sh

## Tip: History

- View previous command history with:
  history
- Save command history to a file:
  history > history.txt

## wget, curl, grep

- **wget**: Download files from the internet:
  wget http://example.com/file.txt

- **curl**: Fetch, upload, and manage data over the internet:
  curl [options] [URL]

- **grep**: Search for text within files:
  grep "search_term" file.txt

  **Common options**:
  - `-i`: Case-insensitive search.
  - `-v`: Invert the match (shows lines not containing the search term).
  - `-n`: Show line numbers for matching lines.
  - `-r`: Recursive search through directories.

  **Regular expressions**:
  - `.*`: Matches any character zero or more times.
  - `^`: Matches the beginning of a line.
  - `$`: Matches the end of a line.
