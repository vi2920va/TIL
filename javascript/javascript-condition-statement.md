# JavaScript Condition Statement

### 1. CONDITION STATEMENT

특정 조건이 참\(true\)인 경우 실행하는 명령의 집합.

#### 1\) if ~ else statement

정 조건이 참\(true\)인 경우 문장을 실행하기 위해 `if문`\(statement\)을 사용한다. 또한 선택적으로 조건이 거짓\(false\)인 경우 문장을 실행하기 위해서는 `else 절`을 사용한다.

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

`switch문`은 프로그램이 표현식을 평가하고 값을 조건과 비교한다. 만약 값이 일치한다면, 프로그램 각 조건의 하위 문장을 실행한다. `switch 문`은 아래와 같이 사용한다.

```javascript

```

프로그램은 주어진 값과 일치하는 `case 라벨`을 찾는다. 그리고 나서 관련된 구문을 실행한다. 만약 매치 되는 라벨이 없다면 `default 절`을 찾는다. 찾게 되면 관련된 구문을 수행한다. `default 절`을 못 찾게 된다면 프로그램의 `switch문`을 종료한다. 여기서 `default 절`의 위치는  꼭 맨 마지막 필요는 없다.

한 번 일치된 문장이 수행되고 switch 문을 따라서 계속 수행한다면 각각의 조건절로 연결된 선택적인 `break` 문은 프로그램이 `switch 문`을 벗어나게 한다. 만약 `break 문`이 생략되면, 프로그램은 `switch 문` 안에서 다음 문장을 계속 수행한다.

#### 3\) condition ternary expression

조건문에 속하는`if,` `else if`, `else`, `switch 문`은 조건에 해당될 경우 결과 값을 반환할 수 있었지만, 변수에는 담아서 사용할 수 없었다. 하지만 `조건 연산자(3항 연산자)`의 경우에는 조건식의 참\(true\)과 거짓\(false\)일 경우 내가 원하는 변수에 담아서 사용할 수 있다. 조건 연산자는 아래의 코드와 같이 사용한다.

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



