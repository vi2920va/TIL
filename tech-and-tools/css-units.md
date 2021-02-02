# CSS Units

Units 

CSS는 절대적인 단위\(absolute unit\), 상대적인 단위\(relative unit\)두 가지로 나뉜다.

1. absolute units 

•  절대 단위\(absolute units\)는 고정된 값을 출력 하면서 절대 크기가 변화하지 않기 때문에 반응형 웹 사이트 만들 때 적합하지 않다.

•  주로  px은 픽셀\(화소\)단위를 사용한다.

2. relative units

•  상대적인 단위\(relative units\)에는 em, rem, vh, % 등 여러가지 단위들이 존재한다.

1\) em

em단위는 부모 요소의 크기 영향을 받아서 자식 요소가 상대적인 값으로 변화하게 된다.

&lt;div class=“parent”&gt;

 parent

 &lt;div class=“child”&gt;

 child

 &lt;/div&gt;

&lt;/div&gt;

body {

 color: white;

 background: \#293029;

}

div {

 border: 1px solid white;

 margin: 32px; 

}

.parent {

 /\* html element font size = 16px \*/

 /\* 16 \* 8\(%\) = 128px \*/

 font-size: 8em;

}

.child{

 /\* parent element font size = 128px \*/

 /\* 128 \* 0.5\(%\) = 64px \*/

 font-size: 0.5em;

}

2\) rem

위에서 em은 부모 요소에 따라서 자식 요소가 상대적으로 변화한다고 언급을 했었는데,  여기서 말하는 rem은 부모 요소에 따라서 자식 요소가 상대적으로 변화하지 않고 최상위 요소\(root element\)에 존재하는 &lt;html&gt; 요소에 영향을 받아서 크기가 변화한다. 

&lt;html&gt; 또는 &lt;body&gt;  요소에서 font-size를 설정하지 않으면 브라우저에 지정된  font-size가 적용된다.

3\) vh, vw 

•  vipwport는 전체 웹 페이지 가운데 브라우저 창에 보이는 영역을 말한다. 

•   vh\(viewport hight\)의 단위는 뷰포트 높이값의 1/100를 의미한다. 

•  vw\(viewport width\)의 단위는 뷰포트 너비값의 1/100분의 1를 의미한다.

•  vw,vh는 viewport 너비와 높이의 1%의 길이와 동일하다.

&lt;h2&gt; viewport - vh, vw&lt;/h2&gt;

body {

 color: white;

 background : \#293029;

}

h2{

margin: 32px;

border: 1px solid white;

/\* vw 단위는 브라우저에 화면 크기에 따라서 너비가 유동적으로 변화한다. \*/

font-size: 6vw;

}

4\) %

% 단위는 백분율 단위의 상대 단위이다. 요소의 지정된 사이즈에서 상속된 값이나 또는 기본 값에 상대적인 사이즈 설정한다.

&lt;h2&gt; % example &lt;/h2&gt; 

h2{

  /\* 16px \* 150% = 24px \*/

 font-size: 150%;

}

3.  어떤 경우에 무슨 units를 써야되는지 차이점.

1.  첫 번째 기준은 부모 요소\(parent element\)에 따라서 사이즈가 변경될 경우에는 em, % 단위를 사용하고, 부모 요소가 아닌 브라우저에 따라서 사이즈가 변경될 경우에는 rem, vw, vh 단위를 사용해야 한다.

2.   두 번째 기준은 요소의 너비\(width\)에 따라서 사이즈가 변경될 경우에는 %, v\* 단위를 사용하고, font-size에 따라서 사이즈가 변경될 경우에는 em, rem 단위를 사용한다.

3.  컴포넌트가 브라우저 어디에서도 상관없이 사이즈가 고정 되기를 원한다면 rem 단위를 사용하는게 적합하고 그렇지 않고, 부모 요소에 따라서 사이즈가 변화하기를 원한다면 em 단위를 쓰는게 적합하다.

em demo

em 단위의 font-size를 사용하게 되면 부모 요소의 영향을 받아서

계속 해서 사이즈가 커지게 된다.

&lt;div class="level1"&gt;

  &lt;h1&gt;level 1&lt;/h1&gt;

  &lt;div class="level2"&gt;

    &lt;h1&gt;level 2&lt;/h1&gt;

    &lt;div class="level3"&gt;

      &lt;h1&gt;level 3&lt;/h1&gt;

      &lt;div class="level4"&gt;

        &lt;h1&gt;level 4&lt;/h1&gt;

      &lt;/div&gt;

    &lt;/div&gt;

  &lt;/div&gt;

&lt;/div&gt;

.level1 {

  /\*  16 \* 2 = 32px  \*/

  font-size: 2em;

}

.level2 {

  /\*  32 \* 2 = 64px  \*/

  font-size: 2em;

}

.level3 {

  /\* 64 \* 2 = 128px \*/

  font-size: 2em;

}

.level4 {

  /\* 128 \* 2 = 256px \*/

  font-size: 2em;

}

rem demo

rem 단위를 사용하게 되면 부모 요소가 아닌 최상위 요소에 영향을 받아서 font-size가 편하기 때문에 계속 해서 사이즈 변화하지 않고 일정한 것을 확인할 수 있다.

&lt;div class="level1"&gt;

  &lt;h1&gt;level 1&lt;/h1&gt;

  &lt;div class="level2"&gt;

    &lt;h1&gt;level 2&lt;/h1&gt;

    &lt;div class="level3"&gt;

      &lt;h1&gt;level 3&lt;/h1&gt;

      &lt;div class="level4"&gt;

        &lt;h1&gt;level 4&lt;/h1&gt;

      &lt;/div&gt;

    &lt;/div&gt;

  &lt;/div&gt;

&lt;/div&gt;

.level1 {

  /\*  16 \* 2 = 32px  \*/

  font-size: 2rem;

}

.level2 {

  /\*  16 \* 2 = 32px  \*/

  font-size: 2rem;

}

.level3 {

  /\* 16 \* 2 = 32px \*/

  font-size: 2rem;

}

.level4 {

  /\* 16 \* 2 = 32px \*/

  font-size: 2rem;

}

 em demo\(padding\)

padding이 상황에 따라서 변경이 되기 위해서는 px 단위보다 em 단위를 쓰는게 적합하다.

&lt;h1&gt;

  Hello, dream coders 👏

&lt;/h1&gt;

h1 {

  display: inline-block;

  font-size: 5em;

  background: skyblue;

 padding : 1em;

  /\* padding: 10px; \*/

}

em, rem demo

&lt;section class="component"&gt;

  &lt;header class="title"&gt;Master Front-end ✨&lt;/header&gt;

  &lt;p class="contents"&gt;

    Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sapiente

    veniam, nulla porro distinctio aliquid, quos quidem odio consectetur

    aperiam, delectus cum. Deserunt facilis excepturi similique natus minus

    deleniti rem sit?

  &lt;/p&gt;

&lt;/section&gt;

.component {

  width: 50%;

  border: 1px solid burlywood;

  font-size: 2rem;

}

.title {

  padding: 0.5em 0.5rem;

  background-color: burlywood;

}

.contents {

  font-size: 1rem;

  padding: 0.5em 0.5rem;

}

@media screen and \(max-width: 780px\) {

  .component {

    font-size: 1.5rem;

  }

}  


