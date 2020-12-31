# BOBY : image, figure, figcaption

### HTML image 정의

HTML 문서는 이미지\(image\)를 포함하지 않고 연결하여 사용한다. 

웹 페이지에서 주로 사용되는 이미지의 종류는 `.jpg, .png, .gif, .svg` 등이 있다.

#### 1\) 이미지 삽입

HTML문서에서 이미지를 삽입할 때는 `<img>`요소를 사용한다. 

`src` 속성은 이미지가 저장된 주소의 URL이고, `alt`속성은 이미지 대체 텍스트 이다.

`<img>`요소는 빈 요소\(empty element\)이다.

```markup
<img src="./image/example.svg" alt="example file">
```

#### 2\). 이미지 파일 형식들

① jpg image

jpg 이미지는 압출륙이 높고,다양한 색상을 처리하도록 설계되었다. 사진 또는 복잡한 그래픽 이미지에 많이 사용되는 포멧 입니다. 하지만 gif, png와 달리 투명한 픽셀은 허용되지 않는다.

② png image

png는 사진이나 애니메이션을 제외한 모든 유형에 적합합니다. 사진의 경우 동일한 품질의 png 파일 크기가 일반적으로 jpg 보다 크기 때문입니다. 하지만 jpg와 달리 투명처리가 가능해 아이콘, 로고, 다이어그램 등에 사용한다.

③ gif image

gif는 표현 가능한 색상이 256색으로 제한되어 있기 때문에 사진에는 적합하지 않습니다. 하지만 애니 메이션을 적용할 수 있는 포멧으로 단순한그래픽의 애니메이션에 사용하면 좋다. 투명처리가 가능하긴 하지만, png 포멧 보다 표현력이 떨어진다.

④ svg image

svg 는 벡터 기반 그래픽 포멧으로 품질 손실 없이 확대, 축소 할 수 있다. 오늘날 처럼 다양한 스크린에 대응하는 반응형 웹 디자인에 매우 적합하다.

#### 3\) 이미지를 감싸는 요소

`<figure>`요소는 사진, 이미지, 다이어그램 등을 감싸는 요소이다. 

`<figcaption>`요소는 `<figure`&gt;요소의 설명을 나타낸다.

```markup
<figure>
    <img src="/media/cc0-images/elephant-660-480.jpg"
         alt="Elephant at sunset">
    <figcaption>An elephant at sunset</figcaption>
</figure>
```

#### Reference

img element  [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/img)

figure element [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/figure)

figcaption element [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/figcaption)

