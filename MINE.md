![제노](/Markdown/assets/D2.jpg)
>화이팅


---

### git을 사용해서 작성한 내용물을 저장하는 것
- `git remote add origin https://githup.com/minju3335`
 - 위 주소를 origin이라고 부르기로 함
- `git push origin master` : 원격저장소에 저장
- 파일 내용 수정하기
- Ctrl + s 눌러서 저장하기
- `git add .` : 수정한 모든 내용을 stage에 올림
- `git commit -m "해당내용"`: 코멘트를 다는 것 (저장 안하면 안됨 !)
- `git push origin master` : 위 내용을 github에 올림




---
### 다른 사람이 만든 코드 복제해오기 (pull이라고 부름)
- 협업할 때 사용
- 터미널을 사용해줘야 함
1. 폴더 여백에 마우스 우클릭해서 'open gitbash'열기
2. `pwd`로 위치 확인 > `cd ~` > `cd Desktop/camp31`
3. 초록색 code버튼에 주소를 복사해서 터미널 `git clone <주소>`를 입력
4. 생성된 폴더에 들어가서 여백에 '코드로 열기'로 열기


---
### 다른 사람이 수정한 부분 가져오기
1. `git pull origin master` : 다른 사람이 수정한 부분을 가져옴
2. 추가/수정 뒤에 **저장**하기 **꼭꼭꼭**
3. 다시 `add > commit -m > push`를 해줌
- 다만 다른 내용을 가져오면 충돌함 -> 택1로 충돌해결하기 (merge)


---
### branch를 따로 만들어 분업하기
1. `git branch` : 브랜치 생성
2. `git branch -c <브랜치이름>` (보통 이름은 기능을 따름)
3. 