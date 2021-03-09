# JavaScript Objects

## Object

JavaScript의 기본 데이터 타입은 객체\(Object\)이다. 객체는 일종의 복합체로, 여러 값\(원시 타입의 값 또는 다른  객체\)들을 묶어 이름으로 저장하고, 값을 가져올 수 있다. 즉, 객체는 이름과 값으로 구성된 프로퍼티들의 정려로디지 않은 집합이다.

### 1. 객체 생성

객체 리터럴 또는 생성자 함수를 정의하고 new 키워드를 사용해서 만들 수도 있다.

#### 1\) 객체 리터럴

객체를 생성하는 가장 쉬운 방법은 객체 리터럴을 사용하는 것이다. 객체 리터럴은 중괄호\({}\) 안에, 이름과 값을 쌍점\(:\)으로 구분한 순서 쌍을 쉼표로 연결한 리스트다. 프로퍼티 이름으로는 JavaScript 식별자 또는 문자열을 사용할 수 있다, 프로퍼티의 값으로는 JavaScript의 표현식을 사용할 수 있다. 이때 표현식의 값\(원시 값 또는 객체 값\)은 곧 프로퍼티의 값이 된다.

```javascript
let empty = {};

let page = {
  category : "javaScript",
  title : "for ~ in",
  author : "vi2920va",
  date : "2021-03-09"
};

```

#### 2\) 생성자 함수\(constructor function\)

JavaScript의 객체\(instance\)는 생성자 함수\(constructor function\)를 통해 생성된다. new 연산자 뒤에 생성자 함수를 실행하면, 내장 객체 또는 사용자 정의 객체 인스턴스를 생성한다. 여기서 말하는 인스턴스 라는 용어는 객체\(object\)와 유사하다. 다만 의미상으로 "객체"는 좀 더 일반적인 반면에 "인스턴스"는 라고 표현하면 현재 생성된 바로 그 객체라는 인스턴스한 뉘앙스를 더 짙게 표현할 수 있다.

```javascript
// (1) 생성자 함수 정의.
// 생성자 함수는 관례적으로 첫글자는 대문자로 작성해, 일반 함수와 구분한다.
function Tab(){
 this.el = document.querySelector(selector);
}

// (2) 정의된 생성자 함수를 new 연산자와 함께 실행하면 객체 인스턴스를 생성.
let main_tab = new Tab('.main__tab');
let body_tab = new Tab('body');

// (3) 생성자 함수를 통해서 생성된 인스턴스를 확인.
console.log(main_tab instanceof Tab);
console.log(main_tab.constructor === Tab);
```





#### 

