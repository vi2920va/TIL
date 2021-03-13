---
description: 'BOBY : script, noscript elements'
---

# 스크립팅 요소들

### 1.  &lt;script&gt; element

JavaScript 코드 또는 파일을 HTML 문서에 작성하거나, 연결할 때 사용한다.

#### 1\) &lt;script&gt; element - attributes

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
      <td style="text-align:center"><code>async</code>
      </td>
      <td style="text-align:center">async</td>
      <td style="text-align:center">
        <p>&#xC2A4;&#xD06C;&#xB9BD;&#xD2B8;&#xAC00; &#xBE44;&#xB3D9;&#xAE30;&#xC801;&#xC73C;&#xB85C;
          &#xC2E4;&#xD589;&#xB428;&#xC744; &#xBA85;&#xC2DC;.</p>
        <p>(&lt;script&gt; &#xC694;&#xC18C;&#xAC00; &#xC678;&#xBD80; &#xC2A4;&#xD06C;&#xB9BD;&#xD2B8;&#xB97C;
          &#xCC38;&#xC870;&#xD558;&#xB294; &#xACBD;&#xC6B0;&#xC5D0;&#xB9CC; &#xC0AC;&#xC6A9;&#xD560;
          &#xC218; &#xC788;&#xB2E4;.)</p>
      </td>
      <td style="text-align:center">HTML5</td>
    </tr>
    <tr>
      <td style="text-align:center"><code>charset</code>
      </td>
      <td style="text-align:center">character set</td>
      <td style="text-align:center">
        <p>&#xC678;&#xBD80; &#xC2A4;&#xD06C;&#xB9BD;&#xD2B8; &#xD30C;&#xC77C;&#xC5D0;&#xC11C;
          &#xC0AC;&#xC6A9;&#xB418;&#xB294; &#xBB38;&#xC790; &#xC778;&#xCF54;&#xB529;
          &#xBC29;&#xC2DD;&#xC744; &#xBA85;&#xC2DC;.</p>
        <p>(&lt;script&gt; &#xC694;&#xC18C;&#xAC00; &#xC678;&#xBD80; &#xC2A4;&#xD06C;&#xB9BD;&#xD2B8;&#xB97C;
          &#xCC38;&#xC870;&#xD558;&#xB294; &#xACBD;&#xC6B0;&#xC5D0;&#xB9CC; &#xC0AC;&#xC6A9;&#xD560;
          &#xC218; &#xC788;&#xB2E4;.)</p>
      </td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>defer</code>
      </td>
      <td style="text-align:center">defer</td>
      <td style="text-align:center">
        <p>&#xD398;&#xC774;&#xC9C0; &#xD30C;&#xC2F1;&#xC774; &#xBAA8;&#xB450; &#xB05D;&#xB098;&#xBA74;
          &#xC2A4;&#xD06C;&#xB9BD;&#xD2B8;&#xAC00; &#xC2E4;&#xD589;&#xB428;&#xC744;
          &#xBA85;&#xC2DC;.</p>
        <p>(&lt;script&gt; &#xC694;&#xC18C;&#xAC00; &#xC678;&#xBD80; &#xC2A4;&#xD06C;&#xB9BD;&#xD2B8;&#xB97C;
          &#xCC38;&#xC870;&#xD558;&#xB294; &#xACBD;&#xC6B0;&#xC5D0;&#xB9CC; &#xC0AC;&#xC6A9;&#xD560;
          &#xC218; &#xC788;&#xB2E4;.)</p>
      </td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>src</code>
      </td>
      <td style="text-align:center">URL</td>
      <td style="text-align:center">&#xC678;&#xBD80; &#xC2A4;&#xD06C;&#xB9BD;&#xD2B8; &#xD30C;&#xC77C;&#xC758;
        URL&#xC744; &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>type</code>
      </td>
      <td style="text-align:center">media type</td>
      <td style="text-align:center">&#xC2A4;&#xD06C;&#xB9BD;&#xD2B8;&#xC758; &#xBBF8;&#xB514;&#xC5B4; &#xD0C0;&#xC785;&#xC744;
        &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center"></td>
    </tr>
  </tbody>
</table>

```markup
<script src="js/app.js"></script>
```

### 2. &lt;noscript&gt; element

사용자의 웹 브라우저 환경에서 스크립트를 지원되지 않거나, 스크립트가 꺼져있는 경우, 문서에 표시될 문구를 삽입한다.

```markup
<noscript>
    <p>JavaScript를 지원하지 않습니다.</p>
</noscript>

```



