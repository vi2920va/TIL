---
description: JavaScript Object
---

# 객체 / 상속

## 객체\(Object\)

JavaScript의 기본 데이터 타입은 **객체\(Object\)**이다. 객체는 일종의 복합체로, 여러 값\(원시 타입의 값 또는 다른  객체\)들을 묶어 이름으로 저장하고, 값을 가져올 수 있다. 즉, **객체는 이름과 값\(key /  value\)으로 구성된 프로퍼티\(prpperty\)들의 정렬로 되지 않은 집합이다.**

#### 1\) 객체 특징

* 객체는 객체가 가진 고유 프로퍼티를 유지하는 것 외에 '프로토타입' 이라고 하는 다른 객체의 프로퍼티를 상속받는다.
* 객체의 메서드들은 일반적으로 상속받은 프로퍼티이고, 이를'프로토타입 상속'이라고 한다.
* 객체는 프로퍼티를 동적으로 추가하고 제거할 수 있기 때문에 동적이다.
* 객체는 변경 가능하며, 그 값 대신에 참조\(reference\)를 통해 조작한다.
* 객체는 객체를 참조하며, 객체 자체를 복사하지는 않는다.

#### 2\) property

프로퍼티는 이름과 값으로 구성된다.  프로퍼티는 **프로퍼티 키\(property key\)**로 유일하게 식별할 수 있다. 즉, 프로퍼티 키는 프로퍼티를 식별하기 위한 식별자\(identifier\)다. 프로퍼티 키의 명명 규칙과 프로퍼티의 값으로 사용할 수 있는 값은 아래와 같다.

* **property key** : 빈 문자열을 포함하는 모든 문자열 또는 `symbol`.
* **property value** : JavaScript의 모든 값.

### 1. 객체 생성

**객체 리터럴** 또는 **생성자 함수를 정의하고 new 키워드**를 사용해서 만들 수도 있다.

#### 1\) 객체 리터럴

객체를 생성하는 가장 쉬운 방법은 객체 리터럴을 사용하는 것이다. 객체 리터럴은 중괄호\(`{}`\) 안에, 이름과 값을 쌍점\(`:`\)으로 구분한 순서 쌍을 쉼표로 연결한 리스트다. 프로퍼티 이름으로는 JavaScript 식별자 또는 문자열을 사용할 수 있다, 프로퍼티의 값으로는 JavaScript의 모든 값을 사용할 수 있다.

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

JavaScript의 **객체\(instance\)**는 **생성자 함수\(constructor function\)**를 통해 생성된다. new 연산자 뒤에 생성자 함수를 실행하면, 내장 객체 또는 사용자 정의 객체 인스턴스를 생성한다. 여기서 말하는 **인스턴스 라는 용어는 객체\(object\)와 유사하다**. 다만 의미상으로 "객체"는 좀 더 일반적인 반면에 "인스턴스"는 라고 표현하면 현재 생성된 바로 그 객체라는 인스턴스한 뉘앙스를 더 짙게 표현할 수 있다.

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

`Object.create()`메서드를 사용하게 되면 새로운 객체를 생성 할 때  create 내부에 전달되는 객체의 능력을 새롭게 생성 되는 객체가 물려 받게 할 수 있다.  즉. **상속을 구현**할 수 있다. \(단, 새롭게 생성된 객체에서 속성을 기술해도, 상속을 해준 부모의 속성은 변하지 않는다.\)

```javascript
Object.create(proto[, propertiesObject])
```

📝 **proto**

새로 만든 객체의 프로토타입이어야 할 객체.

📝 **propertiesObject\(\)**

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

let x = Object.create(car);
x.wheels = 10;
console.log(x.hasOwnProperty('wheels')); // true
console.log(car['wheels']); // 4
```

### 2. 프로퍼티 접근

프로퍼티의 값을 가져오기 위해서는 마침표\(.\)연산자 또는 대괄호\(\[ \]\) 연산자를 사용한다. 마침표 연산자\(.\)를 사용할 경우에는 연산자 우측에는 반드시 프로퍼티 이름\(property key\)이 식별자로 와야한다. 대괄호 연산자를 사용할 경우, 대괄호 안의 값은 반드시 프로퍼티 이름의 문자열이어야한다.

```javascript
let car = {
  type: 'normal',
  weels: 4,
  handle: 1,
  mirros: {
    side: 2,
    back: 1
  },
  engine: '3000cc',
  weight: '313kg',
  booster: false
};

console.log(car.weels); // 4
console.log(car['type']); // normal
```

### 3. 프로퍼티 속성

프로퍼티의 속성을 설정하거나 임의의 속성을 새 프로퍼티를 만들기 위해서는 `Object.defineProperty`**\(\)**를 호출한다. 이때 함수의 인자로 수정할 객체와 추가하거나 변경할 프로퍼티 이름, 프로퍼티의 기\(descriptor\) 객체를 넘긴다.

####  1\) Object.defineProperty\(\)

`Object.defineProperty()` 정적 메서드\(static method\)는 객체에 직접 새로운 속성을 정의하거나 이미 존재하는 속성을 수정한 후, 그 객체를 반환한다.

```javascript
Object.defineProperty(obj, prop, descriptor)
```

 📝 **obj** 

속성을 정의할 객체.

📝 **prop**

새로 정의하거나 수정하려는 속성의 이름 또는 `Symbol`.

📝 **descriptor**

새로 정의하거나 수정하려는 기술하는 객체.

```javascript
let car = {
  type: 'normal',
  weels: 4,
  handle: 1,
  mirros: {
    side: 2,
    back: 1
  },
  engine: '3000cc',
  weight: '313kg',
  booster: false
}

Object.defineProperty(car, 'price', {
  value: '4000$'
});
console.log(car.price); // 4000$
```

 **속성 기술자\(property descriptors\)**는 **데이터 기술\(data descriptors\)**와 **데이터 접근 기술\(accessor descriptors\)**로 나뉜다.

#### **1-2\) 데이터 기술\(data descriptors\)**

데이터 기술과 데이터 접근 기술은 모두 객체이면 다음과 같은 키를 공유한다.

| key |  default value | description |
| :--- | :--- | :--- |
| writable | false | 할당 연산자\(=\)를 통한 값을 변경 가능 여부. |
| enumerable | false | 객체의 속성으로 열거 가능 여부. |
| configurable | false | 객체의 속성 제거 가능 여부. |
| value | undefined | 객체의 속성 값 설정. |

#### 1-3\) 데이터 접근 기술\(accessor descriptors\)

데이터 접근 기술은 다음 키를 선택사항으로 가진다.

| key | default value | description |
| :--- | :--- | :--- |
| get | undefined | 속성에 설정된 값을 가져온다. |
| set | undefined | 속성의 값으로 할당. |

#### 2\)  Object.defineProperties\(obj, props\)

이미 존재하거나 새로운 프로퍼티들의 각종 속성들을 재정의 할 수 있다.

#### 3\) Object.preventExtensions\(\)

**객체의 확장 차단**하는 메서드로 새로운 속성이 이제까지 객체에 추가되는 것을 방지.

#### 4\) Object.isExtensible\(\)

**객체의 확장**이 가능한지 확인.

#### 5\) Object.seal\(\)

**객체를 밀봉**하는 메서드로 그 객체는 새로운 속성을 추가할 수 없고, 현재 존재하는 모든 속성을 설정 불가능 상태로 만들어준다. 하지만 쓰기 가능한 속성의 값은 밀봉 후에도 변경할 수 있다.

#### 6\) Object.isSealed\(\)

**객체가 밀봉** 됐는지 확인.

#### 7\) Object.freeze\(\)

객체를 동결하는 메서드로 동결된 객체의 속성은 지우거나 바꿀 수 없다. 즉 밀봉과 속성 값 변경이 차단된다.

#### 8\) Object.isFrozen\(\)

 객체가 동결 됐는지 확인.

### 4. 프로퍼티 삭제

delete 연산자는 객체의 프로퍼티를 삭제한다. 이 연산자는 프로퍼티의 값을 지우는 것이 아니라 프로퍼티를 지운다.

```javascript
let car = {
  type: 'normal',
  weels: 4,
  handle: 1,
  mirros: {
    side: 2,
    back: 1
  },
  engine: '3000cc',
  weight: '313kg',
  booster: false
};

delete car.booster;
console.log(car['booster']); // undefined
```

### 5. 프로퍼티 검사

객체의 `hasOwnProperty(`\)메서드는 주어진 이름의 프로퍼티가 객체에 존재하는지를 검사한다.

```javascript
let car = {
  type: 'normal',
  weels: 4,
  handle: 1,
  mirros: {
    side: 2,
    back: 1
  },
  engine: '3000cc',
  weight: '313kg',
  booster: false
};


delete car.booster;

console.log(car.hasOwnProperty('weight')); // true
console.log(car.hasOwnProperty('boster')); // false
```

### 6. 프로퍼티 열거

 for/in 문을 사용하면 객체가 가진 프로퍼티들을 쉽게 순회할 수 있다.

```javascript
let car = {
  type: 'normal',
  weels: 4,
  handle: 1,
  mirros: {
    side: 2,
    back: 1
  },
  engine: '3000cc',
  weight: '313kg',
  booster: false
}

for (let property in car) {
  console.log(`${property} : ${car[property]}`);
  // type : normal
  // weels : 4
  // handle : 1
  // mirros : [object Object]
  // engine : 3000cc
  // weight : 313kg
  // booster : fasle 
}
```

#### Reference

Object →[\(MDN\)](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Object#object_%EC%83%9D%EC%84%B1%EC%9E%90%EC%9D%98_%EB%A9%94%EC%84%9C%EB%93%9C)









 

#### 

