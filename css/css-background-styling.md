# CSS backgrounds

### 1. BACKGROUND DESIGN

요소의 **배경\(background\)** 속성을 사용하면 **배경의 색상, 이미지, 위치, 반복, 고정 여부 등을 설정할** 수 있다. 그리고 모던 브라우저에서는 배경 이미지의 시작점\(origin\)을 조정하거나, 클리핑\(clipping\) 영역을 설정 할 수 있다.

요소의 배경이 지정된 공간은 요소의 `content-box`, `padding-box`, `border-box`까지 포함되고, 모던 브라우저에서는 배경을 차지하는 영역을 `background-clip` 속성을 사용하여 변경할 수 있다.

#### 1\) backgrounds property

배경과 관련된 속성들.

<table>
  <thead>
    <tr>
      <th style="text-align:center">property name</th>
      <th style="text-align:center">
        <p>default</p>
        <p>value</p>
      </th>
      <th style="text-align:center">description</th>
      <th style="text-align:center">spec</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:center"> <code>background-color</code>
      </td>
      <td style="text-align:center"><code>transparent</code>
      </td>
      <td style="text-align:center">HTML &#xC694;&#xC18C;&#xC758; &#xBC30;&#xACBD;&#xC0C9; &#xC124;&#xC815;.</td>
      <td
      style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>background-image</code>
      </td>
      <td style="text-align:center"><code>none</code>
      </td>
      <td style="text-align:center">HTML&#xC694;&#xC18C;&#xC758; &#xBC30;&#xACBD;&#xC73C;&#xB85C; &#xB098;&#xD0C0;&#xB0A0;
        &#xBC30;&#xACBD; &#xC774;&#xBBF8;&#xC9C0;&#xB97C; &#xC124;&#xC815;.</td>
      <td
      style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>background-position</code>
      </td>
      <td style="text-align:center"><code>left top</code>
      </td>
      <td style="text-align:center">&#xBC18;&#xBCF5;&#xB418;&#xC9C0; &#xC54A;&#xB294; &#xBC30;&#xACBD; &#xC774;&#xBBF8;&#xC9C0;&#xC758;
        &#xC0C1;&#xB300; &#xC704;&#xCE58;(relative position)&#xB97C; &#xC124;&#xC815;.</td>
      <td
      style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>background-repeat</code>
      </td>
      <td style="text-align:center"><code>repeat</code>
      </td>
      <td style="text-align:center">&#xBC30;&#xACBD; &#xC774;&#xBBF8;&#xC9C0;&#xB294; &#xAE30;&#xBCF8; &#xC124;&#xC815;&#xC73C;&#xB85C;
        &#xC218;&#xD3C9;&#xACFC; &#xC218;&#xC9C1; &#xBC29;&#xD5A5;&#xC73C;&#xB85C;
        &#xBAA8;&#xB450; &#xBC18;&#xBCF5;&#xB418;&#xC5B4; &#xB098;&#xD0C0;&#xB09C;&#xB2E4;.
        &#xC774; &#xC18D;&#xC131;&#xC744; &#xC774;&#xC6A9;&#xD558;&#xBA74; &#xC774;&#xB7EC;&#xD55C;
        &#xBC30;&#xACBD; &#xC774;&#xBBF8;&#xC9C0;&#xB97C; &#xC218;&#xD3C9;&#xC774;&#xB098;
        &#xC218;&#xC9C1; &#xBC29;&#xD5A5;&#xC73C;&#xB85C;&#xB9CC; &#xBC18;&#xBCF5;&#xB418;&#xB3C4;&#xB85D;
        &#xC124;&#xC815;.</td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>background-attachment</code>
      </td>
      <td style="text-align:center"><code>scroll</code>
      </td>
      <td style="text-align:center">&#xC704;&#xCE58;&#xAC00; &#xC124;&#xC815;&#xB41C; &#xBC30;&#xACBD; &#xC774;&#xBBF8;&#xC9C0;&#xB97C;
        &#xD574;&#xB2F9; &#xC704;&#xCE58;&#xC5D0; &#xACE0;&#xC815;&#xC2DC;&#xD0AC;
        &#xC218;&#xB3C4; &#xC788;&#xB2E4;. &#xC774;&#xB807;&#xAC8C; &#xACE0;&#xC815;&#xB41C;
        &#xBC30;&#xACBD;&#xC774;&#xBBF8;&#xC9C0;&#xB294; &#xC2A4;&#xD06C;&#xB864;&#xACFC;
        &#xBB34;&#xAD00;&#xD558;&#xAC8C; &#xD654;&#xBA74;&#xC758; &#xC704;&#xCE58;&#xC5D0;&#xC11C;
        &#xC774;&#xB3D9;&#xD558;&#xC9C0; &#xC54A;&#xB294;&#xB2E4;.</td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>background</code>
      </td>
      <td style="text-align:center"></td>
      <td style="text-align:center">&#xC704;&#xC5D0; &#xC788;&#xB294; 5&#xAC00;&#xC9C0; &#xBC30;&#xACBD; &#xC18D;&#xC131;&#xC744;
        &#xBAA8;&#xC544; &#xC791;&#xC131;&#xD558;&#xB294; &#xC18D;&#xAE30;&#xBC95;<b>.</b>
      </td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>background-size</code>
      </td>
      <td style="text-align:center"><code>auto</code>
      </td>
      <td style="text-align:center">&#xBC30;&#xACBD; &#xC774;&#xBBF8;&#xC9C0;&#xC758; &#xD06C;&#xAE30;&#xB97C;
        &#xB3D9;&#xC801;&#xC73C;&#xB85C; &#xC870;&#xC815;&#xD558;&#xC5EC; &#xC124;&#xC815;.</td>
      <td
      style="text-align:center">CSS 3</td>
    </tr>
    <tr>
      <td style="text-align:center"><code>background-clip</code>
      </td>
      <td style="text-align:center"><code>border-box</code>
      </td>
      <td style="text-align:center">&#xBC30;&#xACBD; &#xC774;&#xBBF8;&#xC9C0;&#xB97C; &#xD074;&#xB9AC;&#xD551;
        &#xD558;&#xB294; &#xC601;&#xC5ED;&#xC744; &#xC124;&#xC815;.</td>
      <td style="text-align:center">CSS 3</td>
    </tr>
    <tr>
      <td style="text-align:center"><code>background-origin</code>
      </td>
      <td style="text-align:center"><code>padding-box</code>
      </td>
      <td style="text-align:center">&#xBC30;&#xACBD; &#xC774;&#xBBF8;&#xC9C0;&#xC758; &#xC2DC;&#xC791; &#xC704;&#xCE58;&#xB97C;
        &#xD2B9;&#xC815; &#xC601;&#xC5ED;&#xC73C;&#xB85C; &#xC124;&#xC815;.</td>
      <td
      style="text-align:center">CSS 3</td>
    </tr>
  </tbody>
</table>



+++





