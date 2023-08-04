# 입문자를 위한 HTML 기초 강의

## 섹션 0

### HTML이란?

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

### HTML 문서 만들기

HTML 파일의 확장자는 html 또는 htm
파일을 수정하고 싶다면 텍스트 편집기로 (notepad, Brackets, VSCode, etc.)
결과를 확인하고 싶다면 웹브라우저로 (Chrome, Firefox, Safari, etc.)

### 개발자 도구

웹사이트 개발용 도구로, 대부분 최신 브라우저에는 개발자 도구가 탑재되어 있다. HTML, CSS 코드 확인, 모바일 모니터링, 네트워크 상태 점검, 스크립트 명령어 확인 등 다양한 기능을 통해 개발자에게 편의 제공

- Elements
- Console
- Sources
- Network

### 코드 에디터

개발자가 프로그램 소스 코드를 편집하기 위해 사용하는 소프트웨어; 코드는 텍스트이며 빠르고 편하게 코드(텍스트)를 작성하기 위해 코드 에디터를 사용; 자동 완성, 하이라이트 등의 기능이 있음

## 섹션 1

### HTML 태그 사용법: 시작과 끝

태그는 <>, </>를 사용해 컨텐츠의 시작과 끝 표시 </br>
각 태그는 컨텐츠를 감싸며 태그명은 컨텐츠의 성격과 의미를 나타냄 </br>
ex. <태그>컨텐츠</태그>

### HTML 태그 사용법: 단일 태그

경우에 따라 시작과 끝을 구분할 필요가 없는 태그 존재 </br>
ex. `<!DOCTYPE html>`

### HTML 태그 사용법: 속성

태그의 부가적 기능을 정의하는 것으로, 선택사항 </br>
속성은 시작 태그의 내부에 정의한다. 속성의 개수에는 제한이 없다 </br>
ex. `<link rel="stylesheet" href="">` 에서 rel, href 등

### HTML 태그 사용법: 주석

코드에 대한 메모를 남기기 위해 사용 </br>
ex. `<!--  -->`

### HTML 태그 사용법: 태그 종류

**Reference** : https://www.w3schools.com/tags/default.asp
|Tag |Description|
|-----------|-----------|
|`<!--  -->`|Defines a comment|
|`<!DOCTYPE>`|Defines a document type|
|`<a></a>`|Defines a hyperlink|
|`<abbr></abbr>`|Defines an abbreviation or an acronym|
|`<address></address>`|Defines contact information for the author/owner of a document|
|`<area>`|Defines an area inside an image map|
|`<article></article>`|Defines an article|
|`<aside></aside>`|Defines content aside from the page content|
|`<audio></audio>`|Defines embedded sound content|
|`<b></b>`|Defines bold text|
|`<base>`|Specifies the base URL/target for all relative URLs in a document|
|`<bdi></bdi>`|Isolates a part of text that might be formatted in a different direction from other text outside it|
|`<bdo></bdo>`|Overrides the current text direction|
|`<blockquote></blockquote>`|Defines a section that is quoted from another source|
|`<body></body>`|Defines the document's body|
|`<br>`|Defines a single line break|
