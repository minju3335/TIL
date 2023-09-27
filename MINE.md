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
3. `git switch <브랜치이름>`
    - 원래 master 였던 게 kmj로 변경되어있음
4. 저장하기
5. `git add .`
6. `git commit -m "message"`
7. `git push origin <브랜치이름>`

---
### Master branch로 병합하기
- Pull requests > New pull requests > branch 선택 > Create pull request

---
### Fork (원격저장소를 자신의 원격저장소로 가져옴)
- 다른 사람의 github repository를 복제하여 어떤 부분을 수정, 추가, 삭제를 용이하게 해주는 복제 기능
- 다른 사람의 깃허브를 가져오기 위해 Clone작업을 해야 함
- 다른 사람의 repository에서 'Fork'를 클릭해서 뜨는 주소를 복사하기
- camp31 파일에서 우클릭 후 'Open to Gitbash'을 열어서 `git clone <복사한url주소>`를 입력하면 파일이 생성됨
- add, commit, push 3단계를 하고 위의 brach 병합과정을 거치면 된다
