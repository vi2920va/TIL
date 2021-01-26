# CSS gradient

### 1. GRADIENT

그레디언트\(gradient\)는 한 색에서 다른 색으로 연결되는 중간 단계를 그라데이션 이라고 하며,  종류에는 선형\(linear\), 원형\(radial\)그레디언트가 있다.

#### 1\) linear grandint

선형 그레디언트\(linear gradient\)는 그레디언트 라인\(gradient\)이라는 각각의 점이 다른 컬러값을 갖는 하나의 축을 정의할 수 있다. 그레디언트 라인은 그레디언트를 포함하는 box 형태의 영역 중심 좌표와 각도로 정의된다. 그레디언트 컬러값은 시작점\(starting point\), 종료점\(ending point\)과 두 점 사이에 삽입 가능한 색상점\(color stop point\)들로 정의된다.

시작점은 그레디언트 라인상에서 그레디언트 색상이 시작되는 지점을 의미하고, 종료점은 시작점과 비슷하게 그레디언트 색상이 종료지점을 의미한다. 이 처럼 시작점과 종료점 사이에 색상점은 이용하여 좀 더 다양한 색상 전환 효과를 생성할 수 있으며, 다중 색상 그레디언트\(multi color gradient\)를 구성할 수 있다.

{% code title="Syntax" %}
```css
background: linear-gradient([<angle> | to <side-or-corner>]?, <color-stop-list>);
```
{% endcode %}

📝`<side-or-corner> = [left | right] || [top | bottom]`

기본값은\(bottom\)으로 그레디언트의 방향을 지정하고, 색상의 정지 위치를 결정하는 그레디언트 라을 지정한다.

📝`<angle>`

그레디언트가 어느 방향으로 향하는지 각도\(deg\)를 결정한다.



```css
/* 기본 선형 그레디언트 각도를 지정하지 않으면 위에서 아래로 적용 */
background: linear-gradient(blue, pink);

/* left에서 시작해서 right에서 종료, blue로 시작해서 red로 종료 */
background: linear-gradient(to right, blue, pink);

/* left bottom 시작해서 right top에서 종료, blue로 시작해서 red로 종료 */
background: linear-gradient(to bottom right, blue, pink);
```



