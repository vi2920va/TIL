---
description: CSS animation
---

# 애니메이션

### 1. animation

CSS3에서 추가된 `animation`속성은 요소에 적용되는 CSS 스타일을 다른 CSS 스타일로 부드럽게 전환시켜 준다. 애니메이션은 애니메이션을 나타내는 CSS 스타일과 애니메이션의 중간 상태인 `keyframes`들로 구성된다. 또한 애니메이션은 트래지션\(transition\)보다 훨씬 더 규모가 복잡하며 다양한 능력을 가지고 있기 때문에 좀 더 정밀한 효과를 구현할 수 있다.

#### 1\) animation 장점

* JavaScript를 모르더라도 간단하게 애니메이션를 만들 수 있다.
* JavaScript를 이용한 애니메이션은 잘 만들어졌다라도 성능이 좋지 못할 때가 있다. CSS  애니메이션은 frame-skipping 같은 여러 기술을 이용하여 최대한 부드럽게 렌더링된다.
* 브라우저는 애니메이션의 성능을 효율적으로 최적화 할 수 있다. 

#### 2\) animation-\* property

`animation-*`에 제공되는 속성은 아래와 같다.

* `animation-name`
* `animation-duration`
* `animation-delay`
* `animation-direction`
* `animation-iteration-count`
* `animation-play-state`
* `animation-timing-funuction`
* `animation-fill-mode`

#### 3\) keyframes

CSS3에서 애니메이션 효과를 사용하기 위해서 우선 애니메이션 키프레임\(keyframe\)을 정의해야한다. 키프레임에는 특정한 시간에 해당 요소가 가져야 할 CSS 스타일을 명시한다. 

`@keyframes` 규칙 안에 이렇게 CSS 스타일 설정해놓으면, 해당 요소의  스타일은 특정 시간까지 현재 스타일에서 설정해 놓은 새로운 스타일로 천천히 변화하게 된다. 즉, 애니메이션이 동작하기 위해서 먼저 `animation-name` 속성을 이용하여 요소와 키프레임을 연결해 주어야 한다.

#### 4\) animation-name

`animation-name`속성은 `@keyframes`속성에서 설정한 애니메이션의 이름이다. 이름을 설정해야 애니메이션을 재생할 수 있다. 즉, 이름을 정의해야 애니메이션을 재생\(호출\)할 수 있다. 

```css
/* 유효한 애니메이션 이름 */
animation-name: name;
animation-name:_name;
animation-name:-name;

/* 유효하지 않은 애니메이션 이름 */
animation-name: 1name;
animation-name: @name;
```

#### 5\) animation-duration

`animation-duration` 속성은 애니메이션을 한 번 재생하는 데 걸리는 시간을 설정한다. 기본값은 0으로 설정되었기 때문에 아무런 움직임도 발생하지 않으며 또한 값이 음수로 설정할 경우에도 애니메이션은 재생되지 않는다.

💻 animation\(animation-name, animation-duration\) [→\(CODEPEN\)](https://codepen.io/vi2920va/full/ZEpZKXb)

#### 6\) animation-delay

`animation-delay` 속성은 애니메이션 시작을 지연할 시간을 설정하는 속성.

| property value | description |
| :--- | :--- |
| `0`\(defalut\) | 기본값으로 애니메이션을 시작한다. |
| `now` | `0`으로 설정한 값과 같이 애니메이션을 시작한다.  |
| `s/ms` | 설정한 시간이 지난 뒤에 애니메이션을 시작한다. 설정한 값이 음수가 아니라 양수이면 '-1s' 1초가 지난 뒤의 장면부터 애니메이션을 재생한다. |

#### 7\) animation-direction

`animation-direction` 속성은 애니메이션의 재생 방향을 정의하는 속성이다. `@keyframes` 속성의 `from`에서 `to`로 재생하는 것이 순방향 이고, `to`에서 `from`으로 재생하는 것이 역방향이다. 

| property value | description |
| :--- | :--- |
| `noraml`\(default\) |  애니메이션을 순방향으로 재생하고 재생이 한 번 끝나면 첫 번째 프레임부터 다시 시작한다. |
| `alternate` | 애니메이션을 순방향으로 시작해 역방향과 순방향으로 번갈아서 애니메이션을 재생한다. 홀수 번째로 재생할 때는 순방향으로 재생하고, 짝수 번째로 재생할 때는 역방향으로 재생한다. |
| `reverse` | 애니메이션을 역방향으로 재생하고 재생이 한 번 끝나면 마지막 프레임부터 다시 시작한다. |
| `alternate-reverse` | 애니메이션을 역방향으로 시작해 순방향과 역방향으로 번걸아서 애니메이션을 재생한다. 홀수 번째로 재생할 때는 역방향으로 재생하고, 짝수 번째로 재생할 때는 순방향으로 재생한다. |

💻 animation\(animation-direction\) [→\(CODEPEN\)](https://codepen.io/vi2920va/full/NWRmjeQ)

#### 8\) animation-iteration-count

`animation-iteration-count` 속성은 애니메이션을 재생하는 횟수를 정의하는 속성.

| property value | description |
| :--- | :--- |
| `1`\(default\) | 숫자\(number\)값으로 설정한 횟수만큼 애니메이션을 설정한다. 설정한 값 숫자가 소수 일 경우에 애니메이션 재생 도중에 첫 번째 프레임으로 돌아가 멈춘다. 또한 숫자가 음수일 경우에 애니메이션을 재생하지 않는다. |
| `infinite` | 애니메이션을 무한으로 반복. |

#### 9\) animation-play-state

이 속성은 애니메이션 재생 여부를 정의하는 속성.

| property value | description |
| :--- | :--- |
| `running` | 애니메이션을 재생. |
|  `paused` | 애니메이션을 정지. |

#### 10\) animation-timing-function

애니메이션의 키프레임 사이의 재생 속도를 조절하는 속성으로 재생하는 동안 단계별 속도 설정.

| property value | description |
| :--- | :--- |
| `linear` | 등속도, 전환 과정에 속도의 변화 없이, 처음부터 끝까지 일정하게 유지 |
| `ease` | 점전적인 기술, 기본값은 `ease` 로서 느리게 시작한 후 빠르게 가속되다가 다시 느리게 끝난다. |
| `ease-in` | 가속, 애니메이션이 느리게 시작된 후 빠름 흐름으로 끝난다. |
| `ease-out` | 감속, 애니메이션 빠르게 시작된 후 느리게 끝난다. |
| `ease-in-out` |  점진적인 가속 후에 감속, 느리게 시작한 후 중간 지점에서 빨라지다가 다시 느려지면서 `ease`와 비슷하지만 그 변화 정도가 `ease` 처럼 급격하지는 않다. |
| `cubic-bezier(n,n,n,n)` | 애니메이션 효과가 사용자가 정의한 `cubic-bezier` 함수에 따라 진행. |

#### 11\) @keyframes/animation

애니메이션을 재생할 각 프레임의 스타일을 정의하는 것으로 `from`또는 `0%`속성에서 출발해서 `to`또는`100%`속성에서 설정한 스타일로 점차 바뀌면서 애니메이션을 재생.

| property value | description |
| :--- | :--- |
| `0%` |  애니메이션의 시작 프레임. |
| `from` | 애니메이션의 시작 프렘임으로 0%과 같다. |
| `100%` | 애니메이션의 마지막 프레임. |
| `to` | 애니메이션의 마지막 프레임으로 100%와 같다. |

{% code title="Syntax" %}
```css
@keyframes animationName {
  from { 
    css-styles; 
  } 
  to { 
    css-styles;
  }
}
```
{% endcode %}

`from`, `to`키워드 대신 %를 사용하여 또한 시작과 끝 키프레임 사이에 %단위로 키프레임을 삽입할 수 있다.

```css
@keyframes move {
  0% {
    top: 0px;
  }
  25% {
    top: 20px;
  }
  75% {
    top: 175px;
  }
  100% {
    top: 200px;
  }
}
```

#### Reference

Using CSS animations [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Animations/Using_CSS_animations)

animation [→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/CSS/animation)

@keyframes [→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/CSS/@keyframes)

CSS3 Animation [→\(SITE\)](https://poiemaweb.com/css3-animation)

Transitions & Animations[ →\(SITE\)](https://learn.shayhowe.com/advanced-html-css/transitions-animations/)

