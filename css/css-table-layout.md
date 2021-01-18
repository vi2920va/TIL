# CSS table layout

### 1. TABLE LAYOUT

테이블\(table\)은 복잡한 정보를 제공하기에 특히 접근성을 고려해서 디자인/스타일링 해야한다. 웹 브라우저의 테이블 기본 스타일링은 공간이 협소하고, 각 행\(rows\)과 각 열\(columms\)간 구분이 명확하지 않다.

#### 1\) table element → &lt;caption&gt;

테이블 디자인 시, 접근성 고려하여 작성된 테이블 제목 caption 요소는 시각 디자인 과정에서 그리지 않기도 한다. 시각 디자인 상에서 그려지지 않았다 하더라도, 프론트엔드 개발자는 모든 사용자를 고려하여 테이블 요약 내용을 구조화 해야 한다. 

#### 2\) [a11y-hidden](https://snook.ca/archives/html_and_css/hiding-content-for-accessibility) class

스크린리더\(screen reader\) 사용자가 테이블 요약을 들을 수 있도록 요약을 제공하되, 시각 디자인 결과와 같이 화면에서는 감춰야 한다. 접근성을 고려하여 콘텐츠를 화면서 감추려면 CSS를 사용하여 재사용\(reusable\)가능하도록 클래스\(class\)로 설계\(design\)하여 사용해야 한다.

### 2.  table styling

#### 1\) border

테이블, 요소 셀\(제목/내용\)의 테두리\(border\)를 디자인 할 수 있다.

#### 2\) border-collapse

테이블 셀 사이 간격을 접거나\(collapse\), 나눌\(separate\) 수 있다. 이 속성은 오직 `<table>`요소에만 사용할 수 있다.

#### 3\) border-spacing

테이블 테두리 사이 간격을 설정할 수 있다. 이 속성을 사용하기 위해서는 `border-collapse`의 속성 값이 `separate`일 때 셀 간의 공백의 크기를 조절 할 수 있다.

#### 4\) caption-side

테이블 캡션 위치\(`top`, `bottom`\)를 설정 할 수 있다.

#### 5\) table-layout

테이블 레이아웃\(`auto`, `fixed`\) 설정을 통해 콘텐츠의 양에 따라 셀의 크기를 변경하거나, 고정 할 수 있다. \(`fixed` 설정 시, `width` 설정 필요\)

#### 6\) empty-cells

빈 셀\(empty cells\)의 표시\(`show` \| `hide`\) 설정이 가능하다. \(`hide` 설정 시 빈 셀은 화면에 그려지지 않는다.\)

#### 7\) margin/padding

테이블 셀은 `margin` 속성이 설정되지 않는다. 반면에 `padding`속성은 설정 가능하다.











