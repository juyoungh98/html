# 입문자를 위한 HTML 기초 강의

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

HTML 파일의 확장자는 html 또는 htm
파일을 수정하고 싶다면 텍스트 편집기로 (notepad, Brackets, VSCode, etc.)
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
ex. <태그>컨텐츠</태그>

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

- `<!DOCTYPE html>` : 문서의 첫 부분에서 문서 유형을 지정하는 단일태그
- `<html></html>` : 문서 유형 지정 후 실제 문서가 시작되고 끝나는 지점을 나타내는 태그
- `<head></head>` : 웹 브라우저 화면에는 보이지 않지만 웹 브라우저가 알아야 할 정보를 포함; </br>
  `<meta charset='UTF-8'>`은 문자 인코딩 및 문서 키워드 등에 대한 요약 정보를 기입하는 단일 태그
- `<body></body>` : 웹 브라우저 화면에 표시될 내용이 입력되는 태그; </br>
  텍스트, 이미지, 사용자 인터페이스 태그 등을 포함하여 다양하게 구성할 수 있음

### 6. HTML 텍스트 태그

- 문단: `<p></p>`; 문단 요소를 나타내는 태그로 가장 많이 사용되는 텍스트 태그; </br>
  하나의 p 태그는 하나의 문단을 표현하며, 문단과 문단 사이에는 공백이 있음
- 제목: `<headline></headline>`; 제목(표제) 요소를 나타내는 태그로 h1 ~ h6까지 있음
- 수평선: `<hr>`; 수평선을 표시하는 태그로 주제 변경 또는 내용 구분을 위해 사용됨

### 7. HTML 텍스트의 특징

일반적으로 Enter키는 줄바꿈을 의미하나 HTML 코드에서는 이를 무시하며 공백도 한번만 인정됨 </br>
HTML에서는 `</br>` 태그가 줄바꿈을, `&nbsp;`가 공백을 표현

### 8. 태그의 구분

태그 구분 : 개발자 도구 활용

- 블록 레벨 요소 : 자기가 속한 영역의 너비를 모두 차지하여 블록 형성
- 인라인 레벨 요소 : 자기에게 필요한 만큼의 공간만 차지

<hr>
<hr>

### HTML Tag Reference

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
|`<em></em>`|Defines emphasized text (<em>text</em>; italics)|
|`<mark></mark>`|Defines highlighted text (<mark>text</mark>)59|
|`<meta>`|Defines metadata about an HTML document|
|`<head></head>`|Contains metadata/information for the document|
|`<html></html>`|Defines the root of an HTML document|
|`<title></title>`|Defines a title for the document
