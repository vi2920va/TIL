# CSS typography

### 1. TYPHOGRAPHY

타이포그래피\(typhography\)는 글자와 문단의 속성을 제어한다.

### 2. FONT PROPETIES

#### 1\) font-family

`font-family` 속성은 하나의 글꼴 또는 여러 개의 글꼴을 같이 설정할 수 있다. 여러 개의 글꼴이 설정 되었으면 웹 브라우저는 위에서부터 순서대로 글꼴을 읽어들인다.  

글꼴의 이름이 한 단어 이상으로 이루어지면 반드시 따옴표\(""\)사용하여 둘러 쌓는다. 또한 여러 개의 글꼴을 나열할 때에는 쉼표\(,\)로 구분짓는다.

#### 2\) font-style

`font-style`속성은 주로 이탤릭체를 사용하기 위해 사용하며, 다음과 같이 3가지 속성값을 가진다.

* normal - 텍스트에 어떠한 스타일도 적용하지 않는다.
* italic - 텍스트에 이탤릭체로 나타낸다.
* oblique - 텍스트를 기울인다. `italic` 속성과 매우 유사하지만 지원하는 브라우저가 거의 없다.

#### 3\) font-variant

`font-variant`속성은 속성값이 small-caps 설정되면 텍스트에 포함된 영문자 중 모든 소문자를 작은 대문자\(small-caps\)글꼴로 변경 시킨다.

#### 4\) font-weight

font-weight 텍스를 얼머나 두껍게 표현할지 설정한다. 사용할 수 있는 속성값는 `lighter, normal, bold, bolder, 100, 200, ...,900`등으로 텍스트의 두꼐를 설정할 수 있다.

#### 5\) font-size

`font-size`속성은 텍스트의 크기를 설정한다.

### 3. TEXT PROPETIES

#### 1\) line-height

인라인 요소의 높이를 표현, 글자가 요소  높이의 중간에 위치하도록 사용

\(line-height\) - \(font-size\)/2 = 반행간

반행간 + font-size + 반행간 = line-height

#### 2\) letter-spacing

자간, 글자 사이의 간격 설정.

#### 3\) word-spacing

어간, 단어와 단어 사이의 간격 설정.

#### 4\) text-align

`text-align`속성은 텍스트의 수평 방향 정렬을 설정한다. `text-align` 속성은 `text-direction`속성과는 상관없이 우선적으로 적용된다.

#### 5\) text-indent

`text-indent`속성은 단락의 첫 줄에 들여쓰기 할지 안 할지를 설정한다. 웹 페이지가 기본적으로 들여쓰기가 설정되어있지 않다.

#### 6\) text-transform

`text-transform`속성은 텍스트에 포함된 영문자에 대한 대소문자를 설정한다. 이 속성은 텍스트에 포함된 모든 영문자를 대문자 또는 소문자로 변경시켜준다. 또한 단어의 첫 문자만을 대문자로 변경할 수 있다.

#### 7\) text-decoration

`text-decoration`속성은 텍스트에 여러가지 효과를 설정하거나 제거하는데 설정.

#### 8\) text-shadow

`text-shodowm`속성은 텍스트에 간단한 그림자 효과를 설정.

#### 9\) white-space

공백\(tab, space, line break\)처리 설정.

#### 10\) word-break

줄 바꿈 할 때 단어/글자 인지 결정해서 설정.

#### 11\) word-wrap

박스의 가로 영역을 넘친 단어 내에서 임의의 분리.

