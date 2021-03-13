---
description: 'BOBY : section elements'
---

# 섹션/메인 요소

### 

![ section elements](https://gblobscdn.gitbook.com/assets%2F-MB80aCzBxhQjQ8-LC7X%2F-MEwexhULwRo3EPoCGbS%2F-MEwfCAtROxyOefk200X%2Fhtmlsection.png?alt=media&token=548942c2-1b35-4429-846e-df0c4fe5b2b3)

### 1. &lt;html&gt;  root element <a id="1-root-setion-element"></a>

HTML문서에서 `<html>`요소는 문서의 **최상단 요소\(root element\)**를 나타내며 "루트 요소"라고 부른다.  모든 다른 요소들은 `<html>`요소의 자손이다.

`<head>` 요소는 해당 문서에 대한 정보인 메타 데이터\(meta data\)의 집합을 정의할 때 사용한다.

#### 1\) &lt;head&gt; element

`<head>`요소는 `<html>` 요소의 첫 번째 요소로 해당 문서에 대한 정보 메타 데이터\(meta data\)의 집합을 정의한다.

#### 2\) &lt;body&gt; element

`<body>`요소는 `<html>` 요소의 두번째 요소로 본문 영역을 표시한다. 본문 영역은 실제 콘텐츠가 표현되는 공간이 문서의 텍스트, 하이퍼링크, 이미지, 리스트 등과 같은 모든 콘텐츠 영역을 정의한다.

HTML문서에는 단 하나의 `<body>` 요소만 존재할 수 있다.

### 2. &lt;section&gt; elements <a id="2-less-than-section-greater-than-element"></a>

HTML5에서 구조를 설계할 수 `<main>,<nav>,<section>,<article>,<aside>,<header>,<footer>` 등 다양한 구조관련된 요소가 새롭게 추가되었다.

#### 1\) &lt;header&gt; element

웹 페이지 제목, 로고, 목차, 검색등을 포함하는데 `<header>`요소를 사용한다.

`<header>` 요소는 섹션 요소가 아니다. 즉, 섹션 요소 내부에 넣어도 되고 필요에 따라서 묶어 분리해서 사용해도 된다.

#### 2\) &lt;nav&gt; element

웹 페이지의 포함된 탐색 링크를 포함하는 요소이다. 

`<nav>`요소는 비순차 목록 `<ul>`요소를 사용한다.

웹 페이지 모든 링크 `<nav>`요소에 포함하는 것 아니며 주로 탐색하는 링크만을 포함한다.

나머지 링크는 하단에 위치한 `<footer>`요소만 으로도 충분하다.

#### 3\) &lt;section&gt; element <a id="1-less-than-section-greater-than-elemenet"></a>

`<section>`요소는 **내용적 흐름과 구조를 만들기 위해 내용을 나누는 용도**이다.

**소개\(introduction\), 뉴스 항목\(news item\), 연락처 정보\(contact information\)등과 같은 관련이 있는 내용을**`<section>`**요소로 묶어서 주제별로 표시한다.**

`<section>`요소는 독립적인 영역이라 `<section>`내에 `<header>`와`<footer>`요소를 둘 수 있다.

콘텐츠 포함된 독립적인 성향이 크다면 `<section>`요소 대신에 `<article>`요소를 사용하는것을 권장한다.

#### 4\) &lt;article&gt; element <a id="2-less-than-article-greater-than-element"></a>

`<article>`요소는 **본문과 별개로 구성되어 다른 영역에 영향을 주거나 받지 않고 독립적으로 배포**되거나 `재사용 할 수 있다.`

`<article>`요소는 **잡지, 신문, 논문, 보고서, 블로그 기타 소설 미디어 일 수 있다.**

`<article>`내부에 `<section>` 요소를 포함할 수 있고, 반대로 `<section>` 내부에 `<article>`를 포함할 수도 있다.

**웹 접근성이 측면에서 반드시 제목 \(h1 ~ h6\)를 포함 시켜 식별해야 한다.**

```markup
<article>
	<h2>기사 제목</h2>
		...
</article>
```

#### 5\) &lt;aside&gt; element <a id="3-less-than-aside-greater-than-element"></a>

`<aside>` 요소는 웹 사이트 사이드바에 해당 되는 부분으로 본문 내용과 직접적인 관련성이 적거나 없는 내용으로 구성된다.

#### 6\) &lt;main&gt; element <a id="4-less-than-nav-greater-than-element"></a>

`<main>`요소는 문서의 `<body>`요소 안에서 메인 콘텐츠에 해당된다.

`<main>`요소는 보이는 요소가 2개 이상이면 안된다. 즉, 사용되지 않는 `<main>`요소는 화면에서 **감춤\(hidden\)**처리해야 한다.

`<article>, <aside>, <nav>`요소는 `<main>`요소를 자식으로 포함할 수 없다. 반대로 `<main>`요소는 섹션 요소들을 포함할 수 있다.

`<main>`요소 내부에는 `<header>,<footer>` 요소를 직접적으로 포함하지 않는다.

```markup
<main>...</main>
<main hidden>...</main>
<main hidden>...</main>
```

#### 7\) &lt;footer&gt; element

`<footer>` 요소는 일반적으로 섹션의 저자, 링크, 저작권 정보 등을 포함하는 데 사용한다.

`<footer>`요소 또한 섹션 요소가 아니며, 섹션 요소 내부에 넣어도 되고 필요에 따라서 묶어 분리해서 사용해도 된다.

#### Reference 

html element [→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/html)

head element [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/head)

body element [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/body)

header element [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/header)

section element [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/section)

nav element [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/nav)

article element [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/article)

aside element [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/aside)

main element [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/main)

footer element [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/footer)



















