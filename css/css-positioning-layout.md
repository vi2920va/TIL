# CSS positioning layout

### 1. POSITIONING LAYOUT

포지셔닝\(positioning\)은 웹 브라우저가 렌더링 하는 기본 레이아웃 흐름\(normal layout flow\)을 재정의하여 흥미로운 효과를 만들어 낼 때 사용한다. 예를 들면 기본 레이아웃 흐름에서 레이아웃 내부 일부 요소의 위치를 조정하려면 position 속성을 사용하여 조정할 수 있다.

페이지의 다른 부분 위에 떠있는 [UI](https://namu.wiki/w/UI) 요소를 만들고 싶거나, 페이지의 스크롤과 상관없이 항상 브라우저 창의 동일한 위치에 자리한 UI 요소를 만들고자 한다면 position 속성을 이용한다.

#### 1\) positioning layout type

* **static postion** - 기본값\(default\), 정적 위치
* **relative position**  - 상대 위치
* **absolute position** - 절대 위치
* **fixed position** - 고정된 위치
* **sticky position** - 달라붙는 위치, IE 브라우저 미지원

#### 2\) static position

static는 기본값으로 문서 흐름에 따라 순서대로 위치를 지정한다. 이 값은 요소가 가지고 있는 기본값으로 위치를 지정하지 않을 때와 같다. 즉,  자기가 원래 위치해야 하는 그 곳에 위치해야 한다. `position` 속성 값이 `static`일 경우에 **offset** 값을 무시한다.

#### 3\) relative position

relative는 내가 가지고 있는 일반 흐름의 위치에서 상대적으로 이동하며 기본 흐름을 유지한다. 즉, 자기가 원래 위치해야 하는 위치를 기준으로 상대적인 **offset** 거리만큼 이동한다.

#### 4\) absoulte position 

👉 상위 요소가 없다면 `html` 또는 `body`기준으로 설정되는데 브라우저 마다 다르다.

해당 요소의 첫 번째 부모 요소 위치\(`position: static` 제외\)에 따라 결정된다. 이 요소 박스는 문서의 흐름에서 완전히 벗어나기 때문에 요소가 일반적인 문서의 흐름에서 차지하던 공간은 그 요소가 가지고 있던 위치는 없는 것 처럼 사라져 버린다. 그리고 기존 요소가 있어야 할 위치와 상관없이 위치를 지정할 수 있기 때문에 **절대 위치** 라고 한다.

#### 🖐 **float VS absolute**

`float`의 경우에는 설정된 요소 보다 마크업 순서상 먼저 작성된 요소들에게는 영향을 끼치지 않고, 오직 `float` 이 적용된 요소보다 나중에 작성된 요소들에게만 영향을 끼치게 된다. 반면에 `absolute`가 적용된 요소는 마크업 순서상 먼저 작성되었던, 나중에 작성 되었던 상관 없이 모두 영향을 받게 된다.

#### 5\) fixed position

`fixed`는 부모 요소와 관계 없이 브라우저 화면\(viewport\)를 기준으로 위치를 고정한다. 즉, `fixed`가 적용된 요소는 뷰포트에 상대적으로 위치가 지정되는데 이는 페이지가 스크롤 되더라도 같은 곳에 위치한다는 의미이다. 그리고 상위\(부모\) 요소를 찾지 않는다.

#### 6\) **sticky position**

 `position` 값을 `sticky`로 설정할 경우 `relative`처럼 동작하면서 `relative` 요소가 없는 경우에는 `fixed` 처럼 동작하는 두가지 효과를 모두 가질 수 있다. 수익 목적의 광고를 노출하는 경우에 많이 쓰인다. 

#### Reference

css position [→\(SITE\)](https://poiemaweb.com/css3-position)

sticky positioning [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/CSS/position#sticky_positioning)

position sticky [→\(CSS-TRICKS\)](https://css-tricks.com/position-sticky-2/)





