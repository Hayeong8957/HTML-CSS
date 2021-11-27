# 💻 모각코 11월 과정 : HTML+CSS 심화

### 📌 1일차 : 웹 개발 이해하기(html, css, javascript)
- 웹 개발에 대한 전체적인 기초 개념을 숙지
- 나의 첫 html 파일 만들기

### 📌 2일차 : HTML, css 본격 시작하기
- html의 기본 구조
- css 활용 방법: class, id 이해하기
- 나만의 위키 만들기(html, css)

### 📌 3일차 : 웹 폰트 적용하기
- css를 적용하는 3가지 방법(style속성, 내부 스타일 시트, 외부 스타일 시트)
- 웹 폰트 이해하기 / 적용하기(link방식, @import방식, @font-face방식)
- 2일차 파일에서 css파일 분리한 후, 웹 폰트 2개 이상 적용하기

### 📌 4일차 : 크기 적용
- 패딩(padding)과 마진(margin)
- 다양한 단위(px, em, rem, %)
- 네비게이션바 만들며 패딩, 마진 개념 복습

### 📌 5일차 : 레이아웃 만들기
- div태그와 span태그는 기본으로 설정되어 있는 디자인 속성이 거의 없다.
- display 속성(block, inline, inline-block)
- position 속성(static, relative, absolute, fixed)
- 미니홈피 기본 레이아웃 

### 📌 6일차 : 홈화면-구조 만들기
- flex 속성의 기초(큰 박스 > 작은 박스 순서로 만든다.)
  - flex로 복잡한 레이아웃을 만들 수 있다.
  - container와 item ▶ 가로로 혹은 세로로 쌓이도록 배치하고 싶은 박스가 flex item, 아이템을 둘러싼 박스가 container
  - display: flex; ▶ 필수
  - flex-direction: row vs column ▶ row = 가로로 쌓기, column = 세로로 쌓기
  - flex: 숫자; ▶ 숫자는 컨테이너의 면적 중에서 차지할 면적의 비율
- 미니홈피 홈화면 레이아웃 만들기 : flex 레이아웃 사용 1

### 📌 7일차 : Flex 속성 적용하기
- flex 레이아웃의 아이템에 적용할 수 있는 속성
  - flex-basis ▶ 아이템의 기본 크기
  - flex-grow ▶ 아이템이 얼마나 커질지 설정
  - flex-shrink ▶ 아이템이 얼마나 작아질지 설정
  - flex ▶ flex-basis, flex-shrink, flex-grow를 한번에 설정
- flex 레이아웃의 컨테이너에 적용할 수 있는 속성
  - flex-direction ▶ flex 레이아웃의 방향 설정
  - flex-wrap ▶ flex 아이템이 컨테이너 크기를 넘어갈 때 처리 방법
  - align-items ▶ 수직축으로 정렬하기
  - justify-content ▶ 수평축으로 정렬하기
- 미니홈피 홈화면 레이아웃 만들기 : flex 레이아웃 사용 2

### 📌 8일차 : css 파일 분리하기

### 📌 9일차 : 홈 화면 완성하기
- 여러가지 선택자 활용하기
  - 띄어쓰기 없이 선택자 붙여쓰기 ▶ 여러 조건에 적용(AND)
  - 쉼표로 구분하여 선택자 나열하기 ▶ 여러 조건에 적용(OR)
  - 띄어쓰기로 선택자 나열하기 ▶ 하위 요소에 적용
  - `>` 로 구분하여 선택자 나열하기 ▶ 하위 요소에 적용(사이에 다른 태그가 없어야 함)
  - 선택자: 상태 ▶ 특정 상태일 때 적용 (hover, active, focus)
- 다양한 선택자 활용하여 파도타기 버튼(Dropdown), 메뉴 버튼 완성

### 📌 10일차 : 스크롤 만들기-overflow
- overflow 속성
  - overflow 속성은 스크롤과 관련, overflow-x + overflow-y 이다.
  - visible ▶ 내용물이 항상 다 보여짐
  - auto ▶ 스크롤이 필요할 때만 스크롤 생김
  - scroll ▶ 항상 스크롤바 있음
  - hidden ▶ 컨테이너 초과하는 내용물을 안보이게 함
- 미니홈피 사진첩 만들기(overflow 속성 사용)

### 📌 11일차 : 미니홈피 다이어리 만들기
- 외부 라이브러리 적용(font-awesome)
- transition 속성
  - 속성 값이 변할 때 애니메이션을 적용할 수 있는 속성
  - ```transition: 800ms ease all;```
  - ```800ms``` ▶ 속성이 변하는 시간
  - ```ease```  ▶ 애니메이션 종류
  - ```all```   ▶ 적용할 속성

### 📌 12일차 : 미니홈피 다이어리 비밀글 추가
- Javascript로 파일 불러오기
<details>
<summary>Javascript 코드 해석</summary>
<div markdown="1">

1) 버튼을 누르면 ```getTextFile```이라는 함수가 실행된다.

2) ```<input>``` 태그 요소 하나를 만들고, 해당 요소의 이름을 input이라고 붙인다. (변수명)

3) input 태그의 속성을 정해준다. (ex. ```input.type```)
이렇게 만들어주면 ```<input type="file" accept="text/plain" />```이라는 html 코드와 같아진다.

4) ```input.onchange```코드는 ```<input>``` 태그가 변화했을 때 (즉, 파일 열기 버튼을 눌러서 파일이 추가되었을 때) ```processFile```이라는 함수가 실행되고, ```processFile``` 함수의 인자(file)로 파일을 넘겨준다.

5) ```processFile``` 함수에서는 넘겨받은 file을 읽어서 표시한다.
파일을 읽을 수 있는 reader라는 변수를 만들고, uft-8 형식을 적용한다. (한글을 읽기 위함)

6) ```reader.onload```부분은 reader가 파일을 읽으면 function () { .... } 중괄호 안의 부분이 실행된다.
```document.getElementById("text")```를 통해 text라는 id를 가진 요소를 찾아
```~.innerText = reader.result``` 코드로 해당 요소의 innerText, 즉 텍스트를 reader가 읽은 결과 텍스트로 대체한다.

</div>
</details>
