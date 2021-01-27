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



