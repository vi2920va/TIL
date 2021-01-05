# LISTS : Unordered list, Ordered list,Description list

### HTML 목록 

HTML에서 여러 요소들을 일렬로 나열한 목록을 리스트\(list\)라고 한다. 

HTML 리스트는 크게 3가지로 나뉜다.

* 비순차 목록\(Unordered list\)
* 순차 목록\(Ordered List\)
* 정의 목록\(Description List\)

#### 1\) 비순차 목록\(Unordered list\)

`<ul>`요소는 순서가 없는 HTML 리스트를 정의할 때 사용한다.

`<ul>` 요소에 속하는 각 아이템은 `<li>`요소를 사용하여 나타낸다.

앞에 표시 되는 마커\(marker\)는 번호 대신 작은 점을 표현한다.

```markup
<ul>
	<li>bread</li>
	<li>cake</li>
	<li>fruit
		<ul>
			<li>apple</li>
			<li>mango</li>
			<li>melon</li>
		</ul>
	</li>
</ul>
```

#### 2\) 순차 목록\(Ordered List\)

`<ol>` 요소는 순서가 있는 HTML 리스트를 정의할 때 사용한다.

`<ol>` 요소에 속하는 각 아이템은 `<li>`요소를 사용하여 나타낸다.

앞에 표시 되는 마커\(marker\)는 숫자 또는 알파펫으로 표현한다.

```markup
<ol>
	<li>bread</li>
	<li>cake</li>
</ol>

<ol type="F" start="3">
	<li>bread</li>
	<li>cake</li>
	<li>fruit<li>
</ol>
```

#### 3\) 정의 목록\(Description List\)

`<dl>`요소는사전 처럼 용어를 설명하는 목록 HTML 리스트를 정의할 때 사용한다.

`<dl>`요소에 속하는 각 아이템은 오직 `<dt>`와 `<dd>`요소를 사용하여 나타낸다.

`<dt>` 요소는 용어의 이름과 `<dd>` 요소는 용어에 대한 설명이 들어간다.

```markup
<dl>
  <dt>coffee</dt>
  <dd>black hot drink</dd>
  <dt>milk</dt>
  <dd>White cold drink</dd>
</dl>
```

#### Reference 

ul element [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul)

ol element [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ol)

dl element [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/dl)

dt element [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/dt)

dd element [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/dd)

