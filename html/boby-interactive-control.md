---
description: 'BOBY : Interactive control'
---

# 인터렉티브 요소

### 1. Interactive control

인터랙티브 컨트롤\(interactive control\)은 사용자가 입력한 데이터를 브라우저나 서버로 전송하기 위한 도구이다. 과거에는 데이터 전송을 위해 폼이나 자바스크립트를 이용해야먄 했다. 웹이 점점 애플리케이션화 되면서 웹 문서 어느 곳에서든 전송이 이루어질 필요가 있었고, 이를 위해 새롭게 요소가 제안되었다.

#### 1\) &lt;detalis&gt; element

`<detalis>`요소는 사용자가 직접 조작하여 보거나 숨길 수 있는 세부사항\(additional detalis\)을 명시할 때 사용한다. 보통 사용자가 직접 접거나 펼 수 있는 대화영 위젯\(interactive widget\)을 정의할 때  사용되면, 그 안에는 어떠한 종류의 콘텐츠도 포함될 수 있다. 이러한 요소의 콘텐츠는`open`속성이 설정되기 전까지 화면에 보여지지 않는다.

`<summary>`요소는 `<detalis>`요소에서 화면에 보일 제목\(visble heading\)을 명시할 때 사용한다. 이 제목을 마우스로 클릭함으로써 `<detalis>`요소를 보이도록 할 수도 있고 숨길 수도 있다.

```markup
<details>
    <summary>today's exchange rate</summary>
    <ul>
        <li>dollar($) : 1,135.90</li>
        <li>euro(€) : 1,284.08</li>
        <li>en(￥) : 1,014.88</li>
    </ul>
</details>
```

#### 2\) &lt;summary&gt; element

`<summary>`요소는 `<details>`요소에 의해 생성되는 대화형 위젯에서 기본적으로 보이는 제목을 정의할 때 사용한다. `<summary>`요소는 반드시 `<detalis>`요소의 첫 번째 자식 요소이어야 하며, 이 제목을 마우스로 클릭함으로써 `<details>`요소를 보이도록 할 수도 있고 숨길 수도 있다.

#### 3\) &lt;dialog&gt; element

`<dialog>`요소는 대화 상자\(dialog box\)나 대화 윈도우\(dialog window\)를 정의할 때 사용한다. 이 요소는 웹 페이지에서 손 쉽게 팝업 대화 상자를 만들 수 있도록 해준다.

```markup
<dialog open>This is an open dialog window</dialog>
```

  






