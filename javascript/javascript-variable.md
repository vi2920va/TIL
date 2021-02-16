# JavaScript Variable

### 1. JavaScript Declarations

JavaScript의 선언\(Declaration\)에는 var, let, const 세가지 키워드를 사용하는 방법이 있다.

#### 1\) Variables

변수\(Variable\)는 메모리에 데이터를 저장하기 위한 기억 공간을 의미한다. 즉, 데이터를 담아 놓는 그릇이라고 생각하면 된다. 또한 변수에 담긴 데이터는 필요에 따라 수시로 데이터를 변경 시킬 수 있다.

#### 1\) **Variable Declaration**

JavaScript에서 **변수 선언\(Variable Declaration\)**은 `var`, `let`, `const` 세가지 키워드를 사용하는 방법이 있다.

```javascript
// var 변수명 = 할당 값;
var last_year;
var currentYear;

// 지정된 초기값 없을때  
// 선언된 변수의 값은 undefined
console.log(last_year);
console.log(currentYear);

// 선언되지 않은 변수를 읽을 때 
// ReferenceError: z is not defined 
console.log(z);
```

#### 변수 이름 작성 규칙

JavaScript에서 변수 이름은 식별자\(identifier\)라고 불린다. 식별자는 문자, 밑줄\(\_\) 혹은 달러 기호\($\)로 시작해야 하는 반면 이후는 숫자\(0~9\)일 수도 있다.  대소문자를 구분하기에 문자는 A부터 Z\(대문자\)와 a부터 z\(소문자\)까지 모두 포함된다.



#### 2\) V**ariable Assignment**

변수에 값을 대입하는 것을 "**변수에 할당한다.**" 는 의미이다.

```javascript
// 값 할당(assignment)
// 대입, 할당 연산자 (operator)
var x, y;
x = 9;
y = x * x + 10;
console.log('x:', x);
console.log('y:', y);
```

#### 3\)  Variable Scope

변수의 범위를 '**스코프\(Scope\)' 라고 부른다.**

* Global Scope
  * 전역 변수\(Global Scope\)는 함수의 외부에서 선언된 변수로 프로그램 전체에서 접근할 수 있는 변수이다.
* Local Scope
  * 지역변수\(Local Scope\)는 함수 내부에서 선언된 변수로 함수가 실행되면 만들어지고 함수가 종료되면 소멸하는 변수이다. 또한 함수 외부에서 접근할 수 없다.

```javascript
// #1. phone 전역변수, scopeFn() 함수 내부에 지역 변수 
var phone = 'Galaxy';

function scopeFn() {
  var phone = 'iPhone';
  console.log('지역 변수', phone); // 'iPhone'
}
scopeFn();
console.log('전역 변수', phone); // 'Galaxy'

// #2. var 키워드를 쓰지 않으면 함수 내에 선언되지 않은 변수는 지역 변수로 처리하지 않는다.
// 즉, 다시 말해서 상위루트로 이동해서 tablet를 찾고 없으면 tablet를 전연 변수로 만들기 떄문
// 에 아래의 코드는 잘못된 사용법이다.
// function subFn() {
// 	 tablet = 'Note XII'; 
//   console.log(tablet);
// }
// subFn(); 


// #3. 네임스페이스 (객체)
var y9 = {};

// 전역을 오염시키지 않으려면, 네임스페이스 객체 활용
// 네임스페이스를 활용한 변수 대용
y9.phone = 'Galaxy Note 8';
// 네임스페이스를 활용한 함수 대용
y9.getPhone = function () {
  return this.phone;
};
```

#### 4\) Variable Hoisting

호이스팅\(Hosting\)은 변수의 정의가 그 스코프에 따라 선언과 할당으로 분리되는 것은 의미한다. 선언 부분이 해당 스코프의 최상위로 변경된다.

```javascript
//  호이스팅
message("commit");
function message(){
    //선언되지 않은 값을 호출 할 때 error : not defined 
    console.log(git);
    
    // 변수의 선언을 먼저 하고 난 뒤 할당.
    var test;
    console.log(test);
    test ="Git message";
    console.log(test);
}
```

#### Reference

JavaScript 문법과 자료형[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Values,_variables,_and_literals)

