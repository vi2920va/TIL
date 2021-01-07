# HEAD :  title, base, style elements

### 1. HEAD ElEMENTS

 `<head>` 요소는 해당 문서에 대한 정보인 메타 데이터\(meta data\)의 집합을 정의할 때 사용한다.

다음과 같은 요소들은 `<head>` 요소에 포함 되어야 한다.

* `<title>`, `<style>`,`<base>`,`<link>`, `<meta>`, `<script>`, `<noscript>`
* `<script>`,`<noscript>` 요소는 `<head>` 뿐만 아니라 `<body>` 요소에 포함 시킬 수 있다.

#### 1\) TITLE ELEMENT

`<title>` 요소는 해당 문서의 제목\(title\)을 정의할 때 사용한다.

`<title>` 요소는 브라우저의 제목 표시줄, 탭의 제목으로 사용되며 즐겨찾기 등록 시 해당 페이지에 대한 즐겨찾기 이름으로 사용되기도 한다.

또한 검색 엔진에 의한 검색 결과 페이지에서도 해당 페이지의 제목으로 나타난다.

모든 HTML 문서에는 `<title>` 요소가 반드시 필요하며 두 개 이상의 `<title>` 요소를 사용할 수 없다.

만약 `<title>` 요소가 존재하지 않으면, 해당 문서는 HTML 유효성 검사를 통과하지 못한다.

#### 2\) BASE ELEMENT

 `<base>` 요소는 문서의 모든 상대 주소\(relative URL\)에 대한 기본 URL\(base URL\)과 `target` 속성 값을 정의할 때 사용한다.

하나의 문서에는 단 하나의 `<base>` 요소만 존재할 수 있다.

`<base>` 요소는 반드시 `<head>` 요소 내에 위치해야 한다.

`<base>` 요소는 반드시 `href`, `target` 속성 중에서 하나 이상의 속성 값을 명시 해야 한다.

```markup
<head>
	<base href="https://github.com">
</head>
<body>
	<!-- https://github.com/vi2920va -->
	<a href="./vi2920va">GIT</a>
</body>
```

#### 3\) STYLE ELEMENT

이 요소는 HTML 문서의 스타일 정보를 정의 할 때 사용한다.

`<style>` 요소는 해당 요소가 포함된 HTML 문서 콘텐츠에 적용되는 CSS를 명시한다.

HTML 문서는 여러 개의 `<style>` 요소를 사용할 수 있다.

별도의 파일로 지정된 외부 스타일 시트는 `<link>` 요소를 사용하여 참조한다.

#### Reference

head element[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/head)

title element[ ](https://developer.mozilla.org/ko/docs/Web/HTML/Element/head)[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/title)

style element[ ](https://developer.mozilla.org/ko/docs/Web/HTML/Element/head)[→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/style)

base element[ ](https://developer.mozilla.org/ko/docs/Web/HTML/Element/head)[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/base)

Document Metadata[ →HTML 5.2 표준 기술 사양﻿](https://html.spec.whatwg.org/multipage/semantics.html)



