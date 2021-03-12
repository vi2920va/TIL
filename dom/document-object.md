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

#### 1\) document.getElementsByTagName\(tag name\)

해당 태그의 이름을 요소를 모두 선택, HTML Collection을 반환한다.

#### 2\) document.getElementsByClassName\(class name\)

해당 클래스에 속한 요소를 모두 선택, HTML Collection을 반환한다.

#### 3\) document.getElementById\(ID\)

해당 아이디의 요소를 선택.

#### 4\) document. getElementByName\(name attribute\)

해당 name 속성값을 가지는 요소를 모두 선택.

#### 5\) document.querySelector\(selector\)

 지정된 CSS 선택자로 하나의 요소를 선택하고 해당하는 첫 번째 요소만 반환한다.

#### 6\) document.querySelectorAll\(\)

지정된 CSS 선택자를 가진 요소를 모두 선택,  Node List를 반환한다.

#### 7\) HTML Collection

getElementsByTagName\(\), getElementsByClassName\(\) 메서드를 사용하면 HTML Collection을 반환한다. HTML Collection은 유사 배열 객체\(array like object\)라고 해서 배열 비슷한 방법을 가지고 사용한다. 또한 HTML Collection은 실시간으로 노드의 상태를 변경한다.

#### 8\) Node list

querySelectorAll\(\) 메서드를 사용하면 Node list를 반환한다. Node list는 유사 배열 객체 이지만 HTML Collection과 달리 라이브가 상태가 아니므로 실시간으로 변경되지는 않는다.

### 3. HTML 요소의 생

#### 1\) document.createElement\(HTML element\)

HTML 문서에서 지정한 요소 이름 HTML 요소를 만들어 반환한다. 요소 이름을 인식할 수 없으면 **`HTMLUnknownElement`** 를 대신 반환한다.

#### 2\) docuemnt.write\(text\)

웹 브라우저에 텍스트를 출력하는 명령어. \(단, document.write\(\) 메서드는 로딩 시 HTML 문서 해석을 지연 또는 차단 시키니 사용하지 않는 것이 좋다.\)

### 4. HTML 이벤트 핸들러 추가



### 5. HTML 객체의 선택



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

### 



