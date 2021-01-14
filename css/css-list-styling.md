# CSS list styling

### 1. LISTS STYLING

HTML 목록&lt;ul&gt;, &lt;ol&gt;, &lt;li&gt;, &lt;dl&gt;, &lt;dt&gt;, &lt;dd&gt;\)과 관련된 속성.

#### 1\) list-style-type

리스트 앞에 오는 블릿의 타입 결정하는 속성.

| property value | description |
| :---: | :---: |
| `none` | 아무런 장식도 없는 형태. |
| `disc`\(defalut\) | 채워진 원형 형태. |
| `circle` | 속이 빈 원형 형태. |
| `square` | 채워진 사각형 형태. |
| `decimal` | 숫자 1. 2. 3. 의 형태. |

#### 2\) list-style-position

리스트 블릿이 밖에 있을지, 안에 있을지 결정하는 속성.

| property value | description |
| :---: | :---: |
| `outside`\(defalut\) | 블릿을 바깥으로 위치. |
| `inside` | 블릿을 내부에 위치. |
| `inherit` | 부모의 값을 상속. |

#### 3\) list-style-image

리스트 블릿으로 기본 형태가 아닌 이미지를 사용하고자 할 때 사용되는 속성값으로 해당 이미지 주소를 `url` 을 적어준다.

```text
ul {
  list-stype-image : url('../img/file.png');
}
```

#### Reference

list-style-type [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/CSS/list-style-type)

list-style-position [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/CSS/list-style-position)

list-style-image [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/CSS/list-style-image)



