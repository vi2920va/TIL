# CSS 3D transform

### 1. 3D TRANSFORM

CSS 3D trnasform은 평면에서 여러 개 CSS 속성을 조합하고 3D 공간에서 회전, 확대, 이동, 비틀기를 포함하고 원근감, 관찰자의 위치를 부여해 3D 공간을 만들어 낼 수 있다. 3D trnasform은 트랜스폼을 적용할 요소에 적용하는 속성과 자식 요소를 3D로 처리하기 위해 부모  요소에 설정하기 위한 속성이 있다.

#### 1\) 3D trnasform property method'

3D 변형\(transform\)을 위해 제공되는 메소드\(method\)는 다음과 같다.

* `translateX(x), translateY(y), translateZ(z), translate3d(x, y, z)`
* `roateX(x), rotateY(y), rotateZ(z), roate3d(x, y, z)`
* `scaleX(x), scaleY(y), scaleZ(z), scale3d(x, y, z)`
* `matrix3d(n x 16)`
* `perspective(n)`

#### 2\) perspective

![&#xC704;&#xC758; &#xC774;&#xBBF8;&#xC9C0;&#xC5D0;&#xC11C; &#xD30C;&#xB780;&#xC0C9; &#xC6D0;&#xD615;&#xC740; 3D &#xACF5;&#xAC04;&#xC0C1;&#xC758; &#xBB3C;&#xCCB4;, d&#xB294; &#xAD00;&#xCC30;&#xC790;&#xC640; &#xD654;&#xBA74;&#xACFC;&#xC758; &#xAC70;&#xB9AC;, z&#xB294; z&#xCD95; &#xC694;&#xC18C;&#xC758; &#xC704;&#xCE58;](../.gitbook/assets/perspective-distance.png)



`perspective` 속성은 원근감을 표시할 수 있도록 관찰자 시점\(위치\)의 거리를 지정하는 속성으로 z index와 관찰자 사이의 거리에 영향을줌으로써 요소에 3D 공간을 제공한다. `perspective`속성 값이 커질수록 왜곡이 적어지게 되고 즉, 관찰자 위치가 가까이서 본 형태의 3D로 나타나게 된다.

💻3D transform\(perspective\) [→\(CODEPEN\)](https://codepen.io/vi2920va/full/yLarzRY)

#### Reference

css\_reference perspective [→\(SITE\)](https://tympanus.net/codrops/css_reference/perspective/)





