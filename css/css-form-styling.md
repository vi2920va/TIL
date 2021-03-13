---
description: CSS form styling
---

# 폼 스타일링

### 1. form styling

사용자가 입력된 내용의 상태를 이해하고 대처할 수 있도록 고려하여 설계해야 한다.

#### 1\) form styling 어려운 이유

사 용자는 각 운영체제가 가진 컨트롤의 사각적인 모양에 익숙하므로, 브라우저 제조사는 폼 컨트롤을 스타일리쉬하게 만드는데 소홀했고, 오늘 날에도 모든 폼 컨트롤을 스타일링 하는 것은 쉽지 않다. 하지만 브라우저 제조사는 전과 달리 폼 컨트롤에 대한 CSS 지원을 향상 시키려고 노력하고 있다.

#### 2\) form styling  level

**The Good** - CSS를 사용해 완벽하게 스타일링 할 수 있는 요소

* `<form>`
* `<fieldset>`
* `<label>`
* `<output>`

**The Bad** - CSS를 사용해 완벽하게 스타일링 할 수 없는 요소들

* `<legend>`
* `placeholder`속성

**The Ugly** - CSS를 스타일링 전혀 적용되지 않는 요소들

* `<select>`
* `<option>`
* `<optgroup>`
* `<datalist>`
* `<progress>`
* `<meter>`

#### Result

#### 💻 simple login form [→\(CODEPEN\)](https://codepen.io/vi2920va/full/vYXPBWV)

 



