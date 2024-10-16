# Lecture 4 - CLI_1


## Kernel
**Core of OS** <br>
controls and communicates with hardware resource

## Shell
Interface that allows users to communicate with kernel: bash, zsh, ...<br>
Users runs applications and give command through shell.

There are two kinds of shell.<br>
1. **CLI**
(Command Line Interfaces)
2. GUI
(Graphical User Interface)

In this document, CLI will be mainly discussed.

---
---

### Shell Commands

- **pwd** : shows the current path in a hierarchical directory

- **cd** : change directory

- **clear** : clear the shell as if when the shell just started

- **rm** : delete files and directories ***permanentely and irreversevely***

- **mkdir** : make a new directory

- **help** : show the way to use the command typed next to help

- **man** : show an manual about the command typed next to man

- **exit** : exit terminal

- **ls** : list files and directories

|Command|Result|
|:---|:---|
|ls|list the files in the working directory|
|ls /bin|list the files in the /bin directory (or any other directory we care to specify)|
|ls -l|list the files in the working directory in long format|
|ls -la|list all files (even ones with names beginning with a period character, which are normally hidden) in the parent of the working directory in long format|

- **cp** : copy files and directories

|Command|Result|
|:---|:---|
|cp file1 file2|Copies the contents of file1 into file2. If file2 does not exist, it is created; otherwise, file2 is silently overwritten with the contents of file1.|
|cp -i file1 file2|Like above however, since the "-i" (interactive) option is specified, if file2 exists, the user is prompted before it is overwritten with the contents of file1.|
|cp file1 dir1|Copy the contents of file1 (into a file named file1) inside of directory dir1.|
|cp -R dir1 dir2|Copy the contents of the directory dir1. If directory dir2 does not exist, it is created. Otherwise, it creates a directory named dir1 within directory dir2.|

- **mv** : move or rename filed and directories

|Command|Result|
|:---|:---|
|mv file1 file2|If file2 does not exist, then file1 is renamed file2. If file2 exists, its contents are silently replaced with the contents of file1.|
|mv -i file1 file2|Like above however, since the "-i" (interactive) option is specified, if file2 exists, the user is prompted before it is overwritten with the contents of file1.|
|mv file1 file2 dir1|The files file1 and file2 are moved to directory dir1. If dir1 does not exist, mv will exit with an error.|
|mv dir1 dir2|If dir2 does not exist, then dir1 is renamed dir2. If dir2 exists, the directory dir1 is moved within directory dir2.|

<br>

### Wildcards

|Pattern|Matches|
|:---|:---|
|*|All filenames|
|g*|All filesnames that begin with the character "g"|
|b*.txt|All filenames that begin with the character "b" and end with the characters ".txt"|
|Data??|Any filename that begins with the characters "Data" followed by exactly 3 more characters|
|[abc]*|Any filename that begins with "a" or "b" or "c" followed by any other characters|
|[[:upper:]]*|Any filename that begins with an uppercase letter. This is an example of a character class.|
|BACKUP.[[:digit:]][[:digit:]]|Another example of character classes. This pattern matches any filename that begins with the characters "BACKUP." followed by exactly two numerals.|
|*[![:lower:]]|Any filename that does not end with a lowercase letter.|