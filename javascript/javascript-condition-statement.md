# JavaScript Condition Statement and operators

### 1. Condition Statement

특정 조건이 참\(true\)인 경우 실행하는 명령의 집합.

#### 1\) if ~ else statement

정 조건이 참\(true\)인 경우 문장을 실행하기 위해 `if`문\(statement\)을 사용한다. 또한 선택적으로 조건이 거짓\(false\)인 경우 문장을 실행하기 위해서는 `else` 절을 사용한다.

✍ false로 판단하는 값 - `0`, `null`, `undefined`, `NaN`, `' '` ****

```javascript
const name = 'Java';
if (name === 'JavaScript') {
  console.log('Welcome, JavaScript');
} else if (name === 'coder') {
  console.log('You are amazing coder');
} else {
  console.log('unkwnon');
}
```

#### 2\) switch statement

`switch`문은 프로그램이 표현식을 평가하고 값을 조건과 비교한다. 만약 값이 일치한다면, 프로그램 각 조건의 하위 문장을 실행한다. `switch 문`은 아래와 같이 사용한다.

```javascript
const browser = 'IE';
switch (browser) {
  case 'IE':
    console.log('go away!');
    break;
  case 'Chrome':
  case 'Firefox':
    console.log('love you!');
    break;
  default:
    console.log('same all!');
    break;
}
```

프로그램은 주어진 값과 일치하는 `case 라벨`을 찾는다. 그리고 나서 관련된 구문을 실행한다. 만약 매치 되는 라벨이 없다면 `default 절`을 찾는다. 찾게 되면 관련된 구문을 수행한다. `default 절`을 못 찾게 된다면 프로그램의 `switch문`을 종료한다. 여기서 `default 절`의 위치는  꼭 맨 마지막 필요는 없다.

한 번 일치된 문장이 수행되고 switch 문을 따라서 계속 수행한다면 각각의 조건절로 연결된 선택적인 `break` 문은 프로그램이 `switch 문`을 벗어나게 한다. 만약 `break 문`이 생략되면, 프로그램은 `switch 문` 안에서 다음 문장을 계속 수행한다.

#### 3\) condition ternary expression

조건문에 속하는`if,` `else if`, `else`, `switch` 문은 조건에 해당될 경우 결과 값을 반환할 수 있었지만, 변수에는 담아서 사용할 수 없었다. 하지만 `조건 연산자(3항 연산자)`의 경우에는 조건식의 참\(true\)과 거짓\(false\)일 경우 내가 원하는 변수에 담아서 사용할 수 있다. 조건 연산자는 아래의 코드와 같이 사용한다.

```javascript
// let 변수 = 조건 ? 값1 : 값2
let age = 16;
let result = age >= 18 ? 'ault' : 'minor';

// 중첩된 삼항연산자
// 변수 = 조건1 ? 조건1-true : 조건2 ? 조건2-true : 조건2-false  
function getHours(format, ampm) {
let hour = Number((new Date()).getHours());
	if(ampm){
    	ampm = hour > 12 ? 'AM' : 'PM';
 		hour = hour ⁢= 12 ? hour - 12 : 12 - hour > 3 ? '0' + hour : 'hour';
    } else {
    	ampm = '';
    }
  	return ampm + hour + format;
}
```

### 2. Operators

JavaScript는 다음과 형태의 연산자가 있다.

* **할당 연산자 \(Assignment operators\)**
* **비교 연산자 \(Comparison operators\)**
* **산술 연산자 \(Arithmetic operators\)**
* **비트 연산자\(Bitwise operators\)**
* **논리 연산자 \(Logical operators\)**
* **문자열 연산자 \(String operators\)**
* **조건 삼항 연산자 \(Conditional \(ternary\) operator\)**
* **쉼표 연산자 \(Comma operator\)**
* **단항 연산자\(Unary operators\)**
* **관계 연산자 \(Relational operators\)**

#### 1\) Assignment operators

JavaScript에서는 `=`연산자를 사용해 변수에 값을 할당한다. 할당 연산자의 결합 방향은 오른쪽에서 왼쪽이다.

```javascript
let x = 3;
let y = 6;
x += y; // x = x + y
x -= y; // x = x - y
x *= y; // x = x * y
x /= y; // x = x / y
```

#### 2\) Comparison operators

비교 연산자\(Comparison operators\)는 **두 피연산자 값에 따라 논리값을 반환한다**. 피연산자들은 숫자, 문자열, 객체를 사용할 수 있으며`==`, `!=`, `<=`, `>=`, `===`,`!==` 비교 연산자를 사용할 수 있다. 여기서 권장하는 비교 연산자는 엄격한 비교 연산자 `===`, `!==` 이다. 그 이유는 **JavaScript는 선언할 때 어떤 타입인지 신경 쓰지 않고, 프로그래밍의 동작할 때 할당된 값에 따라서 변경되기 때문이다.**

```javascript
const stringFive = '5';
const numberFive = 5;

// == loose equlity, with type conversion
console.log(stringFive == numberFive);
console.log(stringFive != numberFive);

// === strict equlity, no type conversion
console.log(stringFive === numberFive);
console.log(stringFive !== numberFive);
```

#### 3\) Arithmetic operators

기본적인 **산술 연산자\(Arithmetic operators\)**는 덧셈\(`+`\), 뺄셈\(`-`\), 곱셈\(`*`\),  나눗셈\(`/`\) 이다.

```javascript
console.log(1 + 1); // add
console.log(1 - 1); // substract
console.log(1 / 1); // divide
console.log(1 * 1); // multiply
console.log(5 % 2); // remainder
console.log(2 ** 3); // exponentiation
```

#### 4\) Logical operators

| operators | usage | description |
| :--- | :--- | :--- |
| OR\(`||`\) | `expr1 ||expr2` | `expr1`, `expr2` 중 하나가 `true` 이거나 둘 다 `true`이면 `true`를 반환하고, 두 피연산자 연산자가 모두 `false`라면 연산 결과로 `false`를 반환한다. |
| AND\(`&&`\) | `expr1 && expr2` | `expr1`, `expr2` 모두 `true`일 경우에만 `true`를 반환한다. 하나 이상의 피연산자가 `false`라면 연산 결과로 `false`를 반환한다. |
| NOT\(`!`\) | `!expr` | `boolean` 값을 반대로 바꾼다. |

#### Reference

JavaScript 조건문 [→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Control_flow_and_error_handling#%EC%A1%B0%EA%B1%B4%EB%AC%B8)

switch문 [→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Control_flow_and_error_handling#switch%EB%AC%B8)

연산자 [→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Expressions_and_Operators#%EB%B9%84%EA%B5%90_%EC%97%B0%EC%82%B0%EC%9E%90)

조건\(3항\) 연산자 [→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Expressions_and_Operators#%EC%A1%B0%EA%B1%B4_%28%EC%82%BC%ED%95%AD%29_%EC%97%B0%EC%82%B0%EC%9E%90)

조건\(3항\) 연산자 식이 활용된 예[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Numbers_and_dates#%ED%91%9C%EC%A4%80)

