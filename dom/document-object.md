# Document Object

## 문서 객체\(Document Object\)

* Document 객체는 웹 페이지 그 자체를 의미.
* 웹 페이지에 존재하는 HTML 요소에 접근하고자 할때는 Document 객체부터 시작해야 한다.
* Document 객체는 HTML 요소와 관련된 작업을 도와주는 다양한 메서드를 제공한다.

### 1. Document Method

Document 객체는 HTML 요소와 관련된 작업을 도와주는 다양항 메서드를 제공한다.

* HTML 요소의 선택
* HTML 요소의 생성
* HTML 이벤트 핸들러 추가
* HTML 객체의 선택

### 2. HTML 요소의 선택

#### 1\) ID로 요소 선택

모든 HTML 요소는 `ID` 속성을 가질 수 있다. ID 속성은 한 문서 안에서 유일해야 하고, 한 문서에서 두 요소의 ID가 같을 수 없다. document 객체의 `getElementByID(ID`\)메서드로 **유일성이 확보된 ID를 전달해서 특정 요소를 선택**할 수 있다.



{% tabs %}
{% tab title="HTML" %}
```markup
<h1>ID를 이용한 선택</h1>

<ul>
  <li>One</li>
  <li id="even">Two </li>
  <li>Three</li>
  <li>Four</li>
  <li>Five</li>
</ul>
```
{% endtab %}

{% tab title="JavaScript" %}
```javascript
let selectedItem = document.getElementById('even');
selectedItem.style.color = 'red';
```
{% endtab %}
{% endtabs %}

#### 2\) Name으로 요소 선택

HTML `name` 속성의 원래 목적은 `<form>` 요소에 이름을 부여하는 것으로, 폼 데이터를 서버로 전송할 때 사용한다. name 속성은 ID 속성과 같은 방식으로 요소에 이름을 부여하지만 name 속성의 값은 문서 안에서 ID 속성과 달리 유일성이 보장되지 않는다. document 객체의  `getElementsByName()` 메서드를 사용하면 **name의 속성 값을 이용해서 HTML 요소를 선택**할 수 있다.

{% tabs %}
{% tab title="HTML" %}
```markup
<h1>name 속성을 이용한 선택</h1>
<p name="first">first paragraph</p>

<ul>
  <li name="first">One</li>
  <li>Two </li>
  <li>Three</li>
  <li>Four</li>
  <li>Five</li>
</ul>
```
{% endtab %}

{% tab title="JavaScript" %}
```javascript
let selectedItem = document.getElementsByName('first');

for(let i = 0; i < selectedItem.length; i++) {
    selectedItem.item(i).style.color = 'red';
}
```
{% endtab %}
{% endtabs %}

#### 3\) Type으로 요소 선택

document 객체의 `getElementsByTagName(tagName)`메서드를 사용하면 같은 **Type\(또는 태그 이름\)의  HTML 요소를 한 번에 모두 선택**할 수 있다.  

{% tabs %}
{% tab title="HTML" %}
```markup
<h1>HTML 태그 이름을 이용한 선택</h1>

<ul>
  <li>One</li>
  <li>Two </li>
  <li>Three</li>
  <li>Four</li>
  <li>Five</li>
</ul>
```
{% endtab %}

{% tab title="JavaScript" %}
```javascript
let selectedItem = document.getElementsByTagName('li');

for (let i = 0; i < selectedItem.length; i++) {
  selectedItem.item(i).style.color = 'red';
}
```
{% endtab %}
{% endtabs %}

#### 4\) CSS Class로 요소 선택

`getElementsByClassName(className)` 메서드를 사용하면 문서 요소의 `class` 속성을 메서드 **인자로 지정한 식별자들 전부가 있는 요소를 찾는다.** 식별자의 구분은 쉼표\(,\)아닌 공백을 사용한다는 점을 주의해야한다.

{% tabs %}
{% tab title="HTML" %}
```markup
<h1>class를 이용한 선택</h1>

<ul>
  <li class="odd">One</li>
  <li>Two </li>
  <li class="odd">Three</li>
  <li>Four</li>
  <li class="odd">Five</li>
</ul>
```
{% endtab %}

{% tab title="JavaScript" %}
```javascript
let selectedItem = document.getElementsByClassName('odd'); 

for (let i = 0; i < selectedItem.length; i++) {
    selectedItem.item(i).style.color = 'red';
}
```
{% endtab %}
{% endtabs %}

#### 5\) CSS선택자로 요소 선택

CSS 스타일시트 문서 내부의 요소나 요소 집합을 선택할 때 사용되는 선택자\(selector\)는 `ID`와 `name` 속성, `HTML 요소`와 `class` 이름을 이용해서 요소를 선택할 수 있다. document 객체의 `querySelectorAll()` 메서드는 CSS 선택자 문자열을 인자로 받아서, 이 선택자와 일치하는 문서 내 모든 요소를 NodeList로 객체로 반환한다. NodeList는 메서드를 호출한 순간 선택자와 일치하는 요소를 그대로 가져오기는 하지만, 그 후에 일어나는 문서 내 변화를 반영하지는 않는다.

{% tabs %}
{% tab title="HTML" %}
```markup
<h1>CSS 선택자 이용한 선택</h1>
<p class="odd">first paragraph</p>

<ul>
  <li class="odd">One</li>
  <li>Two </li>
  <li class="odd">Three</li>
  <li>Four</li>
  <li class="odd">Five</li>
</ul>
```
{% endtab %}

{% tab title="JavaScript" %}
```javascript
let selectedItem = document.querySelectorAll('li.odd'); 

for (let i = 0; i < selectedItem.length; i++) {
    selectedItem.item(i).style.color = 'red'; 
}
```
{% endtab %}
{% endtabs %}

더불어 `querySelector()`메서드는 `querySelectorAll()` 메서드와 달리 **요소 중 문서 순서상 첫 번째 요소만 반**환한다. 일치하는 요소가 없으면 `null`을 반환한다.

{% tabs %}
{% tab title="HTML" %}
```markup
<h1>CSS 선택자 이용한 선택</h1>
<p class="odd">first paragraph</p>

<ul>
  <li class="odd">One</li>
  <li>Two </li>
  <li class="odd">Three</li>
  <li>Four</li>
  <li class="odd">Five</li>
</ul>
```
{% endtab %}

{% tab title="JavaScript" %}
```javascript
let selectedItem = document.querySelector('p.odd');
selectedItem.style.color = 'red';
```
{% endtab %}
{% endtabs %}

#### 6\) NodeList

**NodeList**는 `element.childeNode`와 같은 속성이나 `querySelectorAll()`과 같은 메서드에 의해 반환되는 **Node Collection**이다. NodeList는 마치 배열과 비슷하게 생겼지만 배열과 다르다. 이것을 배열과 같은 형태를 하고 있지만 **배열이 아닌 객체들을 '유사 배열'** 이라고 부른다.  NodeList는 배열이 아니기 때문에 배열에 사용 가능한 메서드를 대부분 사용할 수 없다. 때문에 NodeList에 배열 메서드를 사용하기 위해서는 NodeList를 실제 배열로 변환하는 등 방법을 사용해야 한다. 

대개의 경우 NodeList 라이브 콜렉션으로 DOM의 변경 사항을 실시간 반영한다. 그러나 `querySelectorAll()`**메서드에 의해 반환되는 NodeList 정적 콜렉션으로 DOM의 변경 사항이 실시간으로 반영되지 않는다.**

#### 7\) HTMLCollection

**HTMLCollection** 인터페이스는 요소의 문서 내 순서댜로 정렬된 일반 컬렉션을 나타내며 **NodeList**와 마찬가지로 유사 배열이다. HTML Collection현대적인 DOM의 이전 세대부터 존재하던 구성 요소로 `element.children`과 같은 속성 또는 `getElementsByClassName()`, `getElementsByTagName()`와 같은 메서드에 의해 반영된다. **HTMLCollection은 모두 문서가 바뀔 때 실시간으로 업데이트 되는 라이브 콜렉션**이다.

#### 

#### 

### 3. HTML 요소의 생성

#### 1\) document.createElement\(HTML element\)

HTML 문서에서 지정한 요소 이름 HTML 요소를 만들어 반환한다. 요소 이름을 인식할 수 없으면 **`HTMLUnknownElement`** 를 대신 반환한다.

#### 2\) docuemnt.write\(text\)

웹 브라우저에 텍스트를 출력하는 명령어. \(단, document.write\(\) 메서드는 로딩 시 HTML 문서 해석을 지연 또는 차단 시키니 사용하지 않는 것이 좋다.\)

### 4. HTML 이벤트 핸들러 추가



#### 3\) [matches\(IE 9+\)](https://developer.mozilla.org/en-US/docs/Web/API/Element/matches)

요소가 되었는지 확인하는 메서드.

```javascript
let result = element.matches(selectorString);
```

즉, 요소가 선택 되었는지 여부를 확인할 수 있고 반환 값을 논리 값이기 때문에 조건문에 사용할 수 있다.

```javascript
let tit = document.querySelector('.title');
if(tit.matches('h1')){
	console.log('this is class h1 element true');
}else{
	console.log('this is class h1 element false');
}
```

#### Reference

Live Collection vs Static Collection  [→\(SITE\)](https://im-developer.tistory.com/110)



