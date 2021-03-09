# JavaScript Objects

## 객체\(Object\)

JavaScript의 기본 데이터 타입은 객체\(Object\)이다. 객체는 일종의 복합체로, 여러 값\(원시 타입의 값 또는 다른  객체\)들을 묶어 이름으로 저장하고, 값을 가져올 수 있다. 즉, 객체는 이름과 값\(key /  value\)으로 구성된 프로퍼티들의 정렬로 되지 않은 집합이다.

### 1. 객체 생성

객체 리터럴 또는 생성자 함수를 정의하고 new 키워드를 사용해서 만들 수도 있다.

#### 1\) 객체 리터럴

객체를 생성하는 가장 쉬운 방법은 객체 리터럴을 사용하는 것이다. 객체 리터럴은 중괄호\({}\) 안에, 이름과 값을 쌍점\(:\)으로 구분한 순서 쌍을 쉼표로 연결한 리스트다. 프로퍼티 이름으로는 JavaScript 식별자 또는 문자열을 사용할 수 있다, 프로퍼티의 값으로는 JavaScript의 표현식을 사용할 수 있다. 이때 표현식의 값\(원시 값 또는 객체 값\)은 곧 프로퍼티의 값이 된다.

```javascript
let empty = {};

let car = {
  type: 'normal',
  wheels: 4,
  handle: 1,
  mirrors: { side: 2, back: 1 },
  engine: '3000cc',
  weight: '313kg',
  booster: false
};

```

#### 2\) new 연산자를 사용 객체 생성

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

### 3\) Object.create\(\)

Object.create\(\)메서드를 사용하게 되면 새로운 객체를 생성 할 때  create 내부에 전달되는 객체의 능력을 새롭게 생성 되는 객체가 물려 받게 할 수 있다.  즉. 상속을 구현할 수 있다. \(단, 새롭게 생성된 객체에서 속성을 기술해도, 상속을 해준 부모의 속성은 변하지 않는다.\)

```javascript
Object.create(proto[, propertiesObject])
```

📝 proto

새로 만든 객체의 프로토타입이어야 할 객체.

📝 propertiesObject\(\)

자신의 속성이 열거 가능한 객체는 해당 속성명으로 새로 만든 객체 추가될 속성 설명자\(description\)를 지정한다.

```javascript
let car = {
  type: 'normal',
  wheels: 4,
  handle: 1,
  mirrors: { side: 2, back: 1 },
  engine: '3000cc',
  weight: '313kg',
  booster: false
};

let extend_car_features = {
  type: 'super',
  wheels: 6,
  booster: true,
  engine: '4497cc',
  weight: '452kg',
  maximum: {
    power: '2248 horse-power, 21800 rpm',
    torque: '194kgm, 17100 rpm',
    speed: '695km + alpha'
  }
};

var x = Object.create(car);
x.wheels = 10;
console.log(x.hasOwnProperty('wheels'));
```

### 2. 프로퍼티 속성

프로퍼티의 속성을 설정하거나 임의의 속성을 새 프로퍼티를 만들기 위해서는 Object.defineProperty\(\)를 호출한다. 이때 함수의 인자로 수정할 객체와 추가하거나 변경할 프로퍼티 이름, 프로퍼티의 디스크립터\(descriptor\) 객체를 넘긴다.

####  1\) Object.defineProperty\(\)

`Object.defineProperty()` 정적 메서드\(static method\)는 객체에 직접 새로운 속성을 정의하거나 이미 존재하는 속성을 수정한 후, 그 객체를 반환한다.

```javascript
Object.defineProperty(obj, prop, descriptor)
```

 📝 obj - 속성을 정의할 객체.

📝 prop - 새로 정의하거나 수정하려는 속성의 이름 또는 Symbol.

📝 descriptor - 새로 정의하거나 수정하려는 기술하는 객체.



 

#### 

