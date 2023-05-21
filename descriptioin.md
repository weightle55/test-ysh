# 깃 사용법
 
## 용어정리
* git : 형상관리툴
* remote / local : 원격 형상 / 내 로컬 컴퓨터 형상
* branch : 버전(형상) 단위
* commit : 로컬 저장 명령어 (항상 코멘트를 작성해야함)
* push : 로컬 to 리모트 반영
* pull : 리모트 to 로컬 반영
* checkout : 브랜치 이동
* merge : 브랜치 간의 병합 (업데이트)
* pull request : 리모트에 merge 요청 (내 작업을 최종 반영 요청)
* clone : 저장소 복제 

## 명령어 정리 
* git branch : 브랜치 목록 조회
* git branch -d 브랜치이름 : 브랜치 삭제
* git branch 브랜치 이름 : 브랜치 생성

* git checkout : 브랜치 이동
* git checkout -b 브랜치이름 : 브랜치 생성 후 그 브랜치로 이동

* git add . : 해당 브랜치의 모든 커밋할 파일들을 지정
* git add 파일명 : 해당 파일만 지정
* git commit -m "코멘트" : 위에서 add한 파일들의 변동사항을 저장(로컬반영)
-- checkout 전에 반드시 하고 넘어갈 것
* git push : 해당 브랜치를 리모트에 병합 
* git merge 브랜치이름 : 해당 브랜치를 현재 브랜치로 병합


## 작업 초기 설정
* 로컬 작업할 디렉토리를 생성 
* cd 디렉토리 이동
* git clone 깃저장소http값 -> 로그인(깃 연결)
* git checkout dev

## 작업 순서
* git checkout dev
* git pull
* git checkout 본인작업브랜치
* git merge 
---작업 진행

---작업 후
* git add .
* git commit -m "코멘트"
* git checkout dev
* git merge 본인작업브랜치
* git push 

