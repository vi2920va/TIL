# FORMS : textarea, fieldset, lengend...elements

### 1. TEXTAREA ELEMENT

`<textarea>` 요소는 사용자가 여러 줄의 텍스트를 입력할 수 있는 텍스트 영역을 정의할 때 사용한다. 텍스트 입력 영역에는 개수의 제한 없이 문자를 입력할 수 있으며, 입력된 문자는 고정폭 글꼴로 렌더링 된다.

텍스트 영역의 크기는 `<textarea>`요소의 `cols`속성과 `rows`속성으로 지정할 수 있다.

#### 1\) TEXTAREA  ELEMENT - ATTRIBUTES

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
        &#xD3EC;&#xCEE4;&#xC2A4;&#xAC00;<code>&lt;textarea&gt;</code>&#xC694;&#xC18C;&#xB85C;
        &#xC774;&#xB3D9;&#xB428;&#xC744; &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center">HTML5</td>
    </tr>
    <tr>
      <td style="text-align:center"><code>cols</code>
      </td>
      <td style="text-align:center">number</td>
      <td style="text-align:center">&#xD14D;&#xC2A4;&#xD2B8; &#xC785;&#xB825; &#xC601;&#xC5ED; &#xC911; &#xBCF4;&#xC774;&#xB294;
        &#xC601;&#xC5ED;&#xC758; &#xB108;&#xBE44;&#xB97C; &#xBA85;&#xC2DC;.</td>
      <td
      style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>dirname</code>
      </td>
      <td style="text-align:center">textareaname.dir</td>
      <td style="text-align:center">
        <p>&#xD3FC; &#xB370;&#xC774;&#xD130;&#xAC00; &#xC11C;&#xBC84;&#xB85C; &#xC81C;&#xCD9C;&#xB420;
          &#xB54C; &#xC11C;&#xBC84;&#xB85C; &#xBCF4;&#xB0BC; &#xD14D;&#xC2A4;&#xD2B8;
          &#xC785;&#xB825; &#xC601;&#xC5ED;&#xC758; &#xD14D;&#xC2A4;&#xD2B8; &#xBC29;&#xD5A5;&#xC131;(text
          directionality)&#xC744; &#xC800;&#xC7A5;&#xD560; &#xC774;&#xB984;&#xC744;
          &#xBA85;&#xC2DC;.</p>
        <p>(&#xC5B8;&#xC81C;&#xB098; &#xC774;&#xB984; &#xB4A4;&#xC5D0; &#x201C;.dir&#x201D;&#xB97C;
          &#xCD94;&#xAC00;&#xD568;)</p>
      </td>
      <td style="text-align:center">HTML5</td>
    </tr>
    <tr>
      <td style="text-align:center"><code>disabled</code>
      </td>
      <td style="text-align:center">disabled</td>
      <td style="text-align:center">&#xD574;&#xB2F9;&lt;textarea&gt;&#xC694;&#xC18C;&#xAC00; &#xBE44;&#xD65C;&#xC131;&#xB428;&#xC744;
        &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>form</code>
      </td>
      <td style="text-align:center">form id</td>
      <td style="text-align:center">&#xD574;&#xB2F9; <code>&lt;texrarea&gt;</code> &#xC694;&#xC18C;&#xAC00;
        &#xD3EC;&#xD568;&#xB420; &#xD558;&#xB098; &#xC774;&#xC0C1;&#xC758; <code>&lt;form&gt;</code> &#xC694;&#xC18C;&#xB97C;
        &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center">HTML5</td>
    </tr>
    <tr>
      <td style="text-align:center"><code>maxlength</code>
      </td>
      <td style="text-align:center">number</td>
      <td style="text-align:center"><code>&lt;textarea&gt;</code> &#xC694;&#xC18C;&#xC5D0; &#xD5C8;&#xC601;&#xB418;&#xB294;
        &#xCD5C;&#xB300; &#xBB38;&#xC790;&#xC218;&#xB97C; &#xBA85;&#xC2DC;.</td>
      <td
      style="text-align:center">HTML5</td>
    </tr>
    <tr>
      <td style="text-align:center"> <code>name</code>
      </td>
      <td style="text-align:center">text</td>
      <td style="text-align:center"><code>&lt;textarea&gt;</code>&#xC694;&#xC18C;&#xC758; &#xC774;&#xB984;&#xC744;
        &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>placeholder</code>
      </td>
      <td style="text-align:center">text</td>
      <td style="text-align:center"><code>&lt;textarea&gt;</code>&#xC694;&#xC18C;&#xC758; &#xC785;&#xB825;&#xB420;
        &#xAC12;&#xC5D0; &#xB300;&#xD55C; &#xC9E7;&#xC740; &#xD78C;&#xD2B8;&#xB97C;
        &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center">HTML5</td>
    </tr>
    <tr>
      <td style="text-align:center"><code>readonly</code>
      </td>
      <td style="text-align:center">readonly</td>
      <td style="text-align:center"><code>&lt;textarea&gt;</code> &#xC694;&#xC18C;&#xC758; &#xD14D;&#xC2A4;&#xD2B8;
        &#xC785;&#xB825; &#xC601;&#xC5ED;&#xC774; &#xC77D;&#xAE30; &#xC804;&#xC6A9;&#xC784;&#xC744;
        &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>required</code>
      </td>
      <td style="text-align:center">required</td>
      <td style="text-align:center">&#xD3FC; &#xB370;&#xC774;&#xD130;&#xAC00; &#xC11C;&#xBC84;&#xB85C; &#xC81C;&#xCD9C;&#xB418;&#xAE30;
        &#xC804; &#xD14D;&#xC2A4;&#xD2B8; &#xC785;&#xB825; &#xC601;&#xC5ED;&#xC774;
        &#xBC18;&#xB4DC;&#xC2DC; &#xCC44;&#xC6CC;&#xC838; &#xC788;&#xC5B4;&#xC57C;
        &#xD568;&#xC744; &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center">HTML5</td>
    </tr>
    <tr>
      <td style="text-align:center"><code>rows</code>
      </td>
      <td style="text-align:center">number</td>
      <td style="text-align:center">&#xD14D;&#xC2A4;&#xD2B8; &#xC785;&#xB825; &#xC601;&#xC5ED; &#xC911; &#xBCF4;&#xC774;&#xB294;
        &#xC601;&#xC5ED;&#xC758; &#xB77C;&#xC778;&#xC218;&#xB97C; &#xBA85;&#xC2DC;.</td>
      <td
      style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>wrap</code>
      </td>
      <td style="text-align:center">
        <p>hard</p>
        <p>soft</p>
      </td>
      <td style="text-align:center">&#xD3FC; &#xB370;&#xC774;&#xD130;&#xAC00; &#xC11C;&#xBC84;&#xB85C; &#xC81C;&#xCD9C;&#xB420;
        &#xB54C; &#xC785;&#xB825;&#xB41C; &#xD14D;&#xC2A4;&#xD2B8;&#xC758; &#xC904;
        &#xBC14;&#xAFC8;&#xBC29;&#xC2DD;&#xC744; &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center">HTML5</td>
    </tr>
  </tbody>
</table>

#### 2\) TEXTAREA CSS STYLING

`<textarea>`는 기본적 으로 `display` 값은 block 이다.

다른 양식 요소와 비교하여 상자 모델,font, color 등 일반 CSS를 사용하여 쉽게 조작할 수 있다.

#### 📝**기준 불일치**

기준선을 설정하지 않으면 브라우저 마다 설정하는 기준선이 다르다. 그러므로 기준선은 예측할 수 없기  때문에 사용하지 않는게 났다.\(`vertical-align: baseline`\)

#### 📝**텍스트 영역의 크기 조정 가능 여부 제어**

대부분 브라우저에서 `<textarea>`는 크기를 조정할 수 있다.

페이지에 요소의 크기를 변경하는 데 사용할 수 있는 오른쪽 모서리에 드래그 핸들이 있다.

이는 `resize` CSS 속성에 의해 제어된다. 기본적으로 활성화 되어 있지만, 명시적으로 비활성화 할 수 있다.\(`none`\)

```css
textarea {
  resize: none;
}
```

#### 📝**유효하고 유효하지 않은 값 스타일 지정**

`<textarea>` 요소, 예를 들면 그와 설정 경계 여부 `minlength`, `maxlength` 또는 `required`를 사용하여 강조할 수 있다.

`:valid` 및 `:invalid` 가상 클래스, 예를 들면 텍스트 영역이 유효한지 또는 유효하지 않은 지 따라 테두리 값을 지정할 수 있다.

```css
textarea:invalid {
  border: 2px dashed red;
}

textarea:valid {
   border: 2px solid lime;
}
```

### 2. FIELDSET ELEMENT

`<fieldset>` 요소는 웹 양식의 컨트롤과 `<label>`을 묶을 때 사용한다.

#### 1\) FIELDSET CSS STYLING

`<fieldset>`는 기본적 으로 `display` 값은 block 이다.

`<fieldset>`은 기본 스타일로 콘텐츠를 감싸는 `2px` 너비의 groove 테두리, 작은 양의 내부 여백, 그리고 `min-inline-size: min-content`를 갖는다.

`<legend>` 요소는 `<fieldset>`의 블록 시작 방향\(대개 위쪽\) 테두리 위를 가로지르는 위치에 놓인다.

```markup
<form action="#">
  <fieldset>
    <legend>Simple fieldset</legend>
    <input type="radio" id="radio">
    <label for="radio">Spirit of radio</label>
  </fieldset>
</form>
```

### 3. LEGEND ELEMENT

`<legend>` 요소는 부모 `<fieldset>` 콘텐츠의 설명을 나타낸다.

### 4. DATALIST ELEMENT

`<datalist>` 요소는 다른 컨트롤에서 고를 수 있는 가능한, 혹은 추천하는 선택지를 나타내는 `<option>` 요소 여럿을 담는다.

### 5. PROGRESS ELEMENT

`<progress>` 요소는 어느 작업의 완료 정도를 나타내며, 주로 진행 표시줄의 형태로 띈다.

### 6. OUTPUT ELEMENT

`<output>` 요소는 웹 사이트나 앱에서 계산이나 사용자 행동의 결과를 삽입할 수 있는 컨트롤 데이터 요소 이다.

### 7. METE ELEMENT

`<meter>` 요소는 특정 범위 내에서 스칼라 값, 또는 백분율 값을 나타낸다.

### Reference 

textarea element [→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/textarea)

fieldset element [→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/fieldset)

legend element[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/legend)

datalist element[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/datalist)

progress element[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/progress)

output element[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/output)

meter element[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/meter)

Forms[ →HTML5.2 표준 기술 사양](https://html.spec.whatwg.org/multipage/forms.html#sec-forms)

Formspress - 폼 전송 test[ →\(SITE\)﻿](https://formspree.io/)

