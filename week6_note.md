# Git 1 - lecture 6

### git is a distributed version control flatform for programmers

## Setup
Check whether git is installed or not<br>
If git was not installed, you should install git.
```
git --version
```

How to setup
```
$ git config --global user.name "Jiseok Moon"
$ git config --global user.email your-email-address
$ git config --global init.defaultBranch main
```

Check setup is done or not
```
$ git config --list
```

Initializing a Repository in an Existing Directory
```
{directory} $ git init
```
---

Checking Repository Status
```
$ git status
```

Adding files to be staged
```
$ git add {file_name}
$ git add .
```
Unstaging files
```
git rm --cached {files}
```
Commit
```
$ git commit -m "{commit message}"
```
Change Branch Name
```
git branch -m {origin_name} {new_name}
```

