# BOBY : Embeded

### 1. Embeded Elements

HTML 문서에 끼워 넣는\(embeded\) 이미지, 비디오, 웹 사이트, 이미지맵, SVG 벡터 그래픽 같은 콘텐츠 요소들

#### 1\) &lt;img&gt; element

HTML 문서에 이미지를 포함\(링크\)

#### ① &lt;img&gt; element attribute

| attribute | description |
| :--- | :--- |
| src | 이미지 파일 경로 설정 |
|  alt | 이미지 대체 텍스트 설정 |
| width | 이미지 너비 설정 |
| height | 이미지 높이 설정 |
| usemap | 이미지 맵 연결 설 |



#### 2\) &lt;picture&gt; element

&lt;picture&gt;요소는 다양한 스크린 환경\(스마트폰, 데스크탑, TV 등\)에 맞는 이미지를 화면에 적절하게 표시해 주기 위해 사용한다. 이 요소를 사용할 때에는 1개 이상의 &lt;img&gt;를 포함하는 요소와 &lt;picture&gt;요소의 자식으로 0개 이상의&lt;source&gt;요소가 필요에 따라 사용할 수 있다.

&lt;source&gt;요소를 사용할 수 없을 경우에는 &lt;img&gt;요소가 화면에 표시하게 된다.

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

#### 3\) &lt;source&gt; element

&lt;picture&gt;, &lt;audio&gt;, &lt;video&gt; 요소의 다중 미디어 리소스를 지정하기 위해 사용

```markup
<video src="videofile.mp4" poster="posterimage.jpg" controls>
	<source src="videofile.webm" type="video/webm">
	<source src="videofile.ogg" type="video/ogg">
	<source src="videofile.mov" type="video/quicktime">
	HTML5 <code>video</code> 요소를 지원하지 않는 구형 웹 브라우저를 사용 중입니다.
	<a href="http://outdatedbrowser.com/ko">최신형 브라우저로 업데이트</a> 하세요.
</video>
```

#### 4\) &lt;video&gt; element

