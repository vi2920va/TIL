# CSS animation

### 1. ANIMATION

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

#### 3\) animation-name

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

#### 4\) animation-duration

`animation-duration` 속성은 애니메이션을 한 번 재생하는 데 걸리는 시간을 설정한다. 기본값은 0으로 설정되었기 때문에 아무런 움직임도 발생하지 않으며 또한 값이 음수로 설정할 경우에도 애니메이션은 재생되지 않는다.



#### 5\) animation-delay

animation-delay 속성은 애니메이션 시작을 지연할 시간을 설정하는 속성.

| property value | description |
| :--- | :--- |
| `0`\(defalut\) | 기본값으로 애니메이션을 시작한다. |
| `now` | `0`으로 설정한 값과 같이 애니메이션을 시작한다.  |
| `s/ms` | 설정한 시간이 지난 뒤에 애니메이션을 시작한다. 설정한 값이 음수가 아니라 양수이면 '-1s' 1초가 지난 뒤의 장면부터 애니메이션을 재생한다. |

#### 6\) animation-direction

`animation-direction` 속성은 애니메이션의 재생 방향을 정의하는 속성이다. `@keyframes` 속성의 `from`에서 `to`로 재생하는 것이 순방향 이고, `to`에서 `from`으로 재생하는 것이 역방향이다. 

| property value | description |
| :--- | :--- |
| `noraml`\(defalut\) |  애니메이션을 순방향으로 재생하고 재생이 한 번 끝나면 첫 번째 프레임부터 다시 시작한다. |
| `alternate` | 애니메이션을 순방향으로 시작해 역방향과 순방향으로 번갈아서 애니메이션을 재생한다. 홀수 번째로 재생할 때는 순방향으로 재생하고, 짝수 번째로 재생할 때는 역방향으로 재생한다. |
| `reverse` | 애니메이션을 역방향으로 재생하고 재생이 한 번 끝나면 마지막 프레임부터 다시 시작한다. |
| `alternate-reverse` | 애니메이션을 역방향으로 시작해 순방향과 역방향으로 번걸아서 애니메이션을 재생한다. 홀수 번째로 재생할 때는 역방향으로 재생하고, 짝수 번째로 재생할 때는 순방향으로 재생한다. |

#### 7\) animation-iteration-count

`animation-iteration-count` 속성은 애니메이션을 재생하는 횟수를 정의하는 속성.

| property value | description |
| :--- | :--- |
| `1`\(default\) | 숫자\(number\)값으로 설정한 횟수만큼 애니메이션을 설정한다. 설정한 값 숫자가 소수 일 경우에 애니메이션 재생 도중에 첫 번째 프레임으로 돌아가 멈춘다. 또한 숫자가 음수일 경우에 애니메이션을 재생하지 않는다. |
| `infinite` | 애니메이션을 무한으로 반복한다. |

#### 8\) animation-play-state

이 속성은 애니메이션 재생 여부를 정의하는 속성.

| property value | description |
| :--- | :--- |
| `running` | 애니메이션을 재생한다. |
|  `paused` | 애니메이션을 정지한다. |







