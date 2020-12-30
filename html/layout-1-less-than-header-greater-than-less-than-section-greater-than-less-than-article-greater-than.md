# LAYOUT \(1\) - &lt;header&gt;, &lt;section&gt;, &lt;article&gt;

### HTML LAYOUT 정의

레이아웃\(layout\)은 특정 공간 안에 문자, 이미지, 등의 구성 요소를 보기 쉽게 효과적으로 배치하는 작업을 한다.

HTML에서는 다음과 같은 방법으로 레이아웃을 작성할 수 있다.

* `<div>` 요소를 이용한 레이아웃
* HTML5 의미 요소를 이용한 레이아웃
* `<table>` 요소를 이용한 레이아웃

#### 1\) `<div>`요소를 이용한 레이아웃

아래의 예시 코드는 예전에는 자주 사용되었지만, 지금은 HTML5 의미 요소를 이용한 레이아웃 추천한다.

```markup
<div id="header">Header</div>
<div id="nav">Nav</div>
<div id="section">
  Section
  <div id="article">Article</div>
</div>
<div id="aside">Aside</div>
<div id="footer">Footer</div>
```

#### 2\) HTML5 의미 요소를 이용한 레이아웃

HTML5 에서는 웹 페이지 레이아웃만을 위한 별도의 새로운 요소들을 제공한다. 이러한 요소들의 의미\(semantic\)요소라고 한다.

의미 요소는 기능은 없지만 의미를 명확하게 하여 컴퓨터가 정보를 이해하고, 논리적인 추론까지 할 수 있는 구조를 만들기 위해 추가된 요소이다. 검색 엔진 최적화\(SEO\)를 할 시에 중요한 역할을 한다.



