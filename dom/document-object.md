# Document Object

### 1. Document Object

* Document 객체는 웹 페이지 그 자체를 의미.
* 웹 페이지에 존재하는 HTML 요소에 접근하고자 할때는 Document 객체부터 시작해야 한다.
* Document 객체는 HTML 요소와 관련된 작업을 도와주는 다양한 메서드를 제공한다.

### 2. HTML 요소 선택

문서 객체\(Document Objects\)를 선택하는 방법은 다양한 메서드가 있다.

#### 1\) 하나의 요소 선택

하나의 요소를 선택하고, 첫 번째 요소만 반환한다.

```javascript
document.getElementById(id) 
document.querySelector(cssSelector)
```

#### 2\) 여러 개의 요소 선택

#### HTML Collection <a id="2-2-1-htmlcollection-&#xC815;&#xC758;"></a>

HTML 요소 또는 클래스 이름\(class name\)으로 선택할 경우, **HTML Collection**을 반환한다. 이것은 HTML요소 리스트로 담아 반환하기 위한 객체로 배열과 비슷한 사용법을 가지고 있다. 다른 단어로는 **유사배열\(array-like-object\)** 이라고 부른다. 또한 HTML Collection은 실시간으로 Node의 상태를 변경한다.

#### Node List <a id="2-2-2-nodelist-&#xC815;&#xC758;"></a>

지정된 CSS 선택자를 사용하여 요소를 모두 선택할 경우 **Node List**를 반환한다. Node List는 유사 배열이다. 하지만 HTML Collection과 달리 라이브 상태가 아니다.

```javascript
document.getElementsByTagName(tagName)
document.getElementsByClassName(class)
document.querySelectorAll(selector)
```

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

### 3. HTML 요소의 생성

새로운 HTML 요소를 생성하기 위해 제공되는 메서드.

#### 1\) document.createElement\(HTML Element\)

HTML 문서에서 지정한 요소 이름 HTML 요소를 만들어 반환한다. 요소 이름을 인식할 수 없으면 **`HTMLUnknownElement`** 를 대신 반환한다.

#### 2\) document.write\(text\)

웹 브라우저에 텍스트를 출력하는 명령어.  

📌 **주의**  
**`document.write()`** 는 로딩 시 HTML 문서 해석을 지연 또는 차단 시키니 사용하지 않는 것이 좋다.

