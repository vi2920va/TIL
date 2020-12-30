# HTML Metadata element

### &lt;meta&gt; Element

해당 문서에 대한 정보인 메타데이터\(metadata\)집합을 정의할 때 사용한다. 

`<meta>`요소는 `<base>`,`<link>`,`<script>`,`<style>`,`<title>` 요소와 같은 메타데이터 관련 요소들이 나타낼 수 없는 다양한 종류의 메다데이터를 제공할 때 사용되며, 이렇게 제공된 정보는 브라우저나 검색 엔진, 다른 웹 서비스에서 사용된다. 이러한 `<meta>`요소는 언제나`<head>`요소 내부에 위치해야 된다.

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

### 



