# BOBY : User interaction attributes

### 1. User interaction attributes

 사용자와 상호작용\(interaction\)할 수 있도록 만들어 주는 속성.

#### 1\) hidden attribute

모든 HTML 요소들은 `hidden` 속성을 가질 수 있으며, 요소에 설정되면 요소가 아직 페이지의 현재 상태와 직적적으로 관련이 없거나 페이지 다른 부분에서 내용을 재사용하도록 선언하는데 사용한다. 브라우저는 `hidden` 속성이 설정된 요소르르 화면에 렌더링 하지 않으므로 이 속성이 정의된 요소는 화면에 감춤 처리하게 된다.

* `hidden` 속성을 처리하는 것은 브라우저 단에서는 CSS의 `display: none` 설정과 큰 차이가 없다.

#### 2\) tabindex attribute

tabindex 속성은 키보드로 탐색할 수 있도록 설정하거나, 제외 또는 순서대로 탐색할 수 있도록 설정할 수 있다. 이는 접근성 관점에서 매우 중요한 사항이다. 예를 들어 마우스를 사용할 수 없는 사용자가 키보드를 사용해서 웹 페이지를 이용할 떼 주로 "Tab key"'를 사용하게 된다.

* [기본적으로 포커스가 가능한 요소](https://allyjs.io/data-tables/focusable.html)[들](https://allyjs.io/data-tables/focusable.html)
  * form control elements - `<input>, <button>, <textarea>, <select>` 등
  * elements with href attributes - `<a>, <area>` 
  * elements with controls attributees - `<video>, <audion>`

```markup
<!-- 
	[양수] 탭 포커스 순서(2번째)를 설정한다. 
	(논리적 포커스 흐름에 방해가 되기에 사용을 권장하지 않는다)
 --> 
<button type="button" class="button is-play"
	tabindex="2">재생</button>
<!-- [0] 은 포커스가 없는 요소에 포커스를 가능하게 해 줄 수 있다. div 요소는 포커스를 가지지 않는 요소이지만, 포커스를 적용할 수 있게 된다. 컴포넌트 제작 시, 비 포커스 요소에 포커스를 적용해야 할 경우 유용하게 사용됨. -->
<div tabindex="0"></div>
<!-- [-1] 일반적인 포커스 순서에서 제외시킬 수 있다. (JavaScript 프로그래밍으로 포커스 처리 가능) 컴포넌트의 일부 요소를 일시적으로 포커스 순서에서 제외한 후, 목표에 따라 포커스를 다시 활성화 처리할 수 있다. 즉, 의도적으로 포커스를 가지지 못하게 만들어 놨다가 포커스를 주게끔 할 때 유용하게 사용할 수 있다. -->
<ol class="toc">
	<li><a href="#pinch">위기</a></li>
	<li><a href="#overcome" tabindex="-1">극복</a></li>
</ol>

```

