# CSS 3D transform

## 1. 3D TRANSFORM

> CSS 3D trnasform은 평면에서 여러 개 CSS 속성을 조합하고 3D 공간에서 회전, 확대, 이동, 비틀기를 포함하고 원근감, 관찰자의 위치를 부여해 3D 공간을 만들어 낼 수 있다. 3D trnasform은 트랜스폼을 적용할 요소에 적용하는 속성과 자식 요소를 3D로 처리하기 위해 부모  요소에 설정하기 위한 속성이 있다.

CSS 3D transform 공간을 위해서는 소실점\(투영점, 원근감\)을 지정해야 한다. 그렇지 않으면 의도한 3D 효과가 나타나지 않고 평면으로 보이게 된다. 

### 1\) 3D trnasform property method

3D 변형\(transform\)을 위해 제공되는 메소드\(method\)는 다음과 같다.

* `translateX(x), translateY(y), translateZ(z), translate3d(x, y, z)`
* `roateX(x), rotateY(y), rotateZ(z), roate3d(x, y, z)`
* `scaleX(x), scaleY(y), scaleZ(z), scale3d(x, y, z)`
* `matrix3d(n x 16)`
* `perspective(n)`

### 2\) perspective

![&#xC704;&#xC758; &#xC774;&#xBBF8;&#xC9C0;&#xC5D0;&#xC11C; &#xD30C;&#xB780;&#xC0C9; &#xC6D0;&#xD615;&#xC740; 3D &#xACF5;&#xAC04;&#xC0C1;&#xC758; &#xBB3C;&#xCCB4;, d&#xB294; &#xAD00;&#xCC30;&#xC790;&#xC640; &#xD654;&#xBA74;&#xACFC;&#xC758; &#xAC70;&#xB9AC;, z&#xB294; z&#xCD95; &#xC694;&#xC18C;&#xC758; &#xC704;&#xCE58;](../.gitbook/assets/perspective-distance.png)



`perspective` 속성은 원근감을 표시할 수 있도록 관찰자 시점\(위치\)의 거리를 지정하는 속성으로 z index와 관찰자 사이의 거리에 영향을줌으로써 요소에 3D 공간을 제공한다. `perspective`속성 값이 커질수록 왜곡이 적어지게 되고 즉, 관찰자 위치가 가까이서 본 형태의 3D로 나타나게 된다.

💻3D transform\(perspective\) [→\(CODEPEN\)](https://codepen.io/vi2920va/full/yLarzRY)

### **2-1\) perspective vs perspective\(\)**

부모 요소에게 perpective 속성을 주면 각 박스들은 저 마다 다른 투영점\(perpective\)과 다른 소실점을\(vanishing point\)을 갖고 있기 때문에 의도치 않은 결과를 나타나게 된다. 

💻3D trnasform\(perspective children\) [→\(CODEPEN\)](https://codepen.io/vi2920va/full/mdrYxyG)

개별적인 투영점을 설정할 때는 `transform` 속성의 값으로 `perpetive`를 주고 괄호 안에 수치를 입력한다.

```css
.panel--separate {
  transform: perspective(400px) rotateY(45deg);
}
```

💻 3D tranform\(perspective function\) [→\(CODEPEN\)](https://codepen.io/vi2920va/full/GRjaxJY)

### 3\) perspective-origin

perspective 속성과 함께 소실점으로 나타내는데 사용한다. 이 속성은 관찰자가 어느 위치에서 보고 있는지를 나타내는 속성.

![perspective-origin &#xAC12;&#xC5D0; &#xB530;&#xB77C;&#xC11C; &#xC18C;&#xC2E4;&#xC810;&#xC774; &#xB2EC;&#xB77C;&#xC9C0;&#xB294; &#xC608;&#xC81C; &#xAE30;&#xBCF8;&#xAC12;&#xC740; x&#xCD95;/y&#xCD95; &#xAC01;&#xAC01; 50% 50%](../.gitbook/assets/.png%20%285%29.png)

💻 3D transform\(persopectve-origin\) [→\(CODEPEN\)](https://codepen.io/vi2920va/pen/XWjwEdp)



#### Reference

css\_reference perspective [→\(SITE\)](https://tympanus.net/codrops/css_reference/perspective/)

Card Filp [→\(SITE\)](https://3dtransforms.desandro.com/card-flip)





