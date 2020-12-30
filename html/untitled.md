# HTML 소개

### HTML 정의

HTML\(Hyper Text Markup Language\)은 HyperText\(웹 페이지에서 다른 페이지로 이동할 수 있도록 하는 것\) 기능을 가진 문서를 만드는 언어이다. 즉, 구조를 설계할 때 언어로 hyper link  시스템을 가지고 있으며, 흔히 말해서 웹 페이지를 위한 "마크업 언어"라고 한다.

### HTML 용어

![HTML &#xC6A9;&#xC5B4;](../.gitbook/assets/grumpy-cat-small.png)

| term | description |
| :--- | :--- |
| Element | HTML 요소는 시작 태그와 종료 태그 그리고 태그 사이에 위치한 콘텐츠로 구성된다. |
| Empty Element | 콘텐츠를 가질 수 없는 빈 요소로 대표적인 요소로는 `<br>`,`<hr>`,`<img>` 요소들이 있다. |
| Attribute | 속성은 요소의 성질 또는 특징을 정의하는 명세이다.  |
| Comments | 주석은 주로 개발자에게 코드를 설명하기 위해 사용되며 브라우저는 주석을 화면에 표시하지 않는다. |

### HTML 기본 구조

HTML 문서는 기본적으 **HEAD영역**과 **BODY영역**으로  구분된다.

```markup
<!DOCTYPE html>
<html>
<head>
	<title>Document</title>
</head>
<body>
	<h1>This is heading 1</h1>
	<h2>This is heading 2</h2>
	<h3>This is heading 3</h3>
	<h4>This is heading 4</h4>
	<h5>This is heading 5</h5>
	<h6>This is heading 6</h6>
</body>
</html>
```

#### 1\) &lt;!DOCTYPE&gt; 선언

DOCTYPE은 HTML 문서에서 &lt;html&gt; 요소를 정의 하기 전에 가장 먼저 선언 되어야 한다. DOCTYPE은 HTML 요소는 아니지만 선언된 페이지의 HTML 버전을 웹 브라우저에게 알려주는 역할로 대/소문자를 구분하지 않는다.

#### 2\) HEAD Element

해당 문서에 대한 정보인 메타데이터\(metadata\)집합을 정의할 때 사용한다. 

다음과 같은 요소들은 `<head>` 요소에 포함 되어야 한다.

* `<title>`, `<style>`,`<base>`,`<link>`, `<meta>`, `<script>`, `<noscript>`
* `<script>`,`<noscript>` 요소는 `<head>` 뿐만 아니라 `<body>` 요소에 포함 시킬 수 있다.

#### 3\) BODY Element

&lt;body&gt;요소는 해당 HTML 문서에 텍스트, 이미지, 리스트 등과 같은 모든 콘텐츠 포함하는 영역을 정의할 때 사용한다.

HTML 문서에는 단 하나의 `<body>`요소만 존재할 수 있다.

#### Reference

Getting started with HTML [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started)

### 











