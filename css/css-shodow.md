# CSS box-shadow

### 1. BOX-SHADOW

텍스트에 그림자 효과를 표현하는 text-shadow 속성이 있듯이 CSS3에는 박스 요소에 그림자를 추가할 수 있는 방법으로 box-shadow 속성을 제공한다.

{% code title="" %}
```text
/* offset-x | offset-y | color */
box-shadow: 60px -16px teal;

/* offset-x | offset-y | blur-radius | color */
box-shadow: 10px 5px 5px black;

/* offset-x | offset-y | blur-radius | spread-radius | color */
box-shadow: 2px 2px 2px 1px rgba(0, 0, 0, 0.2);

/* inset | offset-x | offset-y | color */
box-shadow: inset 5em 1em gold;

/* Any number of shadows, separated by commas */
box-shadow: 3px 3px red, -1em 0 0.4em olive;

/* Global keywords */
box-shadow: inherit;
box-shadow: initial;
box-shadow: unset;
```
{% endcode %}



