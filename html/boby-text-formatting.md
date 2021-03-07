# BOBY : text formatting

### HTML Text formatting elements

#### 1\) &lt;strong&gt; element 

`<strong>`요소는 해당 콘텐츠의 중요성, 심각함, 긴급함을 강조할 때 사용되며, 중첩되서 사용 가능하다.

```markup
<p><strong>주의!</strong> 이번 역은 승강장 사이와의 간격이 넓으니 주의하시기 바랍니다!</p>
```

#### 2\) &lt;em&gt; element 

`<em>` 요소는 `<strong>` 보다 다소 약한 강조 요소로 이 요소는 단순히 이탈릭체를 표시하기 위해서 사용하는 건 올바르지 않다.

```markup
<p><em>고양이</em>는 귀여운 동물 입니다.</p>
```

#### 3\) &lt;b&gt; element 

`<b>` 요소는 다른 글자와 구분된 용도로 사용하며 기술적 용어, 다른 언어\(목소리\), 인물의 생각 등을 표현할 때 사용한다.

```markup
<p><b>이 문장은 단순히 굵게 표현된 텍스트다.</b></p>
```

#### 4\) &lt;sup&gt; element 

`<sup>` 요소는 윗첨자, 다른 글자의 오른쪽 위에 놓이는 글자로 때로 약어에서 그리고 각주를 나타날때 사용한다.

```markup
<p>
 <sup>
     <a title="각주는 본문에 대한 참조 문헌이나 본문의 낱말,
     	문장 등의 뜻을 알기 쉽게 풀이하는 덧붙이는 글이다."></a>
 </sup>
</p>
```

#### 5\) &lt;sub&gt; element 

`<sub>`요소는 아래첨자, 다른글자의 오른쪽 아래에 놓이는 작은 글자로 대부분 화하식 또는 수학식에 사용한다.

```markup
<dfn id="sulfuric-acid">
    H<sub>2</sub>50<sub>4</sub>
<dfn>
```

#### 6\) &lt;abbr&gt; element

`<abbr>`요소는 단어의 축약형 또는 머리글자로만 단어를 정의 할 때 사용한다. 

```markup
<h2> 일본에서만 팔던 <abbr title="맥도날드">맥날 </abbr>
초콜릿 파이 오늘부터 한국에서 판매 </h2>
```

#### 7\) &lt;s&gt; element

`<s>` 요소는 더 이상 관련이 없거나 정확하지 않은 텍스트를 표현할 때 사용한다.

```markup
<ul>
    <li>
         <h3>
              <span class="sub-headline">마그네틱 자석 선정리 케이블홀더</span>
               [슈퍼특가] 자석식 선정리기 케이블 홀더
          </h3>
        <p>
          <span class="hidden-text">원래가격:</span><s>11,900원</s>
          <em>50%<em><span class="hidden-text">할인</span>5,900원
        </p>
    </li>
</ul>
```

#### 8\) &lt;mark&gt; element 

`<mark>` 요소는 형광펜을 칠한 것 처럼 하이트라이트 된 텍스트를 정의할 때 사용한다.

```markup
<p>고양이는 <mark>귀엽다</mark></p>
```

#### 9\) time element 

`<time>` 요소는 사람이 읽을 수 있는 형태의 날짜와 시간 데이터를 정의 할 때 사용한다.

```markup
<time datetime="2020-12-31T10:18"> 
2020.12.31 10:18</time>
```

#### 10\) &lt;del&gt; element 

`<del>` 요소는 텍스트 한 가운데 라인을 추가하여 삭제된 텍스트를 표현하는데 사용한다.

```markup
<p>이 벽화가 그려진 시기는 <del>청동기</del> <ins>구석기</ins> 시대이다.</p>
```

#### 11\) &lt;ins&gt; element 

`<ins>` 요소는 텍스트 아래쪽에 라인을 추가하여 삭제된 텍스트를 표현하는데 사용한다.

```markup
<p>이 벽화가 그려진 시기는 <del>청동기</del> <ins>구석기</ins> 시대이다.</p>
```

#### 10\) &lt;i&gt; element 

`<i>`요소는 보통 이탤릭체로 표현되는데 사용되는데 보통은 아이콘을 나타날 때 사용한다.

```markup
<p><i>이 텍스트는 이탤릭체로 나타난다.</i></p>
```

#### 11\) &lt;small&gt; element

`<small>`요소는 크기가 작은 텍스트를 정의할 때 사용된다.

```markup
<p><small>이 텍스트는 크기가 작은 텍스트이다.</small></p>
```

#### Reference 

strong element [→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/strong)

em element [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/em)

b element [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/b)

sup element [→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/sup)

sub element [→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/sub)

abbr element[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/abbr)

time  element[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/time)

s element [→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/s)

ins element [→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/ins)

del element[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/del)

i element [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/i)

mark element [ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/mark)

small element [→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/HTML/Element/small)





