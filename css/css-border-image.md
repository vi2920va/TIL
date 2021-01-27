# CSS border-image

### 1. BORDER-IMAGE

border-image 속성은 요소의 주위에 이미지를 그린다. 일반 테두리를 대체한다.

{% code title="Syntax" %}
```css
/* source | slice */
border-image: linear-gradient(red, blue) 27;

/* source | slice | repeat */
border-image: url("/images/border.png") 27 space;

/* source | slice | width */
border-image: linear-gradient(red, blue) 27 / 35px;

/* source | slice | width | outset | repeat */
border-image: url("/images/border.png") 27 23 / 50px 30px / 1rem round space;
```
{% endcode %}

border-image 속성은 아래에 나열한 값 중 한 개에서 다섯 개 사이를 사용해 지정할 수 있다.

📝`<border-image-source>`

테두리로 사용할 이미지를 설정.

📝`<border-image-slice>`

테두리로 사용할 이미지를 자르는 방법을 설정.

📝`<border-image-width>`

테투리 이미지의 너비값을 설정.

📝`<border-image-outset>`

테두리 영역 너머로 테두리로 사용할 이미지가 얼마만큼 넘어갈지를 설정.

📝`<border-image-repeat>`

테두리로 사용할 이미지의 중간 부분의 처리를 반복 또는 늘릴지 설정.

#### Reference

border-image [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/CSS/border-image)

