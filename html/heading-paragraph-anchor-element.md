# BOBY : Heading, Paragraph, Anchor

### HTML Headings element 정의

`<h1>`~ `<h6>` 레벨 요소는 HTML 문서에 제목\(heading\)을 정의할 때 사용한다.  제목의 레벨 숫자가 높아질 수록 중요성 떨어진다.

```markup
<h1>This is heading 1</h1>
<h2>This is heading 2</h2>
<h3>This is heading 3</h3>
<h4>This is heading 4</h4>
<h5>This is heading 5</h5>
<h6>This is heading 6</h6> 
```

### HTML Paragraph element 정의

HTML 문서에서 문자의 단락을 표현하기 `<p>` 요소를 사용한다. 새로운 문장을 작성 할 경우 `<p>` 요소를 새로 선언해야 한다.

```markup
<p> This is normal text - <b> and this is p text. </b> </p>
```

### HTML Anchor element 정의

페이지 내 링크 이동 또는 다른 페이지로 이동하기 위해서는 `<a>`요소를 사용하여 `<a>`요소 내부에 `href` 속성을 사용하여 주소를 설정한다.

```markup
<a href="www.naver.com">naver</a>
```

#### 1\) 웹 페이지에서 URL 입력하는 방법

① 절대 경로\(absolute path\) - 현재 HTML 문서와 상관없이 URL를 사용해 리소스를 찾는다.

② 상대 경로\(relative path\) - 현재 HTML 문서에서 상대적인 위치를 설정한다.

③ 루트 경로\(root-relative path\) - 현재 HTML 문서가 존재하는 최상위 루트 경로에서 대상을 찾는다.

```markup
<a href="https://example.com">absolute path</a>
<a href="../image/file">relative path</a>
<a href="/(루트), ../(상단 폴더)"> root path</a>
```

#### Reference

h1 ~ h6 elements [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements)

p element [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/p)

a element [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a)







