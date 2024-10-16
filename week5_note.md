# Lecture 5 - CLI_2


## I/O Redirection: Standard Output

- ">" : You can redirect output using “>” after a command to create and **save the
output** in a file

- ">>" :  You can **append** output to an extising file (if it already exitsts),
or create and write to a new file if it doesn’t exist.

- "sort < {file} > {another_file}" : **sort** a file and save the sorted file to another_file

---

- "|"(Pipline) : Pipeline feeds output of previous command to input of next command. You can write multiple commands in a line.

- "\"(Backslash) : Backslah can be used to ignore line change in command (“enter”), to enter a long command in multiple lines.

---

## Permissions
Linux is a multi-user system.<br>
Files and directories have a permission assigned differently to owner / group / others.

### Changing Permissions
- **chmod** : changes permissions<br><br>$ chmod NNN words.txt
    <br> first N is for owner, second N is for group, and last N is for others

|Value|Meaning|
|:---|:---|
|777|rwxrwxrwx|
|755|rwxr-xr-x|
|700|rwx------|
|666|rw-rw-rw-|
|644|rw-r--r--|

### Superuser
A superuser has all system administation authority.
<br>Some commands need superuser’s privilleges.
<br>Put “sudo” before the command if you are a superuser.

---

### Text Editors

- vi, vim
- Emacs
- nano
- gedit
- kwrite

### history
"history" is a command to see previous command history.

### wget
"wget" is a command that downloads files from the internet directly to your active directory.

### curl
"curl" is a command for fetching, uploading, and managing data over the Internet

### grep
"grep" is a command used for searching text within files.