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

`animation-name` 속성은 `@keyframes` 속성에서 설정한 애니메이션의 이름이다. 이름을 설정해야 애니메이션을 재생할 수 있다. 즉, 이름을 정의해야 애니메이션을 재생\(호출\)할 수 있다. 

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

animation-duration 속성은 애니메이션을 한 번 재생하는 데 걸리는 시간을 설정한다. 기본값은 0으로 설정되었기 때문에 아무런 움직임도 발생하지 않으며 또한 값이 음수로 설정할 경우에도 애니메이션은 재생되지 않는다.

#### 5\) animation-delay

animation-delay 속성은 애니메이션 시작을 지연할 시간을 설정하는 속성으로 값으로는 `0`, `now`, `숫자 또는 단위`로 값을 사용할 수 있다. 이때 값이 양수\(-1s\)이면 1초가 지난 뒤의 장면부터 애니메이션을 재생한다.

#### 6\) animation-direction











