# HTML 기초

## 섹션 0

### 1. HTML이란?

HTML =
<u>H</u>yper
<u>T</u>ext
<u>M</u>arkup
<u>L</u>anguage

<u>HyperText:</u> 하이퍼링크를 통해 어떤 문서에서 다른 문서로 접근할 수 있는 텍스트 </br>
<u>Markup:</u> 컨텐츠 표시 </br>
<u>Language:</u> 언어 </br>

- 하이퍼 텍스트와 컨텐츠를 표시해주는 언어; HTML은 웹브라우저를 통해 표시되는 웹페이지의 컨텐츠를 정의하기 위해 사용하는 언어
- 웹페이지의 컨텐츠를 정의하기 위해 사용하는 언어; HTML 코드로 웹페이지에 어떤 내용이 표시될지 정의한 HTML 문서 작성
- 완성된 HTML 코드를 웹브라우저에서 로딩하면 웹페이지가 만들어짐; HTML 코드가 웹브라우저를 통해 해석되고 표현되는 과정: 렌더링

### 2. HTML 문서 만들기

HTML 파일의 확장자는 html 또는 htm </br>
파일을 수정하고 싶다면 텍스트 편집기로 (notepad, Brackets, VSCode, etc.) </br>
결과를 확인하고 싶다면 웹브라우저로 (Chrome, Firefox, Safari, etc.)

### 3. 개발자 도구

웹사이트 개발용 도구로, 대부분 최신 브라우저에는 개발자 도구가 탑재 </br>
HTML, CSS 코드 확인, 모바일 모니터링, 네트워크 상태 점검, 스크립트 명령어 확인 등 다양한 기능을 통해 개발자에게 편의 제공

- Elements
- Console
- Sources
- Network

### 4. 코드 에디터

개발자가 프로그램 소스 코드를 편집하기 위해 사용하는 소프트웨어 </br>
코드는 텍스트이며 빠르고 편하게 코드(텍스트)를 작성하기 위해 코드 에디터를 사용 </br>
자동 완성, 하이라이트 등의 기능이 있음

<hr>
<hr>

## 섹션 1

### 1. HTML 태그 사용법: 시작과 끝

태그는 <>, </>를 사용해 컨텐츠의 시작과 끝 표시 </br>
각 태그는 컨텐츠를 감싸며 태그명은 컨텐츠의 성격과 의미를 나타냄 </br>
ex. `<태그>컨텐츠</태그>`

### 2. HTML 태그 사용법: 단일 태그

경우에 따라 시작과 끝을 구분할 필요가 없는 태그 존재 </br>
ex. `<!DOCTYPE html>`

### 3. HTML 태그 사용법: 속성

태그의 부가적 기능을 정의하는 것으로, 선택사항 </br>
속성은 시작 태그의 내부에 정의; 속성의 개수에는 제한 없음 </br>
ex. `<link rel="stylesheet" href="">` 에서 rel, href 등

### 4. HTML 태그 사용법: 주석

코드에 대한 메모를 남기기 위해 사용 </br>
ex. `<!--  -->`

### 5. HTML 문서의 구조

**HTML 문서의 기본구조**

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>

  </body>
</html>
```

**HTML 문서의 기본구조: 설명** </br>
`<!DOCTYPE html>` : 문서의 첫 부분에서 문서 유형(HTML 버전) 지정하는 단일태그 </br>
`<html></html>` : 문서 유형 지정 후 실제 문서가 시작되고 끝나는 지점을 나타내는 태그 </br>
`<head></head>` : 웹 브라우저 화면에는 보이지 않지만 웹 브라우저가 알아야 할 정보를 나타내는 범위; 제목, 설명, 스타일 등등 </br>
`<body></body>` : 웹 브라우저 화면에 표시될 내용이 입력되는, 구조를 나타내는 범위; 텍스트, 이미지, 사용자 인터페이스 태그 등을 포함하여 다양하게 구성할 수 있음 </br>

### 6. HTML 텍스트 태그

문단: `<p></p>`; 문단 요소를 나타내는 태그로 가장 많이 사용되는 텍스트 태그;
하나의 p 태그는 하나의 문단을 표현하며, 문단과 문단 사이에는 공백이 있음 </br>
제목: `<headline></headline>`; 제목(표제) 요소를 나타내는 태그로 h1 ~ h6까지 있음 </br>
수평선: `<hr>`; 수평선을 표시하는 태그로 주제 변경 또는 내용 구분을 위해 사용됨

### 7. HTML 텍스트의 특징

일반적으로 Enter키는 줄바꿈을 의미하나 HTML 코드에서는 이를 무시하며 공백도 한번만 인정됨 </br>
HTML에서는 `</br>` 태그가 줄바꿈을, `&nbsp;`가 공백을 표현

### 8. 태그의 구분

태그 구분 : 개발자 도구 활용

- 블록 레벨 요소 : 자기가 속한 영역의 너비를 모두 차지하여 블록 형성
- 인라인 레벨 요소 : 자기에게 필요한 만큼의 공간만 차지

### 9. img

img 태그는 이미지를 표시할 때 사용하는 단일 태그 </br>
기본 형태 : `<img src="이미지파일.jpg" alt="이미지설명">` </br>
src는 이미지의 url을, alt는 이미지 로딩 전 또는 로딩에 실패할 경우 이미지 대신에 표시하는 텍스트 </br>
width, height 속성을 사용하여 정수 픽셀 단위로 크기를 조절할 수 있음 </br>

### 10. 컨테이너 태그

컨텐츠나 레이아웃에 영향을 주지 않고, 단지 다른 요소 여럿을 묶어 관리하기 편하게 만드는 역할을 하는 태그를 '컨테이너'라 함 </br>
컨텐츠 내용을 구분하거나 공통적인 스타일을 적용하고자 할 때 개발자는 컨테이너를 사용하는 것이 좋음 </br>

- `<div></div>`
- `<span></span>`

### 11. 전역 속성 (Global Attributes)

전역 속성은 모든 HTML 태그에서 공통적으로 사용할 수 있는 속성 </br>
속성이란 태그의 부가적 기능을 정의하는 것으로, 선택사항임 </br>
속성은 시작 태그의 내부에 정의하며 속성의 개수에는 제한이 없음 </br>

- id : 태그명이 같은 요소들을 식별하기 위해 사용; 태그당 하나
- class : 태그명이 같은 요소들을 식별하기 위해 사용; 다중 지정 및 중복 가능
- style
- title

특정 태그에만 지정 가능한 속성들도 존재

### 12. a

링크란 현재 문서에서 다른 문서로 이동할 수 있는 수단 </br>
anchor(`<a></a>`) 태그 요소의 href 속성을 통해 다른 페이지, 전화번호, 이메일 주소와 그 외 다른 url로 연결할 수 있는 링크를 만듦 </br>
인라인 요소이며, 컨텐츠는 주로 링크의 목적지를 나타냄 </br>
target 속성을 이용하면 새로운 문서를 열 때 현재 탭에서 열지, 새로운 탭에서 열지 결정할 수 있음

### 13. list

목록은 연관 있는 항목(item)들을 나열 </br>
HTML 목록은 '순서 없는 목록'과 '순서 있는 목록'으로 구분 </br>

- `<ul></ul>` : unordered list; 순서 없는 목록
- `<ol></ol>` : ordered list; 순서 있는 목록
- `<li></li>` : list item; 항목

### 14. input

사용자로부터 값을 입력받을 수 있는 대화형 컨드를(또는 '필드')을 나타냄 </br>
기본적으로 인라인 요소이며, 단일 태그 </br>
type 값에 따라 입력 요소의 형태나 입력 데이터 유형이 달라짐; 속성 종류도 달라짐 </br>
사용 가능한 type은 20여가지이며, 기본값은 text </br>
name 속성으로 input 요소를 구별할 수 있음 </br>

### 15. select, option

select는 다수의 옵션을 포함할 수 있는 선택 메뉴 </br>
메뉴(dropdown) 안에 포함되는 옵션은 option 태그를 통해 표시; </br>
select에는 name을 지정할 수 있으며 </br>
각각의 option에는 value를 지정할 수 있음; value는 실제로 처리될 값을 나타냄(server-side) </br>
select와 option 모두 인라인 요소

### 16. textarea

textarea는 여러 줄의 일반 텍스트를 입력할 수 있는 입력 요소 </br>
name을 지정하여 구분할 수 있음

### 17. form

form은 사용자가 입력한 데이터(입력값)을 서버로 보내기 위해 사용하는 태그 </br>
form은 입력 요소들을 감싸며, 입력 값을 서버 측으로 제출(submit)할 수 있음 </br>
form의 입력 값을 위해 input 태그의 type 속성 중 submit 사용 </br>

**form 태그 속성 :**

- action : 입력 값을 전송할 서버의 url
- method : 클라이언트가 입력한 데이터를 어떤 식으로 전송할지 결정 (GET or POST)

GET은 서버에 요청을 보내어 응답을 받아냄; '가져오는' 성격의 요청 </br>
POST는 서버에 요청을 보내어 작업을 수행; 서버의 데이터를 추가/수정/삭제 후 응답을 받아냄; '조작하는' 성격의 요청 </br>

### 18. 서버와 클라이언트

서버는 정보를 제공하는 호스트(host) </br>
클라이언트(client; 사용자)가 요청하면 서버는 그에 대한 응답으로 정보를 제공 </br>
클라이언트의 요청에 따라 응답이 달라질 수 있음 </br>
ex. 로그인 양식은 일반적으로 세 개의 입력 요소로 구성되며 각각 form을 통해 서버로 전송 </br>

### 19. meta

meta 태그는 HTML 문서에 대한 메타데이터를 정의 </br>
메타데이터란 데이터에 대한 데이터, 즉 '정보'를 의미 </br>
meta 태그는 항상 head 태그 안에 들어가며 </br>
일반적으로 문자 세트, 페이지 설명, 키워드, 문서의 작성자 및 뷰포트 설정을 지정하는 데 사용됨 </br>
meta 태그는 웹페이지에 대한 정보를 제공하므로 검색엔진과 상호작용

**meta 태그 속성 :**

- charset : 문자 세트
- http-equiv : 컨텐츠 속성 정보에 대한 http 헤더
- name : 문서 정보
- content : 메타데이터 내용

**자주 사용되는 meta 태그 유형**

- `<meta charset="utf-8">` : 한글을 표시하기 위해 문자 세트 지정하는 작업
- `<meta http-equiv="x-ua-compatible" content="IE=edge">` : 최신 버전의 IE에 맞추어 렌더링
- `<meta http-equiv="refresh" content="10">` : 10초마다 새로고침
- `<meta name="author" content="author-name">`
- `<meta name="description" content="brief-summary">`
- `<meta name="keywords" content="search-keywords">`
- `<meta name="viewport" content="device-width, inital-scale=1.0">`

UTF? Unicode Transformation Format; 가변 길이 유니코드 인코딩; 유니코드는 전 세계 모든 문자를 다루도록 설계된 표준 문자 전산 처리 방식

### 20. 뷰포트(viewport)

뷰포트(viewport)란 현재 화면에 보여지고 있는 영역을 의미 </br>
기기 별로 뷰포트가 다르기 때문에 동일한 웹페이지라도 기기에 따라 다르게 보임 </br>
기기 별 차이로 인한 배율 문제에 대응하기 위해 meta 태그를 통해 뷰포트 관련 설정 추가할 수 있음 </br>

<hr>
<hr>

### HTML Tag Reference

**Reference** : https://www.w3schools.com/tags/default.asp
|Tag |Description|
|-----------|-----------|
|`<!--  -->`|Defines a comment|
|`<!DOCTYPE>`|Defines a document type|
|`<html></html>`|Defines the root of an HTML document|
|`<head></head>`|Contains metadata/information for the document|
|`<meta>`|Defines metadata about an HTML document|
|`<link>`|Defines the relationship between a document and an external resource (most used to link to style sheets)|
|`<title></title>`|Defines a title for the document|
|`<script></script>`|Defines a client-side script|
|`<body></body>`|Defines the document's body|
|`<article></article>`|Defines an article|
|`<p></p>`|Defines a paragraph|
|`<h1></h1> to <h6></h6>`|Defines HTML headings(headlines)|
|`<hr>`|Defines a thematic change in the content; horizontal rule|
|`<br>`|Defines a single line break|
|`<b></b>`|Defines bold text|
|`<em></em>`|Defines emphasized text (<em>text</em>; italics)|
|`<mark></mark>`|Defines highlighted text (<mark>text</mark>)|
|`<img>`|Defines an image|
|`<div></div>`|Defines a block level section in a document|
|`<span></span>`|Defines an inline-block level section in a document|
|`<a></a>`|Defines a hyperlink|
|`<ul></ul>`|Defines an unordered list|
|`<ol></ol>`|Defines an ordered list|
|`<li></li>`|Defines a list item|
|`<input>`|Defines an input control|
|`<select></select>`|Defines a drop-down list|
|`<option></option>`|Defines an option in a drop-down list|
|`<textarea></textarea>`|Defines a multiline input control|
|`<form></form>`|Defines an HTML form for user input|
