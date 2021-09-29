# Git 기본 문법

**```git init```** (초기화)

​	.git 폴더가 생성되며 

​	gut bash에서는 (master)라는 표기를 확인할 수 있음

```
$ git init
Initialized empty Git repository in C:/Users/campusseven02/Desktop/test/.git/
(master) $
```



**```git add<file>```**

working directory상의 변경 내용을 staging area에 추가하기 위해 사용

​		untracked 상태의 파일을 staged로 변경

​		modified 상태의 파일을 staged로 변경

```
$ git add <디렉토리>
$ git add a.txt # 파일 하나만
$ git add a.txt b.txt report.hwp # 여러 파일
$ git add my_folder/ # 특정 폴더
$ git add . # 현재 디렉토리 모든 파일/폴더
```



**```git commit -m "커밋메시지"```**

staged 상태의 파일들을 커밋을 통해 버전으로 기록

SHA-1 해시를 사용하여 40자 길이의 체크섬을 생성하고, 이를 통해 고유한 커밋을 표기한다

커밋 메세지는 변경 사항을 나타낼 수 있도록 명확하게 표기



**```git status```**

Git 저장소에 있는 파일의 상태를 확인할 때 활용

(Working directory, Staging area)

​	파일의 상태를 알 수 있음

Modified : **Changes not staged for commit**(staging되지않은 커밋할 번경사항들)

Staged : **Changes to be committed**(커밋될 수 있는 변경사항들)

**Untracked** : 버전으로 관리된 적 없는 파일(파일을 새로 만든 경우)

**Nothing to commit, working tree clean** (커밋할 변경점이 없다, 버전이 클린함)



**```git log```**

현재 저장소에 기록된 커밋을 조회

다양한 옵션을 통해 로그를 조회할 수 있음

$ git log -1

$ git log -online

$ git log -2 --online
