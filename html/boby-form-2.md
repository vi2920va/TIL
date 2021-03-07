# FORMS : button, select, option, optgroup elements

### 1. &lt;button&gt; element

`<button>` 요소는 클릭할 수 있는 버튼을 정의할 때 사용한다.

#### 1\) &lt;button&gt; element - ATTRIBUTES

<table>
  <thead>
    <tr>
      <th style="text-align:center">attribute</th>
      <th style="text-align:center">attribute value</th>
      <th style="text-align:center">description</th>
      <th style="text-align:center">spec</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:center"><code>autofocus</code>
      </td>
      <td style="text-align:center">autofocus</td>
      <td style="text-align:center">&#xD398;&#xC774;&#xC9C0;&#xAC00; &#xB85C;&#xB4DC;&#xB420; &#xB54C; &#xC790;&#xB3D9;&#xC73C;&#xB85C;
        &#xD3EC;&#xCEE4;&#xC2A4; &#xBC84;&#xD2BC;&#xC73C;&#xB85C; &#xC774;&#xB3D9;&#xB428;&#xC744;
        &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center">HTML5</td>
    </tr>
    <tr>
      <td style="text-align:center"><code>disabled</code>
      </td>
      <td style="text-align:center">disabled</td>
      <td style="text-align:center">&#xD574;&#xB2F9; &#xBC84;&#xD2BC;&#xC774; &#xBE44;&#xD65C;&#xC131;&#xB428;&#xC744;
        &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>form</code>
      </td>
      <td style="text-align:center">forn id</td>
      <td style="text-align:center">&#xD574;&#xB2F9; &#xBC84;&#xD2BC;&#xC774; &#xD3EC;&#xD568;&#xB420; &#xD558;&#xB098;
        &#xC774;&#xC0C1;&#xC758; <code>&lt;form&gt;</code>&#xC694;&#xC18C;&#xB97C;
        &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center">HTML5</td>
    </tr>
    <tr>
      <td style="text-align:center"><code>formaction</code>
      </td>
      <td style="text-align:center">URL</td>
      <td style="text-align:center">
        <p>&#xD3FC; &#xB370;&#xC774;&#xD130;(form data)&#xAC00; &#xC11C;&#xBC84;&#xB85C;
          &#xC81C;&#xCD9C;&#xB420; &#xB54C; &#xD574;&#xB2F9; &#xB370;&#xC774;&#xD130;&#xAC00;
          &#xB3C4;&#xCC29;&#xD560; URL&#xC744;</p>
        <p>&#xBA85;&#xC2DC;</p>
        <p>(&lt;button&gt; &#xC694;&#xC18C;&#xC758; type &#xC18D;&#xC131;&#xAC12;&#xC774;
          &quot;submit&quot;&#xC778; &#xACBD;&#xC6B0;&#xC5D0;&#xB9CC; &#xC0AC;&#xC6A9;&#xD560;
          &#xC218; &#xC788;&#xB2E4;.)</p>
      </td>
      <td style="text-align:center">HTML5</td>
    </tr>
    <tr>
      <td style="text-align:center"><code>formenctype</code>
      </td>
      <td style="text-align:center">
        <p>application/x-www-form-urlencoded</p>
        <p>multipart/form-data</p>
        <p>text/plain</p>
      </td>
      <td style="text-align:center">
        <p>&#xD3FC; &#xB370;&#xC774;&#xD130;&#xAC00; &#xC11C;&#xBC84;&#xB85C; &#xC81C;&#xCD9C;&#xB420;
          &#xB54C; &#xD574;&#xB2F9; &#xB370;&#xC774;&#xD130;&#xAC00; &#xC778;&#xCF54;&#xB529;
          &#xB418;&#xB294; &#xBC29;&#xC2DD;&#xC744; &#xBA85;&#xC2DC;</p>
        <p>(&lt;button&gt; &#xC694;&#xC18C;&#xC758; type &#xC18D;&#xC131;&#xAC12;&#xC774;
          &quot;submit&quot;&#xC778; &#xACBD;&#xC6B0;&#xC5D0;&#xB9CC; &#xC0AC;&#xC6A9;&#xD560;
          &#xC218; &#xC788;&#xB2E4;.)</p>
      </td>
      <td style="text-align:center">HTML5</td>
    </tr>
    <tr>
      <td style="text-align:center"><code>formmethod</code>
      </td>
      <td style="text-align:center">
        <p>get</p>
        <p>post</p>
      </td>
      <td style="text-align:center">
        <p>&#xD3FC; &#xB370;&#xC774;&#xD130;&#xAC00; &#xC11C;&#xBC84;&#xB85C; &#xC81C;&#xCD9C;&#xB420;
          &#xB54C; &#xC0AC;&#xC6A9;&#xD560; HTTP &#xBA54;&#xC11C;&#xB4DC;&#xB97C;
          &#xBA85;&#xC2DC;.</p>
        <p>(&lt;button&gt; &#xC694;&#xC18C;&#xC758; type &#xC18D;&#xC131;&#xAC12;&#xC774;
          &quot;submit&quot;&#xC778; &#xACBD;&#xC6B0;&#xC5D0;&#xB9CC; &#xC0AC;&#xC6A9;&#xD560;
          &#xC218; &#xC788;&#xB2E4;.)</p>
      </td>
      <td style="text-align:center">HTML5</td>
    </tr>
    <tr>
      <td style="text-align:center"><code>formnovalidate</code>
      </td>
      <td style="text-align:center">formnovalidate</td>
      <td style="text-align:center">
        <p>&#xD3FC; &#xB370;&#xC774;&#xD130;&#xAC00; &#xC11C;&#xBC84;&#xB85C; &#xC81C;&#xCD9C;&#xB420;
          &#xB54C; &#xD574;&#xB2F9; &#xB370;&#xC774;&#xD130;&#xC758; &#xC720;&#xD6A8;&#xC131;
          &#xAC80;&#xC0AC;&#xB97C; &#xD558;&#xC9C0; &#xC54A;&#xC74C;&#xC744; &#xBA85;&#xC2DC;.</p>
        <p>(&lt;button&gt; &#xC694;&#xC18C;&#xC758; type &#xC18D;&#xC131;&#xAC12;&#xC774;
          &quot;submit&quot;&#xC778; &#xACBD;&#xC6B0;&#xC5D0;&#xB9CC; &#xC0AC;&#xC6A9;&#xD560;
          &#xC218; &#xC788;&#xB2E4;.)</p>
      </td>
      <td style="text-align:center">HTML5</td>
    </tr>
    <tr>
      <td style="text-align:center"><code>formtarget</code>
      </td>
      <td style="text-align:center">
        <p>_blank</p>
        <p>_self</p>
        <p>_parent</p>
        <p>_top</p>
      </td>
      <td style="text-align:center">
        <p>&#xD3FC; &#xB370;&#xC774;&#xD130;&#xAC00; &#xC11C;&#xBC84;&#xB85C; &#xC81C;&#xCD9C;&#xB41C;
          &#xD6C4; &#xBC1B;&#xC740; &#xC751;&#xB2F5;(response) &#xB370;&#xC774;&#xD130;&#xB97C;
          &#xC5B4;&#xB514;&#xC5D0; &#xD45C;&#xC2DC;&#xD560;&#xC9C0; &#xBA85;&#xC2DC;.</p>
        <p>(&lt;button&gt; &#xC694;&#xC18C;&#xC758; type &#xC18D;&#xC131;&#xAC12;&#xC774;
          &quot;submit&quot;&#xC778; &#xACBD;&#xC6B0;&#xC5D0;&#xB9CC; &#xC0AC;&#xC6A9;&#xD560;
          &#xC218; &#xC788;&#xB2E4;.)</p>
      </td>
      <td style="text-align:center">HTML5</td>
    </tr>
    <tr>
      <td style="text-align:center"><code>name</code>
      </td>
      <td style="text-align:center">text</td>
      <td style="text-align:center">&#xD574;&#xB2F9; &#xBC84;&#xD2BC;&#xC758; &#xC774;&#xB984;(name)&#xC744;
        &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>type</code>
      </td>
      <td style="text-align:center">
        <p>button</p>
        <p>reset</p>
        <p>submit</p>
      </td>
      <td style="text-align:center">&#xD574;&#xB2F9; &#xBC84;&#xD2BC;&#xC758; &#xD0C0;&#xC785;(type)&#xC744;
        &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>value</code>
      </td>
      <td style="text-align:center">text</td>
      <td style="text-align:center">&#xD574;&#xB2F9; &#xBC84;&#xD2BC;&#xC758; &#xCD08;&#xAE30;&#xAC12;(value)&#xB97C;
        &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center"></td>
    </tr>
  </tbody>
</table>

#### 2\) &lt;button&gt; 접근성 고려사항

#### 📝**icon &lt;**button&gt;

아이콘만 사용해 기능을 표현하는 버튼은 접근 가능한 이름을 갖지 않는다.

아이콘 버튼에 접근 가능한 이름을 부여하려면 `<button>` 요소의 **기능을 간략히 묘사하는 텍스트**를 안에 포함 시켜야 한다.

{% code title="icon button" %}
```markup
<button name="favorite" type="button">
  <svg aria-hidden="true" viewBox="0 0 10 10">
  <path d="M7 9L5 8 3 9V6L1 4h3l1-3 1 3h3L7 6z"/></svg>
  Add to favorites
</button>
```
{% endcode %}

#### 📝**크기**

버튼과 같은 대화형 요소는 상호작용하기 충분한 크기의 활성화 영역을 가져야 한다.

충분한 크기는 운동 조절 장애를 가진 사용자와, 터치 스크린 처럼 정확하지 입력 도구 사용자 처럼 다양한 사람을 돕는다. **최소 44 x 44** CSS px\(픽셀\) 크기를 권고 한다.

#### 📝**간격**

버튼과 같은 대화형 요소 다수를 시각적으로 가까이 배치할 땐 서로를 분리하는 공간을 둬야 한다.

간격은 운동 조절 장애를 가진 사용자와 우너하지 않는 상호작용을 하는 걸 방지할 수 있다.

간격은 `margin`과 같은 CSS 속성으로 설정할 수 있다.

### 2. &lt;select&gt; element

`<select>` 요소는 옵션 메뉴를 제공하는 드롭다운 리스트\(drop down list\)를 정의할 때 사용한다.

`<select>` 요소 내부의 `<option>`요소는 드롭다운 리스트에서 사용되는 각각의 옵션을 정의한다.

`<select>` 는 `<label>`과 연결해 접근성을 향상 시킨다.

이러한 &lt;select&gt;요소는 사용자로부터 입력 받기 위한 폼에 사용될 수 있다.

```markup
<label for="coffe-select">Click Coffee Menu :</label>
<select name="coffes" id="coffe-select">
  <option value="">--Please choose an option--</option>
  <option value="caffe-americano">Caffe Americano</option>
  <option value="caffe-latte">Caffe Latte</option>
  <option value="caramel-macchiato">Caramel Macchiato</option>
  <option value="strawberry-yogurt">Strawberry Yogurt</option>
</select>
```

#### 1\) &lt;select&gt; element - attributes

| attribute | attribute value | description | spec |
| :---: | :---: | :---: | :---: |
| `autofocus` | autofocus | 페이지가 로드될 때 자동으로 포커스가 드롭다운 리스트로 이동됨을 명시. | HTML5 |
| `disabled` | disabled | 해당 드롭다운 리스트가 비활성됨을 명시. |  |
| `form` | form id | 해당 드롭다운 리스타가 포함될 하나의 `<form>` 요소를 명시. | HTML5 |
| `multiple` | multiple | 사용자가 한 번에 두 개 이상 옵션을 선택할 수 있음을 명시. |  |
| `name` | text | 드롭다운 리스트 이름을 명시. |  |
| `required` | required | 폼 데이터가 서버로 제출되기 전 사용자가 반드시 드롭다운 리스트의 값을 선택해야 함을 명시. | HTML5 |
| `size` | number | 드롭다운 리스트에서 한 번에 보일 옵션의 개수를 명시. |  |

### 3. &lt;option&gt; element <a id="reference"></a>

`<option>`요소는 옵션 메뉴를 제공라는 드롭 다운 리스트에서 사용되는 하나의 옵션을 정의할 때 사용한다.이러한 `<option>`요소는 `<select>`요소 또는 `<datalist>`요소 내부에서만 위치할 수 있다.

`<option>`요소는 아무런 속성도 명시하지 않은 채 사용할 수 있지만, 서버로 제출되는 값을 명시하는 `value` 속성은 명시하는 것이 일반적이다. 만약 옵션의 개수가 많다면 `<optgroup>`요소를 사용하여 관련된 옵션들을 좀 더 보기 좋게 서로 묶어준다.

#### 1\) &lt;option&gt; element - attributes

| attribute | attribute value | description |
| :---: | :---: | :---: |
| `disabled` | disabled | 해당 옵션이 비활성됨을 명시. |
| `label` | text | 해당 옵션의 라벨\(label\)을 명시. |
| `selected` | selected | 페이지가 로드될 때 옵션 중에서 미리 선택되어는지 옵션을 명시. |
|  `value` | value | 해당 옵션이 선택될 때 서버로 제출되는 값을 명시. |

### 4. &lt;optgroup&gt; element <a id="reference"></a>

`<optgroup>`요소는 옵션 메뉴를 제공하는 드롭다운 리스트에서 사용되는 옵션들의 그룹을 정의할 때 사용한다.

드롭다운 리스트에서 옵션의 수가 많을 경우 `<optgroup>` 요소를 사용하여 관련된 옵션끼리 각각의 그룹으로 묶어주면 사용자가 좀 더 쉽게 드롭다운 리스트를 사용할 수 있다.

#### 1\) &lt;optgroup&gt; element - attribute

| attribute | attribute value | description |
| :---: | :---: | :---: |
| `disabled` | disabled | 해당 옵션이 비활성됨을 명시. |
| `label` | text | 해당 옵션의 라벨\(label\)을 명시. |

#### Reference 

button element [→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/button)

select  element [→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/select)

option  element[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/option)

optgroup  element[ →\(MDN\)﻿](https://developer.mozilla.org/ko/docs/Web/HTML/Element/optgroup)

####  <a id="reference"></a>

