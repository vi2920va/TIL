---
description: CSS box-shadow
---

# 박스 그림자

### 1. BOX-SHADOW

텍스트에 그림자 효과를 표현하는 `text-shadow` 속성이 있듯이 CSS3에는 박스 요소에 그림자를 추가할 수 있는 방법으로 `box-shadow` 속성을 제공한다.

{% code title="Syntax" %}
```css
/* offeset-x | offset-y | color */
box-shadow: 60px -16px teal;

/* offset-x | offset-y | blur-radius | color */
box-shadow: 10px 5px 5px black;

/* offset-x | offset-y | blur-radius | spread-radius | color */
box-shadow: 2px 2px 2px 1px rgba(0, 0, 0, 0.2);

/* inset | offset-x | offset-y | color */
box-shadow: inset 5em 1em gold;

/* Any number of shadows, separated by commas */
box-shadow: 3px 3px red, -1em 0 0.4em olive;
```
{% endcode %}

📝`<length>`

* 두 개의 값을 사용하면 `<offset-x>`,`<offset-y>`로 분석.
* 세 번째 값이 주어지면 `<blur-radius>`로 분석.
* `inset`, `<color>` 키워드는 선택사항.

📝`inset`

값을 지정하지 않으면 요소가 공중에 떠 있는 것 처럼 밖에 있는 그림자가 된다. `inset` 키워드가 존재하면 요소가 움푹 들어간 것 처럼 그림자가 요소의 테두리 안, 배경색 위, 내부 콘텐츠에 밑에 그려지게 된다.

📝`<offset-x>`,`<offset-y>`

그림자의 위치를 설정하는 두 개의 `<length>` 값으로 x는 수평 거리로 그림자를 요소 왼쪽에 표시, y는 수직 거리로 요소 위쪽에 표시한다. 이때 `<blur-radius>` 또는 `<spread-radius>`가 존재하면 흐려지게 된다.

📝`<blur-radius>`

세 번째`<length>`값으로 크면 클수록 그림자 테두리가 흐려지므로 크기는 더 커지고 색은 더 밝아진다. 음수 값은 사용할 수 없으며 값을 설정하지면 0이 되어 테두리가 선명해지게 된다.

📝`<spread-radius>`

네 번째 `<length>` 값으로 양수 값은 그림자가 더 커지고 확산되며, 음수 값은 그림자가 줄어들게 된다.

📝`<color>`

#### Reference

box-shadow [→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/CSS/box-shadow)

text-shadow[ →\(MDN\)](https://developer.mozilla.org/en-us/docs/Web/CSS/text-shadow)

