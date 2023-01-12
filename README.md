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


- 이 외

연결되어 있는 원격 저장소 확인하기
git remote -v

어떤 이름이 어디에 연결되어 있는지 확인가능! 오류가 여기서 많이 발생하니 확인하라!

git remote remove 연결이름명

이러면 연결되어 있는 저장소가 끊어진다. 나의 오류는 여기서 많이 발생한다. 훨씬 쉽게 오류 고치기 가능! 이후 git remote -v를 이용하면 여전히 연결되어있는 상태인지 아닌지 볼 수 있음. 다시 연결하고 싶을 땐 git remote add 다시 써주면 됨

**main 인지 master인지 확인!**


7. 오류!!!!!!!!!!!!   

error: src refspec master does not match any
git에 push 할 때 발생하는 오류이다
해결법!!!
git 정보가 틀어져서 그런거니 git을 초기화 해준다
git init 로 초기화 해준다!