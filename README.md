# Git_usage

Summary of github usage
---------------------------

### `Github`
Push전에 Pull을 하여 자료가 덮어씌워져 자료가 손실되는 것을 방지합니다.

* Root Folder 연결
1. git init
     - 새로 생성한 프로젝트 폴더 안에 .git 폴더를 생성합니다.
2. git remote add origin "Repository 주소"
     - 사용할 Repository 연결(?)합니다.

* Push(git Repository로 자료를 올립니다.)
1. git status
     - 로컬 폴더와 git과의 싱크를 체크합니다.
2. git add .
     - 로컬 폴더와 git Repository 사이의 변경된 파일들이 있을 때 모두 traking합니다.
3. git commit -m "message"
     - 개발자들이 알아볼 수 있는 commit을 다는 명령어입니다.
4. git push origin master
     - git에 push를 합니다.

* Pull(다른 곳에서 자료를 가져옵니다.)
1. git pull origin master
     - 지정해 놓은 Repository의 모든 자료를 끌어옵니다.


* Fork
1. 내 repositoty에 추가할 상대 프로젝트를 fork로 찍어온다.

2. fork할 상대의 repository에서 URL(Clone URL)을 복사하여 받아온다.(*git Clone)
     - git clone [Clone URL]

3. pull-request 작업을 수행할 branch를 생성하고 생성한 branch로 변경합니다
     - git checkout -b [branchName]

4. 원본 프로젝트 repository를 원격 repository에 추가합니다.
     - git remote add origin [Clone URL]

5. 만들어진 branch들 확인
     - git branch

6. 만들어진 branch에서 하고자 하는 프로젝트의 코드 수정과 파일을 추가합니다.

7. 추가한 파일 또는 폴더를 add 합니다.
     - git add [filename]

8. 준비된 파일들을 commit하고 메시지를 남깁니다.
     - git commit -sm "[commit mesagge]"

9. fork한 repository의 branch로 push합니다.
     - git push origin [branch]

10. fork한 repository에서 pull-request를 합니다.
     - 원하는 메시지를 write 칸에 작성합니다.

11. pull-request를 받은 원본 repository 관리자는 요청받은 내용을 확인 후 merge 여부를 결정합니다.
     - branch가 master(기본 생성 branch)인지 확인 후 아닐 경우 branch을 변경합니다.
     - git status(작업 상태 확인)
     - git checkout master(브랜치 변경)

12. branch가 master인 상태에서 전에 작업한 branch와 merge합니다.
     - git merge [branchName]

13. merge 이후 동기화와 branch 삭제
     - 원본 repository에 merge가 완료되면 작업하던 branch를 삭제합니다.
     - 코드 동기화: git pull origin
     - branch 삭제: git branch -d [branchName]
