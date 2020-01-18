# Just practice for basic git

## 유용한 명령어
* status : 현재 상태를 보여준다.
* log : 커밋 로그를 보여준다.

## 첫번째 커밋
1. init : 현재 로컬 폴더에 .git폴더를 만들어준다.
2. add . : 현재 로컬 폴더를 전부 추가한다
3. commit -m "메세지" : commit하기!
4. remote add origin {주소} : origin에 {주소}라는 리포지토리와 연결 (remote -v로 확인 가능)
5. push origin master : origin이라는 리모트에 master라는 브랜치로 푸시

## pull도 해보기
> git pull origin master

## Branch
git branch : 현재 브랜치 목록
git checkout -b {이름} : 새로운 브랜치를 만든다.
git branch {이름} : 해당 브랜치로 이동 -> 로컬 파일도 바뀐다!

## Conflict 로컬에서 해결하기
1. git remote add upsteam {원래 리포지토리 주소} : git remote -v로 리모트에 upsteam이 추가 되었는지 확인
2. git fetch upsteam master : git branch -a로 임시 브랜치가 추가되었는지 체크 
3. git merge upsteam/master : 현재 내 브랜치와 가져온 브랜치를 merge한다.
4. git status로 어떤 부분이 컨플릭트가 났는지 확인 후 수정한다.

