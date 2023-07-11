# Git 기본 문법



- ### 기본 commit 순서

  1.  Git 저장소를 초기화 한다.

     `git init`

  2.  Git config에 계정 연동한다.

     ```
     git config --global user.email "upgrade3001@naver.com"
     git config --global user.name "swpark30"
     ```

  3.  파일을 stage에  add 한다.

     `git add 파일명`

  4. stage에 있는 파일을 commit 한다.

     `git commit -m "커밋 메시지"`

  5.  로컬 저장소와 원격 저장소(github)를 연결해 준다.

     ````
     git remote add [remote하는 저장소 이름 정해준다] [remote할 git url]
     
     git remote add origin https://github.com/swpark30/Python-Git_TIL.git
     ````

  6. commit한 파일들을 push한다.

     ```
     git push [정해준 remote 이름] [push할 브랜치] 
     
     git push origin master
     ```



- ### 추가 기능들

  - git config 설정

    - config 확인

      `git config --list`

    - config 삭제

      `git config --unset user.name`

      *글로벌로 설정 했으면 글로벌을 추가해야한다.

      `git config --unset --global user.name`





