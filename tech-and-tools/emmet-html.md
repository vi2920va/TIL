# HTML EMMET

![emmet](../.gitbook/assets/1_uytzdnlnsiuwev8h_a0bxa.png)

### 1. EMMET 

 강력한 자동완성 기능 등으로 HTML 작성 속도를 크게 향상 시켜주는 플러그인

### 2. BASIC SYNTAX

#### 1\) basic syntax

`>`표시는 하위에 포함한 요소를 생성하라는 의미.

```markup
<!-- div>ul>li-->
<div>
  <ul>
    <li></li>
  </ul>
</div>
```

#### 2\) 병렬로 나열된 요소

병렬로 나열된 요소를 생성하려면 `+` 기호로 연결.

```markup
<!-- div+p+bq -->
<div></div>
<p></p>
<blockquote></blockquote>
```

#### 3\) 여러개 반복 

`*`뒤에 숫자를 입력하면 숫자만큼 반복되서 생성.

```markup
<!-- ul>li*5 -->
<ul>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
</ul>
```

#### 4\) class name 

요소를 생성할때 `.`기호를 사용하면  CSS 클래스 이름과 함께 생성하라는 의미, ID 경우에는 `#`기호를 사용.

```markup
<!-- ul>li.item*5 -->
<ul>
    <li class="item"></li>
    <li class="item"></li>
    <li class="item"></li>
    <li class="item"></li>
    <li class="item"></li>
</ul>
```

#### Reference

Cheat Sheet [→\(SITE\)](https://docs.emmet.io/cheat-sheet/)

