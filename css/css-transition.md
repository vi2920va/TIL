# CSS transition

### 1. TRANSITION

CSS3에서 추가된 `transition`속성은 지정할 속성에 변화나 움직임 등을 주고 싶을 경우에 일정 시간 간격을 두고 그 속성에 변화 또는 움직임을 부드럽게 해주는 기능.

#### 1\) transition property method

`transition`에 제공되는 메서드\(method\)는 아래와 같다.

* `transition-property`
* `transition-duration`
* `transition-timing-function`
* `transition-delay`
* `transition`

#### 2\) transition-property\(\)

`transition-property` 속성은 요소에 어떤 속성을 `transition`효과로 나타낼 지를 결정하는 속성.

#### 3\) transition-duration\(\)

`transition-duration` 속성은 화면 전환이 종료되기 까지 걸리는 시간을 지정하는 속성으로 시간에 적용될 값은 **ms\(밀리초, 1/1000\)** 또는 **s\(초\)** 단위를 사용한다. 기본 설정 값은 0 이기 때문에 이동 효과를 구현하려면 **반드시** `transition-duration` **속성 값을 부여해야 한다.**

💻transition\(transition-property, transition-duration\) [→\(CODEPEN\)](https://codepen.io/vi2920va/full/xxEBJzm)

#### 4\) transition-timing-function\(\)

화면이 전환이 일어나는 시간 동안 어떤 식으로 가속을 하고 감속을 하는지 나타내는 속성으로 아래의 값들로 화면 이동 기간이 어느 정도의 빠르기로 화면 이동 효과를 이뤄질 것인지를 설정하고 애니메이션 속도를 조정할 수 있다.

* `linear` : 등속도, 전환 과정에 속도의 변화 없이, 처음부터 끝까지 일정하게 유지
* `ease` : 점전적인 기술, 기본값은 `ease` 로서 느리게 시작한 후 빠르게 가속되다가 다시 느리게 끝난다.
* `ease-in` : 가속, 애니메이션이 느리게 시작된 후 빠름 흐름으로 끝난다.
* `ease-out` : 감속, 애니메이션 빠르게 시작된 후 느리게 끝난다.
* `ease-in-out` : 점진적인 가속 후에 감속, 느리게 시작한 후 중간 지점에서 빨라지다가 다시 느려지면서 `ease`와 비슷하지만 그 변화 정도가 `ease` 처럼 급격하지는 않다.

💻 transition\(transition-timing-function\(\)\) →[\(CODEPEN\)](https://codepen.io/vi2920va/full/oNzVPbX)

#### 5\) transition-delay\(\)

 화면 이동\(전환\) 효과의 마지막 속성은 전환이 일어나는 시점을 설정할 수 있게 해주는`transition-delay` 속성으로 `transition-duration` 속성 처럼  ms\(밀리초\)/s\(초\) 단위로 설정한다. 기본값은 0 으로서 이벤트가 발생하는 즉시 전환 효과가 일어나며  시간 값에 양수를 입력하면 해당 시간이 경과한 후에 전환 효과가 일어나게 된다.

#### 6\) transition\(\)

`transition`메서드는 모든 `transition` 속성을 이용한 스타일을 한 줄에 설정한다. 위에 적어놓은 것 처럼 `transition-duration` 속성은 필수 값으로 사용해야 한다.

👉 주의해야 될 점은 시간 관련 속성으 `transition-duration, transition-delay` 2개 가 있는데이 중 하나의 값만 선언하면 `transition-duration` 값으로 간주되고`transition-delay`는 기본 값 또는 상속 받은 값을 그대로 사용하는 것으로 간주된다. 즉, **두 개의 속성 중에서** `transition-duration` **속성을 먼저 명시해야 된다.** 이에 대한 순서를 지킨다면 나머지는 키워드의 순서는 원하는대로 설정할 수 있다.



#### Reference

Using CSS transitions [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Transitions/Using_CSS_transitions)

 Easing Functions Cheat Sheet [→\(SITE\)](https://easings.net/)

####   



