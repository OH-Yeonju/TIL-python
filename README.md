## git의 기본!

이 파일은 어떻게 만들었을까?
repositoty를 만들어서 clone 생성하여 수정중이다... 헷갈린다.

**readme.md**파일?
  프로젝트에 대한 설명 문서임

**repository**?
  커밋들이 저장되는 곳


- 내 파일을 github로 옮기기

1. git init
   로컬 저장소를 생성하는 명령어. 일단 내 파일이 들어갈 저장소를 생성하는 것

2. git remote add origin (옮길 repositoty 링크)
   어디로 옮길지 적어주는것! 만든 리포지토리에서 링크를 복사해와서 뒤에 입력한다. 괄호는 입력하지 않음

3. git add .
   뭘 옮길지 결정하는 것. .을 입력하면 전체 다 옮기는 것이고 *git add (파일이름)* 을 할시 그 파일만 옮기게 된다. 수정할 때 저장을 해야 옮겨지는게 결정됨!

4. git commit -m "메세지"
   메세지를 입력해준다. 

5. git push origin master
   파일을 넘겨보자! git push -u origin master 입력시 같은 곳으로 보낸다는 것이라 이후엔 git push만 입력해도 된다.

6. git pull
   git에서 반대로 내 컴퓨터로 파일을 가져오는것. 
   