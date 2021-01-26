# CSS gradient

### GRADIENT

> 그레디언트\(gradient\)는 한 색에서 다른 색으로 연결되는 중간 단계를 그라데이션 이라고 하며,  종류에는 선형\(linear\), 원형\(radial\)그레디언트가 있다.

### 1. linear-gradient\(\)

![linear-grandeient\(\)](../.gitbook/assets/linear-gradient.png)

선형 그레이디언트는 하나의 축\(그레이디언트 라인\)과 두 개 이상의 색상 정지점으로 정의할 수 있다. 축 위의 점은 모두 고유한 색을 가집니다. `linear-gradient()` 함수는 부드러운 그레이디언트를 만들기 위해 축과 직교하는 무수한 선을 그리며, 각 수직선의 색은 축과 교차하는 점의 색과 일치합니다.

{% code title="Syntax" %}
```css
background: linear-gradient([ <angle> | to <side-or-corner> ]? ,<color-stop-list>);
```
{% endcode %}

```css
/* 기본 선형 그레디언트 각도를 지정하지 않으면 위에서 아래로 적용 */
background: linear-gradient(blue, pink);

/* left에서 시작해서 right에서 종료, blue로 시작해서 red로 종료 */
background: linear-gradient(to right, blue, pink);

/* left bottom 시작해서 right top에서 종료, blue로 시작해서 red로 종료 */
background: linear-gradient(to bottom right, blue, pink);
```

📝`<side-or-corner>`

그레디언트 축의 시작점. to 이후 최대 두 개 방향을 나타내는 키워드를 사용할 수 있다.  하나는 수평 방향이고, 다른 하나는 수직 방향이다. 기본값 to bottom이다.

📝`<angle>`

그레디언트 축의 방향으로 odeg는 to top와 같다. 0 이상의 값을 지정하면 축이 시계 방향으로 돌아간다.

#### 1\) gradient angle / \(left, top, right, bottom\)

선형 그레디언트의 각도는 그레디언트가 어느 방향으로 향하는지 결정하는 데 사용한다. 

```css
/* 0deg(360deg) : 아래에서 위로 그레디언트 방향이 진행 */
background: linear-gradient(0deg, blue, pink);

/* 90deg : 왼쪽에서 오른쪽으로 그레디언트 방향이 진행 */
background: linear-gradient(90deg, blue, pink);

/* 180deg : 위에서 아래로 그레디언트 방향이 진행 */
background: linear-gradient(180deg, blue, pink);
  
/* 270deg : 오른쪽에서 왼쪽으로 그레디언트 방향이 진행 */
background: linear-gradient(270deg, blue, pink);
```



