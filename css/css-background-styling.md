# CSS backgrounds

### 1. BACKGROUND DESIGN

요소의 **배경\(background\)** 속성을 사용하면 **배경의 색상, 이미지, 위치, 반복, 고정 여부 등을 설정할** 수 있다. 그리고 모던 브라우저에서는 배경 이미지의 시작점\(origin\)을 조정하거나, 클리핑\(clipping\) 영역을 설정 할 수 있다.

요소의 배경이 지정된 공간은 요소의 `content-box`, `padding-box`, `border-box`까지 포함되고, 모던 브라우저에서는 배경을 차지하는 영역을 `background-clip` 속성을 사용하여 변경할 수 있다.



<table>
  <thead>
    <tr>
      <th style="text-align:center">property name</th>
      <th style="text-align:center">description</th>
      <th style="text-align:center">spec</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:center">background-color</td>
      <td style="text-align:center">HTML &#xC694;&#xC18C;&#xC758; &#xBC30;&#xACBD;&#xC0C9; &#xC124;&#xC815;.
        (default : <code>transparent</code>)</td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>action</code>
      </td>
      <td style="text-align:center">&#xD3FC; &#xB370;&#xC774;&#xD130;&#xAC00; &#xC11C;&#xBC84;&#xB85C; &#xC81C;&#xCD9C;&#xB420;
        &#xB54C; &#xD574;&#xB2F9; &#xB370;&#xC774;&#xD130;&#xAC00; &#xB3C4;&#xCC29;&#xD560;
        URL&#xC744; &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>autocomplete</code>
      </td>
      <td style="text-align:center"><code>&lt;form&gt;</code> &#xC694;&#xC18C;&#xC758; &#xC790;&#xB3D9; &#xC644;&#xC131;
        &#xAE30;&#xB2A5;&#xC744; &#xC0AC;&#xC6A9;&#xD558;&#xC9C0; &#xC5EC;&#xBD80;&#xB97C;
        &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center">HTML5</td>
    </tr>
    <tr>
      <td style="text-align:center"><code>enctype</code>
      </td>
      <td style="text-align:center">
        <p>&#xD3FC; &#xB370;&#xC774;&#xD130;&#xAC00; &#xC11C;&#xBC84;&#xB85C; &#xC81C;&#xCD9C;&#xB420;
          &#xB54C; &#xD574;&#xB2F9; &#xB370;&#xC774;&#xD130;&#xAC00; &#xC778;&#xCF54;&#xB529;
          &#xB418;&#xB294; &#xBC29;&#xBC95;&#xC744;&#xBA85;&#xC2DC;.</p>
        <p>(&#xB2E8;, <code>&lt;form&gt;</code>&#xC694;&#xC18C;&#xC758; method &#xC18D;&#xC131;&#xAC12;&#xC774;
          post &#xC778; &#xACBD;&#xC6B0;&#xC5D0;&#xB9CC; &#xC0AC;&#xC6A9;&#xD560;
          &#xC218; &#xC788;&#xB2E4;.)</p>
      </td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>method</code>
      </td>
      <td style="text-align:center">&#xD3FC; &#xB370;&#xC774;&#xD130;&#xAC00; &#xC11C;&#xBC84;&#xB85C; &#xC81C;&#xCD9C;&#xB420;
        &#xB54C; &#xC0AC;&#xC6A9;&#xB418;&#xB294; HTTP method&#xB97C; &#xBA85;&#xC2DC;.</td>
      <td
      style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>name</code>
      </td>
      <td style="text-align:center"><code>&lt;form&gt;</code> &#xC694;&#xC18C;&#xC758; &#xC774;&#xB984;&#xC744;
        &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center">HTML5</td>
    </tr>
    <tr>
      <td style="text-align:center"><code>novaildate</code>
      </td>
      <td style="text-align:center">&#xD3FC; &#xB370;&#xC774;&#xD130;&#xAC00; &#xC11C;&#xBC84;&#xB85C; &#xC81C;&#xCD9C;&#xB420;
        &#xB54C; &#xD574;&#xB2F9; &#xB370;&#xC774;&#xD130;&#xC758; &#xC720;&#xD6A8;&#xC131;&#xC744;
        &#xAC80;&#xC0AC;&#xD558;&#xC9C0; &#xC54A;&#xC74C;&#xC744; &#xBA85;&#xC2DC;</td>
      <td
      style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>target</code>
      </td>
      <td style="text-align:center"></td>
      <td style="text-align:center"></td>
    </tr>
  </tbody>
</table>

#### 1\) background-color 

HTML 요소의 배경색 설정. \(default : `transparent`\)

#### 2\) background-image

HTML요소의 배경으로 나타날 배경 이미지를 설정. \(default :  `none`\)

#### 3\) background-position

이 속성은 **반복되지 않는 배경 이미지의 상대 위치\(relative position\)를 설정**. \(default : `left top`\)

#### 4\) background-repeat

배경 이미지는 기본 설정으로 수평과 수직 방향으로 모두 반복되어 나타난다. 이 속성을 이용하면 이러한 배경 이미지를 수평이나 수직 방향으로만 반복되도록 설정. \(default : `repeat`\)

#### 5\) background-attachment

이 속성을 사용하여 위치가 설정된 배경 이미지를 해당 위치에 고정시킬 수도 있다. 이렇게 고정된 배경이미지는 스크롤과 무관하게 화면의 위치에서 이동하지 않는다. \(default : `scroll`\)

#### 6\) background

**위에 적은 5가지 배경 속성을 모아 작성하는 속기법.**

#### 7\) background-size

배경 이미지의 크기를 동적으로 조정하여 설정. \(default : `auto`\)

#### 8\) background-clip

배경 이미지를 클리핑 하는 영역을 설정. \(default : `border-box`\)

#### 9\) background-origin

배경 이미지의 시작 위치를 특정 영역으로 설정. \(default : `padding-box`\)







