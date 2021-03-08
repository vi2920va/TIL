# ATTRIBUTES : user interaction attributes

### 1. USER INTERACTION - ATTRIBUTES

 사용자와 상호작용\(interaction\)할 수 있도록 만들어 주는 속성.

#### 1\) HIDDEN - ATTRIBUTE

모든 HTML 요소들은 `hidden` 속성을 가질 수 있으며, 요소에 설정되면 요소가 아직 페이지의 현재 상태와 직적적으로 관련이 없거나 페이지 다른 부분에서 내용을 재사용하도록 선언하는데 사용한다. 브라우저는 `hidden` 속성이 설정된 요소르르 화면에 렌더링 하지 않으므로 이 속성이 정의된 요소는 화면에 감춤 처리하게 된다.

* `hidden` 속성을 처리하는 것은 브라우저 단에서는 CSS의 `display: none` 설정과 큰 차이가 없다.

#### 2\) TABINDEX - ATTRIBUTE

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
	
<!--
 	[0] 은 포커스가 없는 요소에 포커스를 가능하게 해 줄 수 있다. 
 	div 요소는 포커스를 가지지 않는 요소이지만, 포커스를 적용할 수 있게 된다. 
 	컴포넌트 제작 시, 비 포커스 요소에 포커스를 적용해야 할 경우 유용하게 사용된다
-->
<div tabindex="0"></div>

<!-- 
	[-1] 일반적인 포커스 순서에서 제외시킬 수 있다. 
	(JavaScript 프로그래밍으로 포커스 처리 가능) 
	컴포넌트의 일부 요소를 일시적으로 포커스 순서에서 제외한 후, 
	목표에 따라 포커스를 다시 활성화 처리할 수 있다. 
	즉, 의도적으로 포커스를 가지지 못하게 만들어 놨다가 
	포커스를 주게끔 할 때 유용하게 사용할 수 있다. 
-->
<ol class="toc">
	<li><a href="#pinch">위기</a></li>
	<li><a href="#overcome" tabindex="-1">극복</a></li>
</ol>

```

#### 3\) ACCSSKEY - ATTRIBUTE

accskey속성을 사용하면 단축키를 통해서 액션을 연결 시킬 수 있다. 즉 , 단축키를 지정해주는 것이다. 모든  HTML 요소는 accsskey 속성을 가질 수 있으며, 속성 값은 키보드 단축키로 설정된다. 하지만 accsskey 속성의 단축키는 브라우저와 운영체제 플랫폼에 의존하고 있어 운영체제마다 사용자 경험이 달라진다. 쉽게 말해서 windows  사용자와 Mac OSX 사용자가 사용자가 사용하는 단축키는 달라진다. 

#### 브라우저 X 운영체제 플랫폼

```bash
# Windows
	Chrome : Alt + 단축키 
	IE 		 : Alt + 단축키 
	Safari : Alt + 단축키 
	Opera  : Alt + 단축키 
	Firefox: Alt + Shift + 단축키

# Mac OSX
	Chrome : Control + Alt + 단축키 
	Safari : Control + Alt + 단축키 
	Opera  : Control + Alt + 단축키 
	Firefox : Control + 단축키

# Linux
	Chrome : Alt + 단축키 
	Opera  : Alt + 단축키 
	Firefox: Alt + Shift + 단축키

```

#### 4\) CONTETEDITABLE - ATTRIBUTE

기본적으로 HTML 요소들은 편집이 불가능 하지만 contenteditable 속성이 설정된 요소는 사용자가 직접 편집할 수 있도록 만들어 줄 수 있다. 값이 true 또는 빈 문자열\(""\)일 경우 편집을 허용하게 되고, 값이 fasle일 경우 편집을 허용하지 않는다. 예를 들어 사용자가 어떠한 위젯의 콘텐츠를 수정할 수 있는 권한을 주고하 할 때 내용을 수정할 수 있도록 해줄 수 있다.

#### 5\) DRAGGABLE -  ATTRIBUTE

 모든 HTML 요소는 draggable 속성을 가질 수 있다. 값이 true일 경우 드래그\(drag\) 가능하고, 값이 false 또는 빈 문자열\(""\)이면 드래그가 불가능 하다.

```markup
<p draggable="true">
  ... 
</p>
```



