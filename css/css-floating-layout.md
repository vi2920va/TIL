# CSS floating layout

### 1. NORMAL LAYOUT FLOW

CSS가 미반영된 **일반적인 레이아웃 흐름\(normal layout flow\)**은 HTML이 기본적으로 화면에 렌더링 하는 것을 말한다.  마크업 순서대러 위에서 부터 아래 방향으로 나열된다.

💻일반적인 레이아웃 흐름 [→\(CODEPEN\)](https://codepen.io/vi2920va/full/mdrQZXm)

### 1. FLOATING LAYOUT

CSS `float` 속성은  국내 실무 내에서 레이아웃을 설계하는 과정에서 많이 사용되는 속성이다. 복잡한 형태의 레이아웃을 구성하는데 필요한 핵심 속성으로 특정 요소를 떠있게, 흐르도록, 부유하는게 하도록 하는 속성이다. 즉, `float` **속성을 사용해 박스를 왼쪽\(left\) 또는 오른쪽\(right\)으로 "부유"시키는 레이아웃 기법**이다. 여기서 "부유하다"라는 의미는 요소가 기본적인 문서 배치의 흐름에서 벗어나 요소의 모서리가 페이지의 왼쪽 또는 오른쪽으로 이동하는 것을 말한다. 

💻플로팅 레이아웃 흐름 [→\(CODEPEN\)](https://codepen.io/vi2920va/full/PoGxraO)

#### 1\) float property value

✋`float` 속성을 사용할 요소는`position`속성의 `absoulte` 값과 양립할 수 없다.

* `none` - 기본값\(default\)으로 요소를 띄우지 않게 설정.
* `left` - 요소를 왼쪽 방향으로 부유하게 설정.
* `right` - 요소를 오른쪽 방향으로 부유하게 설정.

#### 2\) float property 를 사용할 경우 특징

플로팅된 요소는 그 요소의 종류에 상관없이 블럭 박스가 된다. 예를 들어 인라인 요소인 링크\(anchor\)를 플로팅 시키는 경우에는 이 요소의 특성은 블럭 박스를 변경되고 마치 div 요소 인 것 처럼 동작하게 된다. 즉, 플로팅 된 요소는 `display: inline-block;`을 선언한 것과 동일해지기 때문에 따로 선언해줄 필요는 없다.

### 3. FLOATING CLEAR

✋**clearfix** 방법은 무조건이라기 보다 필요에 의해서 사용되는 것이다.

플로팅한 요소는 문서의 흐름상에서 벗어난 상태이기 때문에 레이아웃을 무너뜨리게 되는 현상을 접하게 된다. 이는 `float` 속성을 사용하면 발생되는 현상이며 이러한 문제를 해결하기 위해서는 `float`를 해제 해주어야한다. 여기서 말하는 "**`float`을 해제한다**"는 의미는 `float`이 적용된 요소를 해제하는 것이 아니라 clear 속성을 적용해 float 의 영향을 받지 않도록 한다는 의미이다. 

`float`를 해제하는 방법 중에 관용적인 이름으로는 **clearfix**라는 방법이 존재한다. 물론 `clear`속성을 적용하기 보다 다른 방법으로 플롯을 해제할 수 있으나 `float`을 사용해 레이아웃을 잡다보면 `clear` 가 필요해지기 때문에 가급적으로 플롯된 요소는 부모 요소에 clearfix 방법을 적용하는 것을 권장하고 있다. 즉, float이 적용된 자식 요소를 부모 요소가 감싸 안지 못하는 현상을 해결하기 위해서는 대략적으로 6가지 방법이 있는데 그 중 대표적으로 많이 사용되는 방법이 clearfix이다. 

#### 1\) 👍 ::after 

`float` 속성을 적용한 요소의 부모 요소에 가상 요소 `::after`를 사용해서 `float`를 해제하는 방법.

```css
 .clearfix::after{
   content: '';
   display: block;
   clear: both;
 }
```

#### 2\) overflow: hidden;

🖐`overflow: hidden;` 인해 보여주고자 하는 콘텐츠를 보여줄 수 없게 되기 때문에 권장되지 않는 방법.

`overflow: hidden;`속성을 이용해 `float`를 해제하는 방식은 부모 요소에 적용해야 하며, 이 속성의 특징은 자식 요소가 부모 요소 박스보다 클 경우에 자식 요소 박스의 콘텐츠를 숨기고 보여주지 않게 하는 속성이다. overflow 속성은 넘치는 것을 숨겨주는 속성인데 여기에서는 넘치는 콘텐츠를 숨긴다는 의미는 부모 요소 박스가 그 자식 요소 콘텐츠를 숨긴다는 의미이다.

#### 3\) empty elemenet - clear

🖐 이 방법은 불필요한 의미 없는 빈 요소를 이용하는 것이 때문에 가장 권장되지 않는 방법.

이 방식은 과거에 널리 사용되던 방식으로 `float` 된 요소의 **마지막 요소로 빈 요소\(empty element\)**를 작성하여 `clear` 속성을 적용하는 방법.

```markup
<div class="box-group">
  <div class="box is-blue"></div>
  <div class="box is-yellow"></div>
  <div class="box is-green"></div>
  <div class="clear"></div>
</div>
```

#### 4\) float

float 속성을 가진 자식 요소의 부모 요소에 똑같이 float를 적용해주는 방법으로 반응형 웹에 적합하지 않으므로 권장되지 않는 방법.



