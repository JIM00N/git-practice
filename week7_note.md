# Week 7 - git 2

```
$ git init

$ git status

$ git add {file_name}

$ git add .

$ git branch -m {file1} {file2}

$ git rm {file_name}
```

```
$ git rm --cached {file_name}
$ git reset HEAD {file}
$ git restore --staged {file}
**unstaging a staged file**
```
- git rm --cached:
스테이징된 파일을 Git의 추적에서 완전히 제거.<br>
파일은 로컬 디스크에 그대로 남아 있지만, Git이 추적하지 않음.<br>
**주로 .gitignore를 설정한 후 파일을 Git에서 제거할 때 사용.**
- git reset HEAD:
스테이징된 변경 사항을 취소하고, 다시 워킹 디렉토리로 돌림.<br>
파일은 Git이 계속 추적하며, 변경 사항은 그대로 남아 있음.
**스테이징에서만 파일을 해제하고 싶을 때 사용.**
- git restore --staged:
특정 파일을 스테이징 영역에서 해제.<br>
변경 사항은 워킹 디렉토리에 그대로 유지되며, git reset보다 명확한 파일 지정 방식.
파일을 스테이징에서 제외하고 싶을 때 사용.


```
$ git restore {file}
```
- Unmodifying a modified file <br>
unmodify != unstaging


## Unmodifying vs Unstaging
- Unmodifying: Cancels modifications in the working directory. <br>The changes are discarded, and the file is restored to its committed state

- Unstaging: Removes a file from the staging area.<br>
The file stays modified, but it is no longer part of the next commit.