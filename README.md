# Lab 5

##  Standard Output

- **Default Output**: By default, the output is screen.
- **Redirect Output**: Use `>` after a command to save the output to a file.
- **cat command**: Displays the content of a text file on the screen.

## Append Output

- Use `>>` to append the output to an existing file or create and write to a new file if it doesn't exist.

## Standard Input

- By default, standard input is from the keyboard.
- Use `<` to redirect input from a file.
- You can combine `<` and `>` to manage both input and output in a single command.

## Pipelines `|`

- A pipeline (`|`) sends the output of the first command to the input of the next command.
  - Example: `command1 | command2 | command3`

## Expansion

- Special characters expand their meaning when used in shell commands.

## Tip: Backslash (`\`)

- The backslash can be used to ignore line breaks and continue a long command over multiple lines.

## Permissions

- Linux is a multi-user system.
- Files and directories have different permissions assigned to the owner, group, and others.

## Changing Permissions

- The `chmod` command is used to change file permissions.
  - Example: `chmod 600 word.txt` (owner can read/write, group and others have no access)

## Superuser

- A superuser has full system administration privileges.
- Some commands require superuser privileges, so use `sudo` before the command if you are a superuser.
  - Example: `sudo apt update`
- Type `exit` to exit a superuser session.

##  Text Editors

- In Linux, you can use CLI-based or GUI-based text editors.

## Shell Script

- You can write and run shell scripts. If there is a problem using nano (on Windows), you can use another text editor (e.g., Notepad).

## Tip: History

- Type `history` to see the previous command history.
- You can also save the history to a text file.
  - Example: `history > history.txt`

## wget

- The `wget` command is used to download files from the internet directly to your current directory.
  - Example: `wget http://example.com/file.txt`

## curl

- `curl` is used for fetching, uploading, and managing data over the internet.
  - Example: `curl [options] [URL]`

## grep

- `grep` is used to search for text within files.
  - Example: `grep "search_term" file.txt`
- **Common Options**:
  - `-i`: Case-insensitive search
  - `-v`: Invert match (find lines not containing the search term)
  - `-n`: Show line numbers along with matching lines
  - `-r`: Recursive search (searches through all files in a directory and its subdirectories)
