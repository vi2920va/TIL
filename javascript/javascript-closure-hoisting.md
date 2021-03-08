# JavaScript  Closure, Hoisting

### 1. 클로저\(Closure\) 

함수와 함수가 선언된 **어휘적 환경의 조합\(lexical scoping\)**이다. 즉, 클로저 안에 정의된 함수는 만들어진 환경을 기억한다. 함수 내부에서 함수를 선언할 때, 내부의 함수는 **클로저\(closure\)** 라고 불린다. 클로저는 **외부 함수에서 생성된 변수들에 접근할 수 있는 권한**을 가지고 있다.

```javascript
const base = 'hello';

function sayHello(name) {
  const text = base + name;

  return function () {
    console.log(text);
  };
}

const hello = sayHello('vi2920va');
hello(); // hello vi2920va
```

### 2. 호이스팅\(Hoisting\) 

함수 안에 있는 선언들을 모두 끌어올려서 해당 함수 유효 범위의 최상단에 선언하는 것. `var`변수의 선언만 호이스팅이 일어난다. `let, const` 변수 선언과 함수 표현식에서는 호이스팅이 일어나지 않는다.

```javascript
firstfun();
firstfun2(); // error

function firstfun() {
    console.log("first fun");
}

var firstfun2 = function() {
    console.log("firstfun2");
}
```

#### Reference

Closures[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Closures)

