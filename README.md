# GIT

초기설정 

git config --global user.name _____

git config --global user.email _____

git config --global에서 --global을 빼면 로컬 설정이 된다.

컬러 설정

git config --global color.ui auto
______________________________________________

CRLF 문제 설정

윈도우 

git config --global core.autocrlf true

맥, 리눅스

git config --global core.autocrlf input

______________________________________________

시작
1. 프로젝트 폴더
2. git init . or
   git clone ___(remote address)___
3. git remote add __(alias)__ __(remote address)__

 대부분 alias에는 origin을 넣는다.
______________________________________________

파일 제외

.gitignore 

node_modules

dbinfo

.obj

등등....
______________________________________________

확인
1. git remote -v  -> URL + 별칭(alias)등의 정보를 보여준다.
2. git remote show __별칭__
3. git log  -> 로그 확인
4. git diff - > 스테이지 영역과 워킹 영역 비교
5. git branch -> 브랜치 목록
6. git rev-parse __branch_name__ -> 브랜치가 가리키고 있는 해시 값 출력
7. git branch -v -> 브랜치 세부 사항 확인

______________________________________________

서버 통신
1. git pull  -> 로컬 저장소로 원격 저장소 내용을 받는다.
2. git add . -> staging 영역에 로컬 작업 내용을 올린다,
3. git commit -m "__content__" -> 로컬 저장소에 커밋 한다.
4. git push __원격 별칭__ __branch__ -> 원격 저장소 주소의 branch에 내용을 업로드 한다.

브랜치
1. git branch
2. git branch __branch_name__ (commit ID) -> 브랜치 생성 ()는 생략 가능
3. git checkout __branch_name__           -> 현재 브랜치를 떠나 해당 브랜치로 이동
4. git checkout -                         -> 이전 브랜치로 이동
5. git checkout -b __branch_name__        -> 브랜치를 생성하면서 브랜치 이동
6. 
   
______________________________________________

임시
1. git fetch - 새로운 마스터 브랜치를 만든다.
2. git merge __Alias__/__branch_name__ - 로컬 저장소에 병합
3. 

______________________________________________

스테이지 영역
1. git rm --cached __FILE_NAME__ - 스테이지 영역에서 해당 파일 삭제
=> 주의 한 번이라도 commit 상태에 올렸다면 reset을 해야한다. 파일이 삭제되거나 변조된것으로 간주하기 때문

______________________________________________

단축키
1. git commit -a - add와 commit을 동시에 한다.

______________________________________________

되돌리기
1. git checkout -- __file_name__ - 해당 파일을 이전에 작성한 버전으로 되돌린다.

______________________________________________

로그
1. git log
2. git log --pretty=short   - 첫 번째 줄의 커밋 메시지만 출력
3. git log __file_name__    - 특정 파일의 로그 확인
4. git log --graph --all    - 그래프로 커밋 내역 확인

______________________________________________

패턴
1. git pull -> git commit -am "" -> git pull -> git push origin master






