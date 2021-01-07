# BOBY : Embeded elements

### 1. Embeded Elements

HTML 문서에 끼워 넣는\(embeded\) 이미지, 비디오, 웹 사이트, 이미지맵, SVG 벡터 그래픽 같은 콘텐츠 요소들

#### 1\) img element

HTML 문서에 이미지를 포함\(링크\)

#### ① img element attribute

| attribute | description |
| :--- | :--- |
| `src` | 이미지 파일 경로 설정 |
| `alt` | 이미지 대체 텍스트 설정 |
| `width` | 이미지 너비 설정 |
| `height` | 이미지 높이 설정 |
| `usemap` | 이미지 맵 연결 설정 |



#### 2\) picture element

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

#### 3\) source element

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

#### 4\) video element

동영상 콘텐츠를 HTML 문서에 포함하기 위해서 사용한다. src 속성이나 `<socurce>`요소를 이용해 여러 개의 동영상 소소 중 하나를 표시.

#### ① video element attribute

| attribute | description |
| :--- | :--- |
| `src` | 비디오 파일 경로 설정 |
| `poster` | 포스터 이미지 경로 설정 |
| `preload` | 사용자 경험 향상\(메다테이터/ 비디오 다운로드\)에 관한 설정 |
| `controls` | 재상 컨트롤 표시 설정 |
| `autoplay` | 자동 재생 설정 |
| `loop` | 반복 설정 |
| `muted` | 음소거 설정 |

```markup
<video src="videofile.mp4" poster="posterimage.jpg">
	HTML5 <code>video</code> 요소를 지원하지 않는 구형 웹 브라우저를 사용 중입니다.
	<a href="http://outdatedbrowser.com/ko">최신형 브라우저로 업데이트</a> 하세요.
</video>
```

#### 5\) audio element

`<audio>`요소도 `<video>`요소와 유사하게 사용된다.

#### ① audio element attribute

| attribute | description |
| :--- | :--- |
| `src` | 오디오 파일 경로 설정 |
| `volume` | 볼륨 조절 설정\(0.0 ~ 1.0\) |
| `muted` | 음소거 설정 |
| `poster` | 포스터 이미지 경로 설정 |
| `preload` | 사용자 경험 향상\(메다테이터/ 비디오 다운로드\)에 관한 설정 |
| `controls` | 재생 컨트롤 표시 설정 |
| `autoplay` | 자동 재생 설정 |
| `loop` | 반복 설정 |

```markup
<audio src="audiofile.mp3">
	HTML5 <code>audio</code> 요소를 지원하지 않는 구형 웹 브라우저를 사용 중입니다.
	<a href="http://outdatedbrowser.com/ko">최신형 브라우저로
		업데이트</a>로 업데이트 하세요.
</audio>
```

#### 6\) track element

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

#### 7\) iframe element

인라인 프레임\(inline frame\)에 다른 HTML 페이지를 포함하여 화면에 표시.

#### ① iframe element attribute

| attribute | description |
| :--- | :--- |
| `src` | 프레임 소스 설정 |
| `width` | 프레임 너비 설정 |
| `height` | 프레임 높이 설정 |
| `allowfullscreen` | 프레임 전체화면 설정 |

```markup
<iframe width="560" height="315" src="https://www.youtube.com/embed/0wlXaHmmOVc?rel=0&amp;showinfo=0"
	allow="autoplay; encrypted-media" allowfullscreen></iframe>

<iframe
	src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d12643.636820892792!2d127.01610674058901!3d37.60429582641849!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x357cbc91e5ca4f03%3A0x18820a16e406c8ea!2z7ISc7Jq47Yq567OE7IucIOyEseu2geq1rCDquLjsnYwx64-ZIDUzMC0zNg!5e0!3m2!1sko!2skr!4v1520001155674"
	width="600" height="450" style="border: 0" allowfullscreen></iframe>
```

#### 8\) map element

이미지 맵\(클릭 가능한 링크 영역\)을 정의하기 위해 `<area>`요소와 함께 사용한다.

```markup
<img src="products-map.jpg" alt="제품 모음" usemap="#products-map">
<map name="products-map">
	<area shape="circle" coords="200,250,25" hreflang="en-GB" href="another.html" alt="Another Page" target="_blank">
</map>
```

#### 9\) area element

이미지의 핫스팟 지역 정의, 하이퍼링크 설정, `<map>`요소 내부에서만 사용 가능하다.

#### ① area element attribute

| attribute | description |
| :--- | :--- |
| `shape` | 핫스팟 모양 설정 |
| `coords` | 모양의 좌표 값 설정 |
| `href` | 하이퍼링크 설정 |
| `target` | 새 창\(탭\) 열림 설정 |
| `alt` | 대체 텍스트 설정 |
| `hreflang` | 연결된 페이지의 언어 속성 설정 |
| `download` | canvas 데이터 다운로드 설정 |

#### 10\) svg element

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



