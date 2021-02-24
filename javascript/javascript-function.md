# JavaScript Function

### 1. Function

함수\(Function\)는 하나의 특별한 목적의 작업을 수행하도록 설계된 독립적인 블록을 의미한다. 즉, 함수는 '절차'로 일을 할 때 거쳐야 하는 일한 차례와 방법이다.  


#### 1\) function declaration

**함수 선언\(function declaration\)**은 지정된 매개변수\(parameter\)를 갖는 함수를 정의한다. 

```javascript
function name([param[, param,[..., param]]]) { [statements] }
```

📝**name**

함수의 이름.

📝 **param**

함수로 전달되는 인수\(argument\)의 이름.

📝**statements**

함수의 몸통\(body\)을 구성하는 문\(statement\).

#### 2\)  function expression

**함수 표현식\(function expression\)**은 함수를 정의할 때 이름을 정해주지 않으면 익명 함수\(anonymous function\)가 된다. 그러므로 변수에 참조 시켜야 한다. 

```javascript
// 함수 선언과 함수 표현식의 차이점은 함수 표현식은 변수에 할당된 다음부터 호출할 수 있다.
// print(); // Error
const print = function () {
  console.log('print');
};

print();
const printAgain = print;
printAgain();
```

#### 3\) calling function

함수를 정의하는 것은 함수를 실행하는 것은 아니다. 함수를 정의하는 것은 간단히 함수의 이름을 지어주고, 함수가 호출될 때 무엇을 할지 지정해주는 것이다.  사실 함수를 호출하는 것은 나타나있는 매개변수를 가지고 지정된 행위를 수행하는 것이다. 

```javascript
console.log(square(5));
function square(n) {
  return n * n;
}
```

#### 4\) callback function

콜백 함수\(callback function\)는 인수로 다른 함수에 전달 된 함수로, 외부 함수 내에서 호출되어 일종의 루틴이나 작업을 완료한다.

```javascript
function greeting(name) {
  console.log('Hello ' + name);
}

function processUserInput(callback) {
  var name = prompt('Please enter your name.');
  callback(name);
}

processUserInput(greeting);
```

#### 5\) function scope

**함수의 범위\(function scope\)**는 함수 코드 블록 내에서 선언된 변수는 함수 코드 블럭 내에서만 유효하고 함수 외부에서는 유효하지 않다\(참조할 수 없다\). 즉, 함수 안에서 변수를 정의하면 함수 안에서 접근할 수 없다.

```javascript
let global = 'global';

function scopeTest() {
  let local = 'local';
  console.log(global);
  console.log(local);
}

scopeTest();
console.log(global);
console.log(local); // Uncaught ReferenceError: local is not defined
```

#### 6\) arrow function expression

 **화살표 표현식\(arrow function expression\)**은 `function` 표현에 비해 구문이 짧다. 화살표 함수는 항상 익명이다. 

```javascript
// Same as following :  => { return expression; }
(param1, param2, …, paramN) => { statements }
(param1, param2, …, paramN) => expression

// Parentheses are optional if there is only one parameter
(singleParam) => { statements }
singleParam => { statements }

// Function without parameters requires parentheses
() => { statements }
```

#### 7\) IIFE \(Immediately Invoked Function Expression\)

즉시 실행 함수 표현\(Immediately Invoked Function Expression\)은 정의되자마자 즉시 실행되는 함수 이다.

```javascript
(function () {
    statements
})();
```

```javascript
// IIFE 내부의 변수는 외부로 부터 접근이 불가능하다.
(function () {
    let aName = "Barry";
})();
aName // throws "Uncaught ReferenceError: aName is not defined"

// IIFE를 변수에 할당하면 함수의 실행된 결과만 저장된다.
const result = (function () {
    let name = "Barry";
    return name;
})();
result; // "Barry"
```

### 2. FUNCTION PARAMETER 

ES6 부터 추가된 함수의 매개변수에는 **default parameter,** **reset parameter** 두 가지 방법이 있다.

#### 1\) default parameter

함수의 매개변수는 `undefined`가 기본으로 설정된다. 그러므로 함수의 매개변수가 `null`또는 `undefined`로 전달될 경우 매개변수를 기본 값으로 초기화 한다.

```javascript
function multiply(a, b = 1) {
  return a*b;
}

multiply(5);
```

#### 2\) reset parameter

**나머지 매개변수\(reset parameter\)** 구문을 정해지지 않은 수\(an indefinite number\)를 배열로 나타낼 수 있게 한다. 

```javascript
function myFun(a, b, ...manyMoreArgs) {
    // console.log('a : ' , a); // one
    // console.log('b : ' , b); // two
    // console.log('manyMoreArgs : ', manyMoreArgs); // [three, four, five, six]
}
myFun('one', 'two', 'three', 'four', 'five', 'six');
```











#### 



