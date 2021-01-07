# BOBY : embeded elements

### 1. EMBEDED ELEMENTS

HTML 문서에 끼워 넣는\(embeded\) 이미지, 비디오, 웹 사이트, 이미지맵, SVG 벡터 그래픽 같은 콘텐츠 요소들

#### 1\) IMG ELEMENT

HTML 문서에 이미지를 포함\(링크\)

#### ① IMG ELEMENT -  ATTRIBUTES

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
      <td style="text-align:center"><code>crossorigin</code>
      </td>
      <td style="text-align:center">
        <p>anonymous</p>
        <p>use-credentials</p>
      </td>
      <td style="text-align:center">&lt;canvas&gt;&#xC694;&#xC18C;&#xC5D0; &#xC0AC;&#xC6A9;&#xB420; &#xC774;&#xBBF8;&#xC9C0;&#xC5D0;
        &#xAD50;&#xCC28; &#xCD9C;&#xCC98; &#xC811;&#xADFC;&#xC744; &#xD5C8;&#xC6A9;&#xD558;&#xB294;
        &#xC81C;3&#xC758; &#xC0AC;&#xC774;&#xD2B8;&#xB85C; &#xBD80;&#xD130;&#xC758;
        &#xC774;&#xBBF8;&#xC9C0; &#xD5C8;&#xC6A9; &#xC5EC;&#xBD80;&#xB97C; &#xBA85;&#xC2DC;.</td>
      <td
      style="text-align:center">HTML5</td>
    </tr>
    <tr>
      <td style="text-align:center"><code>height</code>
      </td>
      <td style="text-align:center">px</td>
      <td style="text-align:center">&#xC774;&#xBBF8;&#xC9C0; &#xB192;&#xC774;&#xB97C; &#xBA85;&#xC2DC;.</td>
      <td
      style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>ismap</code>
      </td>
      <td style="text-align:center">ismap</td>
      <td style="text-align:center">&#xD574;&#xB2F9; &#xC774;&#xBBF8;&#xC9C0;&#xAC00; &#xC11C;&#xBC84; &#xC0AC;&#xC774;&#xB4DC;
        &#xC774;&#xBBF8;&#xC9C0;&#xB9F5;&#xC758; &#xC77C;&#xBD80;&#xC778;&#xC9C0;
        &#xC5EC;&#xBD80;&#xB97C; &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>longesc</code>
      </td>
      <td style="text-align:center">URL</td>
      <td style="text-align:center">&#xC774;&#xBBF8;&#xC9C0;&#xC5D0; &#xB300;&#xD55C; &#xBD80;&#xAC00;&#xC801;&#xC778;
        &#xC124;&#xBA85;&#xC744; &#xC81C;&#xACF5;&#xD558;&#xB294; URL&#xB97C; &#xBA85;&#xC2DC;.</td>
      <td
      style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>sizes</code>
      </td>
      <td style="text-align:center">text</td>
      <td style="text-align:center">&#xC11C;&#xB85C; &#xB2E4;&#xB978; &#xD398;&#xC774;&#xC9C0; &#xB808;&#xC774;&#xC544;&#xC6C3;&#xC5D0;
        &#xB300;&#xD55C; &#xC774;&#xBBF8;&#xC9C0; &#xC18C;&#xC2A4;&#xC758; &#xD06C;&#xAE30;&#xB97C;
        &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>src</code>
      </td>
      <td style="text-align:center">URL</td>
      <td style="text-align:center">&#xC774;&#xBBF8;&#xC9C0; &#xC18C;&#xC2A4;&#xC758; URL&#xC744; &#xBA85;&#xC2DC;.</td>
      <td
      style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>srcset</code>
      </td>
      <td style="text-align:center">text</td>
      <td style="text-align:center">&#xAC01;&#xAC01; &#xB2E4;&#xB978; &#xD658;&#xACBD;&#xC5D0;&#xC11C; &#xC0AC;&#xC6A9;&#xB420;
        &#xC774;&#xBBF8;&#xC9C0; &#xC18C;&#xC2A4;&#xB97C; &#xBA85;&#xC2DC;.</td>
      <td
      style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>alt</code>
      </td>
      <td style="text-align:center">text</td>
      <td style="text-align:center">&#xC774;&#xBBF8;&#xC9C0;&#xB97C; &#xAC00;&#xC838;&#xC624;&#xB294;&#xB370;
        &#xC2E4;&#xD328;&#xD588;&#xC744; &#xACBD;&#xC6B0; &#xBCF4;&#xC5EC;&#xC904;
        &#xB300;&#xCCB4; &#xD14D;&#xC2A4;&#xD2B8;&#xB97C; &#xBA85;&#xC2DC;.</td>
      <td
      style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>width</code>
      </td>
      <td style="text-align:center">px</td>
      <td style="text-align:center">&#xC774;&#xBBF8;&#xC9C0; &#xB108;&#xBE44;&#xB97C; &#xBA85;&#xC2DC;.</td>
      <td
      style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>usemap</code>
      </td>
      <td style="text-align:center">#map name</td>
      <td style="text-align:center">&#xD074;&#xB77C;&#xC774;&#xC5B8;&#xD2B8; &#xC0AC;&#xC774;&#xB4DC; &#xC774;&#xBBF8;&#xC9C0;
        &#xB9F5;&#xC73C;&#xB85C; &#xC774;&#xBBF8;&#xC9C0;&#xB97C; &#xBA85;&#xC2DC;</td>
      <td
      style="text-align:center"></td>
    </tr>
  </tbody>
</table>



#### 2\) PICTURE ELEMENT 

`<picture>`요소는 다양한 스크린 환경\(스마트폰, 데스크탑, TV 등\)에 맞는 이미지를 화면에 적절하게 표시해 주기 위해 사용한다. 이 요소를 사용할 때에는 1개 이상의 `<img>`를 포함하는 요소와 `<picture>`요소의 자식으로 0개 이상의`<source>`요소가 필요에 따라 사용할 수 있다.

`<source>`요소를 사용할 수 없을 경우에는 `<img>`요소가 화면에 표시하게 된다.

```markup
<!-- source attribute : media -->
<picture>
  <source srcset="bamboo-pen.png" media="(min-width: 600px)">
  <img src="bamboo-pen-narrow.png" alt="Bamboo Pen">
</picture>

<!-- source attribute : type -->     
<picture>
  <source srcset="bamboo-pen.svg" type="image/svg+xml">
  <img src="bamboo-pen-narrow.png" alt="Bamboo Pen">
</picture>
```

#### 3\) SOURCE ELEMENT 

`<picture>, <audio>, <video>` 요소의 다중 미디어 리소스를 지정하기 위해 사용

```markup
<video src="videofile.mp4" poster="posterimage.jpg" controls>
	<source src="videofile.webm" type="video/webm">
	<source src="videofile.ogg" type="video/ogg">
	<source src="videofile.mov" type="video/quicktime">
	HTML5 <code>video</code> 요소를 지원하지 않는 구형 웹 브라우저를 사용 중입니다.
	<a href="http://outdatedbrowser.com/ko">최신형 브라우저로 업데이트</a> 하세요.
</video>
```

#### 4\) VIDEO ELEMENT 

동영상 콘텐츠를 HTML 문서에 포함하기 위해서 사용한다. src 속성이나 `<socurce>`요소를 이용해 여러 개의 동영상 소소 중 하나를 표시.

#### ① VIDEO ELEMENT - ATTRIBUTES

<table>
  <thead>
    <tr>
      <th style="text-align:left">attribute</th>
      <th style="text-align:center">attribute value</th>
      <th style="text-align:center">description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><code>src</code>
      </td>
      <td style="text-align:center">URL</td>
      <td style="text-align:center">&#xBE44;&#xB514;&#xC624; &#xD30C;&#xC77C;&#xC758; &#xC704;&#xCE58;(URL)&#xC744;
        &#xBA85;&#xC2DC;.</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>poster</code>
      </td>
      <td style="text-align:center">URL</td>
      <td style="text-align:center">&#xBE44;&#xB514;&#xC624;&#xB97C; &#xB2E4;&#xC6B4;&#xB85C;&#xB4DC; &#xD558;&#xB294;
        &#xB3D9;&#xC548;&#xC774;&#xB098; &#xC0AC;&#xC6A9;&#xC790;&#xAC00; &#xC7AC;&#xC0C1;
        &#xBC84;&#xD2BC;&#xC744; &#xB204;&#xB97C; &#xB54C; &#xAE4C;&#xC9C0; &#xD45C;&#xC2DC;&#xD560;
        &#xC774;&#xBBF8;&#xC9C0;&#xB97C; &#xBA85;&#xC2DC;.</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>preload</code>
      </td>
      <td style="text-align:center">
        <p>auto</p>
        <p>metadata none</p>
      </td>
      <td style="text-align:center">&#xD398;&#xC774;&#xC9C0;&#xAC00; &#xB85C;&#xB4DC; &#xB420; &#xB54C; &#xC624;&#xB514;&#xC624;
        &#xD30C;&#xC77C;&#xC774; &#xAC19;&#xC774; &#xB85C;&#xB4DC;&#xB418;&#xC5B4;&#xC57C;
        &#xD558;&#xB294;&#xC9C0; &#xC5EC;&#xBD80;&#xC640; &#xADF8; &#xBC29;&#xBC95;&#xC744;
        &#xBA85;&#xC2DC;.</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>controls</code>
      </td>
      <td style="text-align:center">control</td>
      <td style="text-align:center">&#xD50C;&#xB808;&#xC774; &#xBC84;&#xD2BC;&#xC774;&#xB098; &#xC815;&#xC9C0;
        &#xBC84;&#xD2BC;&#xACFC; &#xAC19;&#xC774; &#xBE44;&#xB514;&#xC624;&#xC758;
        &#xC2E4;&#xD589;&#xC744; &#xC81C;&#xC5B4;&#xD560; &#xC218; &#xC788;&#xB294;
        &#xC81C;&#xC5B4;&#xAE30;&#xAC00; &#xD45C;&#xC2DC;&#xB428;&#xC744; &#xBA85;&#xC2DC;.</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>autoplay</code>
      </td>
      <td style="text-align:center">autoplay</td>
      <td style="text-align:center">&#xBE44;&#xB514;&#xC624;&#xAC00; &#xC2E4;&#xD589;&#xB420; &#xC900;&#xBE44;&#xAC00;
        &#xB05D;&#xB098;&#xB294; &#xB300;&#xB85C; &#xC790;&#xB3D9;&#xC73C;&#xB85C;
        &#xC2E4;&#xD589;&#xB428;&#xC744; &#xBA85;&#xC2DC;.</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>loop</code>
      </td>
      <td style="text-align:center">loop</td>
      <td style="text-align:center">&#xBE44;&#xB514;&#xC624;&#xAC00; &#xC7AC;&#xC0DD;&#xC774; &#xB05D;&#xB098;&#xBA74;
        &#xB610;&#xB2E4;&#xC2DC; &#xC7AC;&#xC0DD;&#xB428;&#xC744; &#xBA85;&#xC2DC;.</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>muted</code>
      </td>
      <td style="text-align:center">muted</td>
      <td style="text-align:center">&#xBE44;&#xB514;&#xC624;&#xC758; &#xC74C;&#xC131; &#xCD9C;&#xB825;&#xC774;
        &#xC74C;&#xC18C;&#xAC70;&#xB428;&#xC744; &#xBA85;&#xC2DC;.</td>
    </tr>
  </tbody>
</table>

```markup
<video src="videofile.mp4" poster="posterimage.jpg">
	HTML5 <code>video</code> 요소를 지원하지 않는 구형 웹 브라우저를 사용 중입니다.
	<a href="http://outdatedbrowser.com/ko">최신형 브라우저로 업데이트</a> 하세요.
</video>
```

#### 5\) AUDIO ELEMENT 

`<audio>`요소도 `<video>`요소와 유사하게 사용된다.

#### ① AUDIO ELEMENT - ATTRIBUTES

<table>
  <thead>
    <tr>
      <th style="text-align:left">attribute</th>
      <th style="text-align:left">attribute value</th>
      <th style="text-align:left">description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><code>src</code>
      </td>
      <td style="text-align:left">URL</td>
      <td style="text-align:left">&#xC624;&#xB514;&#xC624; &#xD30C;&#xC77C;&#xC758; &#xC704;&#xCE58;(URL)&#xB97C;
        &#xBA85;&#xC2DC;.</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>muted</code>
      </td>
      <td style="text-align:left">muted</td>
      <td style="text-align:left">&#xC624;&#xB514;&#xC624;&#xC758; &#xC74C;&#xC131; &#xCD9C;&#xB825;&#xC774;
        &#xC74C;&#xC18C;&#xAC70;&#xB428;&#xC744; &#xBA85;&#xC2DC;.</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>preload</code>
      </td>
      <td style="text-align:left">
        <p>auto</p>
        <p>metadata none</p>
      </td>
      <td style="text-align:left">&#xD398;&#xC774;&#xC9C0;&#xAC00; &#xB85C;&#xB4DC;&#xB420; &#xB54C; &#xC624;&#xB514;&#xC624;
        &#xD30C;&#xC77C;&#xC774; &#xAC19;&#xC774; &#xB85C;&#xB4DC;&#xB418;&#xC5B4;&#xC57C;
        &#xD558;&#xB294;&#xC9C0; &#xC5EC;&#xBD80;&#xC640; &#xADF8; &#xBC29;&#xBC95;&#xC744;
        &#xBA85;&#xC2DC;.</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>controls</code>
      </td>
      <td style="text-align:left">controls</td>
      <td style="text-align:left">&#xD50C;&#xB808;&#xC774; &#xBC84;&#xD2BC;&#xC774;&#xB098; &#xC815;&#xC9C0;
        &#xBC84;&#xD2BC;&#xACFC; &#xAC19;&#xC774; &#xC624;&#xB514;&#xC624;&#xC758;
        &#xC2E4;&#xD589;&#xC744; &#xC81C;&#xC5B4;&#xD560;&#xC218; &#xC788;&#xB294;
        &#xC81C;&#xC5B4;&#xAE30;&#xAC00; &#xD45C;&#xC2DC;&#xB428;&#xC744; &#xBA85;&#xC2DC;.</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>autoplay</code>
      </td>
      <td style="text-align:left">autoplay</td>
      <td style="text-align:left">&#xC624;&#xB514;&#xC624;&#xAC00; &#xC2E4;&#xD589;&#xB420; &#xC900;&#xBE44;&#xAC00;
        &#xB05D;&#xB098;&#xB294; &#xB300;&#xB85C; &#xC790;&#xB3D9;&#xC73C;&#xB85C;
        &#xC2E4;&#xD589;&#xB428;&#xC744; &#xBA85;&#xC2DC;.</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>loop</code>
      </td>
      <td style="text-align:left">loop</td>
      <td style="text-align:left">&#xC624;&#xB514;&#xC624;&#xC758; &#xC7AC;&#xC0DD;&#xC774; &#xB05D;&#xB098;&#xBA74;
        &#xC790;&#xB3D9;&#xC73C;&#xB85C; &#xB610;&#xB2E4;&#xC2DC; &#xC7AC;&#xC0DD;&#xB428;&#xC744;
        &#xBA85;&#xC2DC;.</td>
    </tr>
  </tbody>
</table>

```markup
<audio src="audiofile.mp3">
	HTML5 <code>audio</code> 요소를 지원하지 않는 구형 웹 브라우저를 사용 중입니다.
	<a href="http://outdatedbrowser.com/ko">최신형 브라우저로
		업데이트</a>로 업데이트 하세요.
</audio>
```

#### 6\) TRACK ELEMENT 

`<track>`요소는 비디오 또는 오디오 재생 시에 자막을 표시하도록 해주는 요소로 `default`속성을 설정하지 않을 경우에는 자막을 사용 하지 않는다.

```markup
<video src="videofile.mp4" poster="posterimage.jpg">
	<track kind="subtitles" src="videofile.ko.vtt" srclang="ko" label="한국어" default>
	<track kind="subtitles" src="videofile.en.vtt" srclang="en" label="English">
</video>

<audio src="audiofile.mp3">
	<track kind="subtitles" src="audiofile.ko.vtt" srclang="ko" label="한국어">
	<track kind="subtitles" src="audiofile.en.vtt" srclang="en" label="English">
</audio>
```

#### 7\) IFRAME ELEMENT 

인라인 프레임\(inline frame\)에 다른 HTML 페이지를 포함하여 화면에 표시.

#### ①  IFRAME ELEMENT - ATTRIBUTES

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
      <td style="text-align:center"><code>src</code>
      </td>
      <td style="text-align:center">URL</td>
      <td style="text-align:center">&#xC694;&#xC18C;&#xC5D0; &#xBCF4;&#xC77C; &#xBB38;&#xC11C;&#xC758; URL&#xB97C;
        &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>width</code>
      </td>
      <td style="text-align:center">px</td>
      <td style="text-align:center">&lt;iframe&gt;&#xC694;&#xC18C;&#xC758; &#xB108;&#xBE44;&#xB97C; &#xBA85;&#xC2DC;.</td>
      <td
      style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>height</code>
      </td>
      <td style="text-align:center">px</td>
      <td style="text-align:center">&lt;iframe&gt;&#xC694;&#xC18C;&#xC758; &#xB192;&#xC774;&#xB97C; &#xBA85;&#xC2DC;.</td>
      <td
      style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>name</code>
      </td>
      <td style="text-align:center">text</td>
      <td style="text-align:center">&lt;iframe&gt;&#xC694;&#xC18C;&#xC758; &#xC774;&#xB984;&#xC744; &#xBA85;&#xC2DC;.</td>
      <td
      style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>sandbox</code>
      </td>
      <td style="text-align:center">
        <p>allow-forms</p>
        <p>allow-pointer-lock</p>
        <p>allow-popups</p>
        <p>allow-same-origin</p>
        <p>allow-scripts</p>
        <p>allow-top-navigation</p>
      </td>
      <td style="text-align:center"><code>&lt;frame&gt;</code>&#xC694;&#xC18C;&#xC5D0; &#xBCF4;&#xC77C; &#xCF58;&#xD150;&#xCE20;&#xC5D0;
        &#xB300;&#xD55C; &#xCD94;&#xAC00;&#xC801;&#xC778; &#xC81C;&#xD55C; &#xC0AC;&#xD56D;(restrictions)&#xB4E4;&#xC758;
        &#xC9D1;&#xD569;&#xC744; &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center">HTML5</td>
    </tr>
    <tr>
      <td style="text-align:center"><code>srcdoc</code>
      </td>
      <td style="text-align:center">html code</td>
      <td style="text-align:center"><code>&lt;frame&gt;</code> &#xC694;&#xC18C;&#xC5D0; &#xBCF4;&#xC77C; &#xC6F9;
        &#xD398;&#xC774;&#xC9C0;&#xC758; HTML &#xCF54;&#xB4DC;&#xB97C; &#xBA85;&#xC2DC;.</td>
      <td
      style="text-align:center">HTML5</td>
    </tr>
  </tbody>
</table>

```markup
<iframe width="560" height="315" src="https://www.youtube.com/embed/0wlXaHmmOVc?rel=0&amp;showinfo=0"
	allow="autoplay; encrypted-media" allowfullscreen></iframe>

<iframe
	src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d12643.636820892792!2d127.01610674058901!3d37.60429582641849!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x357cbc91e5ca4f03%3A0x18820a16e406c8ea!2z7ISc7Jq47Yq567OE7IucIOyEseu2geq1rCDquLjsnYwx64-ZIDUzMC0zNg!5e0!3m2!1sko!2skr!4v1520001155674"
	width="600" height="450" style="border: 0" allowfullscreen></iframe>
```

#### 8\) MAP ELEMENT 

이미지 맵\(클릭 가능한 링크 영역\)을 정의하기 위해 `<area>`요소와 함께 사용한다.

```markup
<img src="products-map.jpg" alt="제품 모음" usemap="#products-map">
<map name="products-map">
	<area shape="circle" coords="200,250,25" hreflang="en-GB" href="another.html" alt="Another Page" target="_blank">
</map>
```

#### 9\) AREA ELEMENT 

이미지의 핫스팟 지역 정의, 하이퍼링크 설정, `<map>`요소 내부에서만 사용 가능하다.

#### ①  AREA ELEMENT - ATTRIBUTES

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
      <td style="text-align:center"><code>rel</code>
      </td>
      <td style="text-align:center">
        <p>alternate</p>
        <p>author bookmark</p>
        <p>help</p>
        <p>license</p>
        <p>next</p>
        <p>nofollow noreferrer</p>
        <p>prefetch prev</p>
        <p>search</p>
        <p>tag</p>
      </td>
      <td style="text-align:center">&#xD604;&#xC7AC; &#xBB38;&#xC11C;&#xC640; &#xB300;&#xC0C1;&#xC758; URL
        &#xC0AC;&#xC774;&#xC758; &#xC5F0;&#xAD00; &#xAD00;&#xACC4;&#xB97C; &#xBA85;&#xC2DC;.</td>
      <td
      style="text-align:center">HTML5</td>
    </tr>
    <tr>
      <td style="text-align:center"><code>shape</code>
      </td>
      <td style="text-align:center">
        <p>default</p>
        <p>rect</p>
        <p>circle</p>
        <p>poly</p>
      </td>
      <td style="text-align:center">&#xC601;&#xC5ED;&#xC758; &#xBAA8;&#xC591;&#xC744; &#xBA85;&#xC2DC;.</td>
      <td
      style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>coords</code>
      </td>
      <td style="text-align:center">&#xC88C;&#xD45C;</td>
      <td style="text-align:center">&#xC601;&#xC5ED;&#xC758; &#xC88C;&#xD45C;&#xB97C; &#xBA85;&#xC2DC;.</td>
      <td
      style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>href</code>
      </td>
      <td style="text-align:center">URL</td>
      <td style="text-align:center">&#xD574;&#xB2F9; &#xC601;&#xC5ED;&#xC5D0; &#xC5F0;&#xACB0;&#xB41C; &#xD558;&#xC774;&#xD37C;&#xB9C1;&#xD06C;&#xC758;
        &#xB300;&#xC0C1; URL&#xC744; &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>media</code>
      </td>
      <td style="text-align:center">media queries</td>
      <td style="text-align:center">&#xB300;&#xC0C1; URL&#xC774; &#xCD5C;&#xC801;&#xD654; &#xB418;&#xB294;
        &#xBBF8;&#xB514;&#xC5B4;&#xB098; &#xB9E4;&#xCCB4;&#xB97C; &#xBA85;&#xC2DC;.</td>
      <td
      style="text-align:center">HTML5</td>
    </tr>
    <tr>
      <td style="text-align:center"><code>target</code>
      </td>
      <td style="text-align:center">
        <p>_blank</p>
        <p>_self</p>
        <p>_parent</p>
        <p>_top</p>
      </td>
      <td style="text-align:center">&#xC601;&#xC5ED;&#xC744; &#xD074;&#xB9AD;&#xD588;&#xC744; &#xB54C; &#xB300;&#xC0C1;
        URL&#xC758; &#xBB38;&#xC11C;&#xAC00; &#xC5F4;&#xB9B4; &#xC704;&#xCE58;&#xB97C;
        &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>alt</code>
      </td>
      <td style="text-align:center">text</td>
      <td style="text-align:center">
        <p>&#xC601;&#xC5ED;&#xC5D0; &#xB300;&#xD55C; &#xB300;&#xCCB4; &#xD14D;&#xC2A4;&#xD2B8;&#xB97C;
          &#xBA85;&#xC2DC;.</p>
        <p>&#xBC18;&#xB4DC;&#xC2DC; <code>href</code> &#xC18D;&#xC131;&#xC774; &#xC124;&#xC815;&#xB418;&#xC5B4;
          &#xC788;&#xC5B4;&#xC57C;&#xB9CC; &#xC0AC;&#xC6A9;&#xD560; &#xC218; &#xC788;&#xB2E4;.</p>
      </td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><code>download</code>
      </td>
      <td style="text-align:center">file name</td>
      <td style="text-align:center">&#xC0AC;&#xC6A9;&#xC790;&#xAC00; &#xD558;&#xC774;&#xD37C;&#xB9C1;&#xD06C;&#xB97C;
        &#xD074;&#xB9AD;&#xD560; &#xB54C; &#xD574;&#xB2F9; &#xB300;&#xC0C1;&#xC73C;&#xB85C;
        &#xC5F0;&#xACB0;&#xB418;&#xC9C0; &#xC54A;&#xACE0; &#xB300;&#xC2E0; &#xD574;&#xB2F9;
        &#xCF58;&#xD150;&#xCE20;&#xAC00; &#xB2E4;&#xC6B4;&#xB85C;&#xB4DC;&#xB428;&#xC744;
        &#xBA85;&#xC2DC;.</td>
      <td style="text-align:center">HTML5</td>
    </tr>
  </tbody>
</table>

#### 10\) SVG ELEMENT 

확장 가능한 벡터 그래픽\(SVG\)은 2차원의 벡터 그래픽을 기술하기 위한 XML 마크업 언어.

```markup
<svg width="150" height="150" viewBox="0 0 150 150">
	<circle r="50" cx="75" cy="75" fill="#333" stroke="#900" stroke-width="4" />
</svg>
```

#### Reference 

picture element[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/picture)

source element[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/source)

video element[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/video)

audio element[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/audio)

track element[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/track)

iframe element[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/track)

map element[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/map)

area element[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/map)

WebVTT [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/API/WebVTT_API)

SVG[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/SVG)

track element [→\(SITE\)](https://web.dev/media-accessibility/)

이미지 맵 좌표생성[ →\(SITE\)](https://www.image-map.net/)



