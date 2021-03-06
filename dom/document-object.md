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

HTML 요 또는 클래스 이름\(class name\)으로 선택할 경우, **`HTMLCollection`**을 반환한다. 이것은 HTML요소 트리스담아 반환하기 위한 객체로 배열과 비슷한 사용법을 가지고 있다. 다른 단어로는 **`유사배열(array-like-object)`** 이라고 부른다. 또한 HTML Collection은 실시간으로 Node의 상태를 변경한다.

#### Node List <a id="2-2-2-nodelist-&#xC815;&#xC758;"></a>



