# CSS backgrounds

### 1. BACKGROUND DESIGN

요소의 **배경\(background\)** 속성을 사용하면 **배경의 색상, 이미지, 위치, 반복, 고정 여부 등을 설정할** 수 있다. 그리고 모던 브라우저에서는 배경 이미지의 시작점\(origin\)을 조정하거나, 클리핑\(clipping\) 영역을 설정 할 수 있다.

요소의 배경이 지정된 공간은 요소의 `content-box`, `padding-box`, `border-box`까지 포함되고, 모던 브라우저에서는 배경을 차지하는 영역을 `background-clip` 속성을 사용하여 변경할 수 있다.

#### 1\) background-color

HTML 요소의 배경색 설정. \(default : `transparent`\)

#### 2\) background-image

HTML요소의 배경으로 나타날 배경 이미지를 설정.  \(default : `none`\)

#### 3\) background-position

배경 이미지의 시작 위치를 지정, 일반적으로 배경 이미지는 왼쪽 위에서 부터 이미지를 표시한다. 이때 이 속성을 사용하게 되면 이미지의 좌표를 원하는 위치에 놓을 수 있으며, 공백\(speace\)을 기준으로 `x, y`좌표를 지정하여 사용한다.  \(default : `left top`\)

#### 4\) background-repeat

배경에 이미지를 넣었다면 이미지를 한 번만 넣을지 반복해서 넣을지 여부를 지정할 수 있다. 일반적을호 컨테이너 박스 보다 작은 이미지를 적용할 시 이미지가 반복되어 출력된다.  \(default : `repeat`\)

#### 5\) background-attachment

위치가 설정된 배경 이미지를 해당 위치에 고정시킬 수도 있다. 이렇게 고정된 배경이미지는 스크롤과 무관하게 화면의 위치에서 이동하지 않는다. \(default : `scroll`\)

#### 6\) background

위에 있는 5가지 배경 속성을 모아 작성하는 속기법**.**

#### 7\) background-size

배경 이미지의 크기를 동적으로 조정하여 설정. \(default : `auto`\)

#### 8\) background-clip

 배경\(이미지나 배경색\)을 어느 부분\(박스\)영역까지 표현할 지를 지정하는 속성. \(default : `border-box`\)

#### 9\) background-origin

 배경 이미지가 어느 위치에서 기준점을 기준으로 잡느냐를 정의하는 속성 \(default : `padding-box`\)







