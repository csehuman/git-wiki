# Gitmoji 사용법
### 목차:
- [Gitmoji란?](#question)
- [Gitmoji 사용법 #1: 외워서 쓰기!](#option-one)
- [Gitmoji 사용법 #2: gitmoji-cli 사용하기!](#option-two)
---
<a name="question"></a>
### Gitmoji란?
> 🐙 GitHub 커밋을 예쁘게 만들어주는 이모티콘들! 🐙

> ex)\
`Initial Commit` 보다 `🔥Initial Commit`이 훨씬 예쁘다!!

이렇게 gitmoji를 활용해 레포를 좀 더 컬러풀하게 가꾸도록 해보자!

---
<a name="option-one"></a>
### Gitmoji 사용법 # 1: 외워서 쓰기!<br/>

<br/>

**사용법 요약:**
1. 커밋 이름에 들어갈 gitmoji에 상응하는 이름을 찾는다.
- [Gitmoji 사전](https://gitmoji.carloscuesta.me/)에 접속
- 원하는 gitmoji 선택, 이에 상응하는 이름 찾기. ex) 🐛: bug
2. 변경된 파일을 스테이지에 올리고, gitmoji 이름를 `:gitmoji이름:` 형태로 커밋 이름에 추가, 커밋 실행
```
git add .
git commit -m ":bug: Found a bug!"
```
3. 해당 커밋을 푸쉬하고, 깃허브에서 커밋 기록을 확인한다.
```
git push 
```
깃허브 커밋 기록 확인 결과:
`🐛 Found a bug!`
<br/><br/>

**사용법 1의 단점:**
- 커밋할 때 마다 gitmoji 사전을 접속하거나 
- gitmoji 이름을 외워야 한다!

---
<a name="option-two"></a>
### Gitmoji 사용법 #2: [gitmoji-cli](https://www.npmjs.com/package/gitmoji-cli) 사용하기!<br/><br/>
**초기 설치:**
1. gitmoji-cli 설치하기
- npm 사용시:
```
npm i -g gitmoji-cli
```
- brew 사용시:
```
brew install gitmoji
```
- npm도 brew도 없을 시,\
[npm 설치](https://web-front-end.tistory.com/3) (Windows/ MacOS) 하거나\
[brew 설치](https://jungwoon.github.io/google%20cloud/2018/02/22/Install-Homebrew/) (MacOS) 후 진행
<br/><br/>

**사용법 요약:**
1. 변경된 모든 파일을 스테이지에 올리기
```
git add .
```
2. 깃모지 커밋 명령 실행하기
```
gitmoji -c
```
3. 사용할 깃모지 선택 후, `Enter`
- `Choose a gitmoji`가 화면에 나올 시, 위아래 방향키 통해 깃모지 목록들 볼 수 있음.
- 원하는 깃모지나, 현재 상황등을 검색하면 이에 맞는 깃모지 목록들이 나올 것임. ex) bug, new, initial 등
- 원하는 깃모지 선택

4. 커밋 제목 지정한 후, `Enter`
- 깃모지는 무조건 제목 전에 나올 것 ex) 💡Hello
- 원하는 커밋 제목 (title) 지정

5. 커밋 내용 지정한 후, `Enter`
- 커밋에 들어갈 내용 작성.
- 원하는 내용 없을 시, 비어둔 채로 넘어가도 됨.

6. `Enter`누를 시, 커밋이 생성됨.

7. 해당 커밋 푸쉬 후, 깃허브에서 커밋 결과 확인하기

