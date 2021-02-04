# CSS grid container

### 1. GRID

CSS grid는 2차원 행과 열의 레이아웃 시스템을 제공한다. 좀 더 복잡한 레이아웃을 위해서 grid를 사용할 수 있다. grid가 잘 적용되는지 확인하기 위해서는 파이어폭스 브라우저에서 테스트 하는 것을 추천한다.

#### 1\) Grid 용어

* Gird 라인\(lines\) - Grid를 행\(rows\) / 열\(colums\)로 나누는 수평선 또는 수직선.
* Grid 셀\(cell\) - Grid를 구성하는 단일 유닛\(single unit\).
* Grid 영역\(area\) - Grid 라인이 감싸는 사각형 영역으로 Grid 영역은 여러 개의 Grid 셀을 포함할 수 있다.
* Grid 트랙\(track\) - 2개의 그리드 라인 사이 공간을 의미, 이 공간은 수평 / 수직 방향 모두를 말한다.
* Grid 행\(row\) - 1개의 Grid 수평 트랙.
* Grid 열\(colum\) - 1개의 Grid 수직 트랙.
* 거터\(Gutter\) - Gird 행과 열 사이이 공간.

### 2. grid propertoies

grid는 flex와 같이 **container**와 **item** 이라는 두 가지 개념으로 구분된다. **container**는 **items**를 감싸는 부모 요소이며, 그 안에서 각 **item**을 배치할 수 있다.

### 3. grid container properites

gird container를 위한 속성들은 아래와 같다.

* `display`
* `grid-template-rows`
* `grid-template-columns`
* `grid-template-areas`
* `grid-template`
* `row-gap(grid-row-gap)`
* `column-gap(grid-column-gap)`
* `gap(grid-gap)`
* `grid-auto-rows`
* `grid-auto-columns`
* `grid-auto-flow`
* `grid`
* `align-content`
* `justify-content`
* `place-content`
* `align-items`
* `justify-items`
* `place-items`

#### 1\) display

그리드 사용하기 위해 컨테이너에 필수로 작성하는 속성으로 gird container를 정의한다.

| value | description |
| :--- | :--- |
|  `gird` | block 특성의 grid container를 정의. |
| `inline-grid` | inline 특성의 grid container를 정의. |

#### 2\) grid-templeate-rows / grid-template-colums

명시적 행의 크기를 정의할 때는 `grid-template-rows` 속성을 사용하고, 열의 크기를 정의할 때는 `grid-template-cloums`속성을 사용.

```css
.grid{
  display: grid;
  /* 행 템플릿 (rows template) */
  grid-template-rows: 10rem 10rem;
  /* 열 템플릿 (columns template) */
  grid-template-columns: 10rem 10rem 10rem;
}
```

#### 3\) grid-template-areas

지정된 그리드 영역 이름 `grid-area`를 참조해 그리드 템플릿을 생성한다. 이때 `grid-area` 속성은 gird container가 아닌 gird item에 적용하는 속성.

#### 4\) grid-temaplate

`grid-template-`\* 관련된 속성을 단축해서 한 줄에 작성할 수 있는 속성.

#### 5\)  grid-row-gap / grid-column-gap 

`grid-row-gap` 속성은 각 행과 행 사이의 간격\(gutter\)를 지정하고, `grid-column-gap` 속성은 각 열과 열 사이 간격을 지정한다.

#### 6\) grid-gap

각 행과 행, 열과 열 사이 간격을 지정한다.

#### 7\)  grid-auto-rows / grid-auto-colums







