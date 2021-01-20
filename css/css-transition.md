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

`transition-duration` 속성은 화면 전환이 종료되기 까지 걸리는 시간을 지정하는 속성으로 시간에 적용될 값은 **ms\(밀리초, 1/1000\)** 또는 **s\(초\)** 단위를 사용.

#### 4\) transition-timing-function\(\)

화면이 전환이 일어나는 시간 동안 어떤 식으로 가속을 하고 감속을 하는지 나타내는 속성.

* linear -  등속도, 전환 과정에 속도의 변화 없이, 처음부터 끝까지 일정하게 유지
* ease - 점전적인 기술, 기본값은 ease 로서 느리게 시작한 후 빠르게 가속되다가 다시 느리게 끝난다.
* ease-in

#### 5\) transition-delay\(\)

 화면 이동\(전환\) 효과의 마지막 속성은 전환이 일어나는 시점을 설정할 수 있게 해주는 `transition-delay` 속성.

#### 6\) transition\(\)

`transition`메서드는 모든 `transition` 속성을 이용한 스타일을 한 줄에 설정.



#### Reference

Using CSS transitions [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Transitions/Using_CSS_transitions)

 Easing Functions Cheat Sheet [→\(SITE\)](https://easings.net/)

####   



