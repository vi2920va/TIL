# BOBY : User interaction attributes

### 1. User interaction attributes

 사용자와 상호작용\(interaction\)할 수 있도록 만들어 주는 속성.

#### 1\) hidden attribute

모든 HTML 요소들은 `hidden` 속성을 가질 수 있으며, 요소에 설정되면 요소가 아직 페이지의 현재 상태와 직적적으로 관련이 없거나 페이지 다른 부분에서 내용을 재사용하도록 선언하는데 사용한다. 브라우저는 `hidden` 속성이 설정된 요소르르 화면에 렌더링 하지 않으므로 이 속성이 정의된 요소는 화면에 감춤 처리하게 된다.

* `hidden` 속성을 처리하는 것은 브라우저 단에서는 CSS의 `display: none` 설정과 큰 차이가 없다.

#### 2\) tabindex attribute

tabindex 속성은 키보드로 탐색할 수 있도록 설정하거나, 제외 또는 순서대로 탐색할 수 있도록 설정할 수 있다. 이는 접근성 관점에서 매우 중요한 사항이다. 예를 들어 마우스를 사용할 수 없는 사용자가 키보드를 사용해서 웹 페이지를 이용할 떼 주로 "Tab key"'를 사용하게 된다.

* [기본적으로 포커스가 가능한 요소](https://allyjs.io/data-tables/focusable.html)들



