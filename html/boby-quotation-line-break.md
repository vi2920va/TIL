# BOBY : Quotation, Line Break

### HTML Quotation

글을 쓰거나, 신문기사 및 다른 글을 인용하는 경우에 인용임을 표시하는 인용문과 인용구을 사용한다. 

`<blockquote>`요소는 긴 인용문에 사용되고 짧은 인용문을 나타낼 때에는 인라인 레벨 요소인 `<q>` 요소를 사용한다.

#### 1\) blockquote element

`<blockquote>`요소는 다른 출처로 부터 인용된 블럭을 정의할 때 사용되며, 이렇게 인용된 블록을 브라우저는 보통 들여쓰기를 사용하여 표현한다.

`cite`속성을 사용하여 출처를 명시할 수 있으며, `cite` 속성은 선택적으로 사용한다.

```markup
<blockquote>문단 단위 이상의 인용할 때 사용한다. 브라우저는 보통 들여쓰기로 나타낸다.</blockquote>
```

#### 2\) q element

`<q>` 요소는 짧은 길이의 인용구를 정의할 때 사용되며,  이러한 인용구를 브라우저는 보통 앞/뒤에 큰 따옴표를 추가하여 표현한다. 

`cite`속성을 사용하여 출처를 명시할 수 있으며, `cite` 속성은 선택적으로 사용한다.

```markup
<q>짧은 인용구를 정의할 때 사용되고, 브라우저는 앞/뒤에 큰 따옴표를 표시한다.</q>
```

#### 3\) address element

`<address>` 요소는 글의 저자 또는 연락처 정보를 명시할 때 사용한다.

```markup
<footer>
    코딩의 시작!!
    <address>      
    티씨피스쿨코리아(주)<br>
    서울시 강남구 역삼동<br>
    Tel: (02)123-4567 | Fax: (02)234-5678
    </address>
</footer>
```

#### 4\) cite element

`<cite>`요소는 책이나 음악, 영화, 예술 작품 등과 같은 창작물의 제목을 정의할 때 사용한다.

```markup
<img src="/examples/images/monalisa.jpg" height="300" width="200" alt="monalisa">
<p><cite>Mona Lisa</cite> 레오나르도 다 빈치, 1503년</p>
```

### HTML Line Break 

HTML 소스 코드에서 엔더\(enter\)를 사용하여도 브라우저 화면에는 실제로 적용되지 않는다. 따라서 텍스트 내의 줄 바꿈을 하고 싶을 때는`<br>`요소를 사용한다.

#### 1\) br element

`<br>` 요소는 주소\(address\) 또는 시\(poem\)등 줄바꿈이 중요한 텍스트에 유용하게 사용된다.

`<br>`요소는 빈 요소\(empty element\)이다.

#### Reference

 blockquote element [→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/blockquote)

address element [→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/address)

cite element [→\(MDN\) ](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/cite)

q element [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/q)

br element [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/br)





