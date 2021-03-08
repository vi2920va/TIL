# HEAD : meta, link elements

### 1. &lt;head&gt; elements

 `<head>` 요소는 해당 문서에 대한 정보인 메타 데이터\(meta data\)의 집합을 정의할 때 사용한다.

다음과 같은 요소들은 `<head>` 요소에 포함 되어야 한다.

* `<title>`, `<style>`,`<base>`,`<link>`, `<meta>`, `<script>`, `<noscript>`
* `<script>`,`<noscript>` 요소는 `<head>` 뿐만 아니라 `<body>` 요소에 포함 시킬 수 있다.

#### 4\) &lt;meta&gt; element 

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

####  5\) &lt;link&gt; element 

이 요소는 해당 문서와 외부 소스\(external resource\) 사이의 관계를 정의할 때 사용한다.

`<link>` 요소는 빈 요소 이며, 속성만을 포함시킨다.

이 요소는 `<head>` 요소 내부에만 위치할 수 있으며, 그 개수는 제한이 없다.

주로 외부 스타일 시트\(external style sheet\)를 연결할 때 사용한다.

#### ① &lt;link&gt;  element - attributes

<table>
  <thead>
    <tr>
      <th style="text-align:left">attribute</th>
      <th style="text-align:center">attribute value</th>
      <th style="text-align:center">description</th>
      <th style="text-align:center">spec</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><code>crossorigin</code>
      </td>
      <td style="text-align:center">
        <p>anonymous</p>
        <p>use-credentials</p>
      </td>
      <td style="text-align:center">&#xD574;&#xB2F9; &#xC694;&#xC18C;&#xAC00; CORS &#xC694;&#xCCAD;&#xC744;
        &#xCC98;&#xB9AC;&#xD558;&#xB294; &#xBC29;&#xC2DD;&#xC744; &#xBA85;&#xC2DC;.</td>
      <td
      style="text-align:center">HTML5</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>href</code>
      </td>
      <td style="text-align:center">URL</td>
      <td style="text-align:center">&#xB9C1;&#xD06C;&#xB420; &#xC678;&#xBD80; &#xB9AC;&#xC18C;&#xC2A4;(external
        resource)&#xC758; URL&#xC744; &#xBA85;&#xC2DC;</td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:left"><code>hreflang</code>
      </td>
      <td style="text-align:center">&#xC5B8;&#xC5B4;&#xCF54;&#xB4DC;</td>
      <td style="text-align:center">&#xB9C1;&#xD06C;&#xB41C; &#xBB38;&#xC11C;&#xC758; &#xC5B8;&#xC5B4;&#xB97C;
        &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:left"><code>media</code>
      </td>
      <td style="text-align:center">media queries</td>
      <td style="text-align:center">&#xB9C1;&#xD06C;&#xB41C; &#xBB38;&#xC11C;&#xB97C; &#xD45C;&#xC2DC;&#xD560;
        &#xBBF8;&#xB514;&#xC5B4; &#xC7A5;&#xCE58;&#xB97C; &#xBA85;&#xC2DC;.</td>
      <td
      style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:left"><code>sizes</code>
      </td>
      <td style="text-align:center">width x hight any</td>
      <td style="text-align:center">&#xC2DC;&#xAC01;&#xC801; &#xBBF8;&#xB514;&#xC5B4;&#xC5D0;&#xC11C; &#xB9AC;&#xC18C;&#xC2A4;
        &#xD3EC;&#xD568;&#xB41C; &#xC544;&#xC774;&#xCF58;&#xC758; &#xD06C;&#xAE30;&#xB97C;
        &#xBA85;&#xC2DC;.
        <br />(<code>&lt;link&gt;</code> &#xC694;&#xC18C;&#xC758; <code>rel</code> &#xC18D;&#xC131;
        &#xAC12;&#xC774; &quot;icon&quot;&#xC778; &#xACBD;&#xC6B0;&#xC5D0;&#xB9CC;
        &#xC0AC;&#xC6A9; &#xAC00;&#xB2A5;)</td>
      <td style="text-align:center">HTML5</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>type</code>
      </td>
      <td style="text-align:center">media type</td>
      <td style="text-align:center">&#xB9C1;&#xD06C;&#xB41C; &#xC678;&#xBD80; &#xB9AC;&#xC18C;&#xC2A4;&#xC758;
        &#xBBF8;&#xB514;&#xC5B4; &#xD0C0;&#xC785;&#xC744; &#xBA85;&#xC2DC;</td>
      <td
      style="text-align:center"></td>
    </tr>
  </tbody>
</table>

#### ② &lt;link&gt; element - rel attributes

`<link>` 요소에서 `rel` 속성은 현재 문서와 외부 리소스 사이의 관계를 명시한다.

`rel` 속성은 `<link>` 요소에 반드시 명시 되어야 하는 **필수 속성**이다.

| value | description |
| :---: | :---: |
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

#### Reference

head element[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/head)

meta element[ ](https://developer.mozilla.org/ko/docs/Web/HTML/Element/head)[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/meta)

link element[ ](https://developer.mozilla.org/ko/docs/Web/HTML/Element/head)[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/link)

Document Metadata[ →HTML 5.2 표준 기술 사양﻿](https://html.spec.whatwg.org/multipage/semantics.html)

