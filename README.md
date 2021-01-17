# Git_usage

Summary of github usage
---------------------------

     Github
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
     
     * Clone
