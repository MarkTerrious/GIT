# GIT

초기설정 
git config --global user.name _____
git config --global user.email _____

git config --global에서 --global을 빼면 로컬 설정이 된다.

컬러 설정
git config --global color.ui auto

______________________________________________

시작
1. 프로젝트 폴더
2. git init . or
   git clone ___(remote address)___
3. git remote add __(alias)__ __(remote address)__

 대부분 alias에는 origin을 넣는다.
 
______________________________________________

확인
1. git remote -v  -> URL + 별칭(alias)등의 정보를 보여준다.
2. git remote show __별칭__
3. git log  -> 로그 확인

______________________________________________

서버 통신
1. git pull  -> 로컬 저장소로 원격 저장소 내용을 받는다.
2. git add . -> staging 영역에 로컬 작업 내용을 올린다,
3. git commit -m "__content__" -> 로컬 저장소에 커밋 한다.
4. git push __원격 별칭__ __branch__ -> 원격 저장소 주소의 branch에 내용을 업로드 한다.
   
______________________________________________



