# CSS INTRO

### CSS 정의

CSS\(Cascading Style Sheets\)는 HTML 요소들이 각 종 미디어에서 어떻게 보이는가를 정의하는 데 사용하는 스타일 시트 언어\(style sheet language\)이다. 

#### 1\) CSS Styling 

####  ① 인라인 스타일\(inline style\) - CSS 코드를 HTML 문서에 포

```markup
<style>
  section {
    color: #903000;
  }

  h1 {
    color: tan;
  }

  abbr {
    cursor: help;
  }
</style>
```

#### ② 내부 스타일 시트\(internal style sheet\) - HTML 요소에 style 속성 사용해서 style을 적용

```markup
<body>
    <h2 style="color:green;">interal style sheet</h2>
</body>
```

#### ③ 외부 스타일 시트\(external style sheet\) - CSS 파일을 HTML 문서에 연결

```markup
<link rel="stylesheet" href="css/style.css">
```

