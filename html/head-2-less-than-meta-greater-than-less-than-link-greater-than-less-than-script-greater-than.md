# &lt;head&gt; \(2\) - &lt;meta&gt;, &lt;link&gt;, &lt;script&gt;

### `<meta>` Element 

 이 요소는 해당 문서에 대한 정보인 메타데이터\(meta data\)를 정의할 때 사용한다.

`<mata>` 요소는 `<base>`, `<link>`, `<script>`, `<style>`, `<title>` 요소와 같은 다른 메타데이터 관련 요소들이 나타낼 수 없는 다양한 종류의 메타데이터를 제공할 때 사용된다.

제공된 정보는 브라우저 검색 엔진, 다른 웹 서비스에서 사용한다.

`name`, `http-equiv` 둘 중 하나의 속성이 명시 되었다면 반드시 `content` 속성도 함께 명시 되어야 한다.

반대로 두 속성이 명시 되었지 않았다면 `content` 속성 또한 명시 할 수 없다.

```markup
<!-- 검색 엔진을 위한 키워드 -->
<meta name="keyword" content="HTML, meta, element">

<!-- 웹 페이지 대한 설명 -->
<meta name="description" content="HTML meta element part">

<!-- 문서의 저자 -->
<meta name="author" content="peridot2029">

<!-- 5초 뒤에 다른 페이지 리다이렉트 -->
<meta http-equiv="refresh" content="5;url=https://github.com/peridot2029">

<!-- 모든 장치에서 웹 사이트가 잘 보이도록 뷰포트 설정 -->
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

###  `<link>` Element 

이 요소는 해당 문서와 외부 소스\(external resource\) 사이의 관계를 정의할 때 사용한다.

`<link>` 요소는 빈 요소 이며, 속성만을 포함시킨다.

이 요소는 `<head>` 요소 내부에만 위치할 수 있으며, 그 개수는 제한이 없다.

주로 외부 스타일 시트\(external style sheet\)를 연결할 때 사용한다.

#### 1\)  `<link>` Attribute

| attribute | description |
| :--- | :--- |
| `crossorigin` | 해당 요소가 CORS 요청을 처리하는 방식을 명시 |
| `href` | 링크될 외부 리소스\(external resource\)의 URL을 명시 |
| `hreflang` | 링크된 문서의 언어를 명시 |
| `media` | 링크된 문서를 표시할 미디어 장치를 명시 |
| `sizes` | 시각적 미디어에서 리소스 포함된 아이콘의 크기를 명시   단, `<link>` 요소의 `rel` 속성 값이 **icon**인 경우에만 사용 가능 |
| `type` | 링크된 외부 리소스의 미디어 타입을 명시 |

#### 2\) `<link>` rel Attribute

`<link>` 요소에서 `rel` 속성은 현재 문서와 외부 리소스 사이의 관계를 명시한다.

`rel` 속성은 `<link>` 요소에 반드시 명시 되어야 하는 **필수 속성**이다.

| value | description |
| :--- | :--- |
| `alternate` | 프린트 페이지, 번역된 페이지와 같이 해당 문서의 대체 버전에 대한 링크를 제공 |
| `author` | 현재 문서의 저자에 대한 링크 제공 |
| `dns-prefetch` | 브라우저가 대상 리소스 원본에 대해 DNS 확인 작업을 미리 수행하도록 명시 |
| `help` | 도움말 문서에 대한 링크 제공 |
| `icon` | 해당 문서의 아이콘을 불러온다 |
| `license` | 해당 문서의 저작권 정보에 대한 링크 제공 |
| `next` | 연관된 문서들의 모음 중 다음 문서에 대한 링크를 제공 |
| `pingback` | 현재 문서에 대한 핑백\(pingback\)을 처리하는 핑백 서버의 주소를 제공 |
| `preconnect` | 브라우저가 대상 리소스의 원본에 미리 연결하도록 명시 |
| `prefetch` | 사용자가 요청할 가능성이 있으므로, 브라우저가 대상 리소스를 미리 가져와 캐시\(cache\) 하도록 명시 |
| `preload` | 브라우저가 **as** 속성과 해당 대상과 관련된 우선 순위에 따라 현재 탐색에 사용할 리소를 미리 가져와 캐시 하도록 명시 |
| `prev` | 연관된 문서들의 모음 중 이전 문서에 대한 링크 제공 |
| `search` | 현재 문서 및 관련된 페이지를 검색 하는데 사용할 리소스에 대한 링크 제공 |
| `stylesheet` | 스타일 시트로 사용할 외부 리소스를 불러온다. |

### `<script>` Element

이 요소는 자바스크립트와 같은 클라이언트 사이드 스크립트\(client side scripts\)를 정의할 때 사용한다.

### `<noscript>` Element

이 요소는 클라이언트 사이드 스크립트\(client-side scripts\)를 사용하지 않도록 설정했거나, 스크립트를 지원하지 않는 브라우저를 위한 별도의 콘텐츠를 정의할 때 사용한다.

#### Reference

head element[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/head)

meta element[ ](https://developer.mozilla.org/ko/docs/Web/HTML/Element/head)[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/meta)

link element[ ](https://developer.mozilla.org/ko/docs/Web/HTML/Element/head)[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/link)

Document Metadata[ →HTML 5.2 표준 기술 사양﻿](https://html.spec.whatwg.org/multipage/semantics.html)

