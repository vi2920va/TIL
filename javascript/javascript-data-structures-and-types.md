# JavaScript Data structures and types

### 1. Data Types

최신 ECMAScript 표준은 7가지 데이터 유형을 정의한다.

* **Boolean** 
* **null**
* **undefined**
* **Number**
* **String**
* **Symbol** \(ES6+\)
* **Object**

#### 1\) null, undefined

**undefined**는 데이터 타입, 값을 나타낸다. 즉, 변수만 선언했지만 할당하지 않은 변수를 말한다. 

**null**의 타입 변수의 경우에는 명시적으로 값을 비어 있음을 나타내는데 사용한다. 즉, 아무것도 참조하지 있지 않다는 의미로 주로 객체를 담을 변수를 초기화 할 때 많이 사용한다.

```javascript
// null
let nothing = null;
console.log(`value : ${nothing}, type : ${typeof nothing}`);

// undefined
let x;
console.log(`value : ${x}, type : ${typeof x}`);
```

### 2. Data type conversion

JavaScript는 동적 형지정\(정형\) 언어이다. 이는 변수를 선언할 때 데이터 형을 지정할 필요가 없음을 의미한다. 또한 데이터 형이 스크립트 실행 도중 필요에 의해 자동으로 변환됨을 뜻한다.

```javascript
// 숫자 값이 문자로 변경되는 경우.
var x = 42;
x = 'The answer is ' + String(42); // "The answer is 42"

// 숫자형 문자 값이 숫자로 변경되는 경우.
var y = '12345';
y = Number(y) - 3; // 12342

// 문자 값을 숫자로 변경해야 하는 경우.
var img_width = '100px';
img_width = window.parseInt(img_width, 10); // 100

var img_height = '201.89px';
img_height = window.parseFloat(img_height, 10); // 201.89
```

### 3. Literals

JavaScript에서 값을 나타내기 위해 **리터럴\(literal\)**을 사용한다. 이는 말 그대로 스크립트에 부여한 고정값으로 변수가 아니다.

* **Array literals**
* **Boolean literals**
* **Floating-point literals**
* **Numeric literals**
* **Object literals**
* **RegExp literals**
* **String literals**

\*\*\*\*







