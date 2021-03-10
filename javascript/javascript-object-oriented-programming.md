# JavaScript Object oriented programming

## 객체 지향 프로그래밍\(Object oriented programming\)

 객체 지향 프로그래밍은 프로그램 설계 방법론의 일종이다. 프로그래밍 할 때 프로그램을 단순히 데이와 처리 방법으로 나누는 것이 아닌 객체\(object\)라는 단위로 나누고 이를 서로 상호 작용 할 수 있게 만들어 주는 역할을 수행한다. 이 방식은 오늘 날 가장 많이 대표적인 프로그래밍 방식이고 JAVA, C\# 등 대표적인 프로그래밍 언어이다. 객체 지향 프로그래밍 특징은 아래와 같다.

1. **캡슐화\(Encapsulation\)**

   캡슐화는 관련있는 멤버 변수와 메서드를 클래스와 같은 하나의 틀 안에 담고 외부에 공개될 필요가 없는 정보는 숨기는 것을 말하며 다른 말로는 **정보 은닉\(information hiding**\)이라고 한다.

2. **추상화\(Abstraction\)**

   추상화는 객체를 만들 때 복잡한 원리나 구동 방식을 사용자로부터 추상화 시켜주는 작업을 추상화라고 한다. 즉, 우리가 만든 객체를 사용자들이 쉽게 쓰드록 해주는 것.

3. **다형성\(Polymorphism\)** 자식 클래스가 부모 클래스에 상속을 받게 되면 부모 클래스의 속성과 기능을 그대로 물려 받게 된다. 자식 클래스는 같은 메서드 일지라도 상황에 맞게 다르게 구현할 수 있다. 이를 다형성이라고 한다.

### 1. 객체 지향 용어

| title |  | example |
| :--- | :--- | :--- |
| Class | 객체의 속성\(properites\)을 정의. | 설계 도면 |
| Object | Class의 인스턴스\(Instance\). | 설계 도면을 통해 구현된 실제 제품 |
| Property | 객체의 속성. | color 등과 같은 명사 형태 |
| Method | 객체의 기능. | walk\(\) 등과 같은 동사 형태 |
| Constructor | 인스턴스 생성 순간에 호출 실행되는 메서드. |  |
| Inheritance | Class는 다른 Class로 부터 속성들을 상속 받을 수 있다. \(Super Class → Sub Class\) |  |
| Encapsulation | Class는 해당 객체의 속성, 메서드만 정의할 수 있다. \(외부 접근 불가\) |  |
| Abstraction | 복잡한 상속, 메서드, 객체의 속성의 결합은 반드시 현실 모델을 시물레이션 할 수 있어야 한다. |  |
| Polymorphism | 다른 Class들이 같은 메서드나 속성으로 정의될 수 있다. |  |

### 1. 생성자 함수와 인스턴스의 생성

 JavaScript는 생성자 함수와 new 연사자를 통해 인스턴스를 통해 생성할 수 있다. 이때 생성자 함수는 클래스 이면서 생성자 역할을 한다.

```javascript
// constructor
function Person(name) {
  // property
  this.name = name;

  // method
  this.greething = function () {
    console.log(`Hi! I' m ${this.name}.`);
  };
}

let teacher = new Person('Diana');
teacher.greething(); // Hi I' m Diana

let student = new Person('Bob');
student.greething(); // Hi I' m Bob
```

위의 예제 코드에서 Person\(\) 생성자 함수로 여러 개의 인스턴스를 생성하게 되면 각 인스턴스가 내용일 동일한 메서드를 각자 소유하게 된다. 이는 메모리 낭비로 생성되는 인스턴스가 많아지거나 메서드가 크거나 많다면 결코 무시할 수 없는 문제가 된다. 이를 해결 위한 문제로는 프로토타입 접근 방식으로 접근해야 한다.

### 2. 프로토타입 체인과 메서드

모든 객체는 '[프로토타입\(prototype\)](https://poiemaweb.com/js-prototype)'이라는 다른 객체를 가리키는 내부 링크를 가지고 있다. 즉, 프로토타입을 통해 직접 객체를 연결할 수 있는데 이를 '프로토타입 체인\(prototype chain\)'이라고 한다. 

 프로토타입을 이용하여 생성자 함수 내부의 메서드를 함수의 프로퍼티\(property\)가 가리키는 프로토타입 객체로 이동시키면서 생성자 함수에 의해 생성된 모든 인스턴스는 프로토타입 체인을 통해 프로토타입 객체의 메서드를 참조할 수 있다.

```javascript
function Person(name) {
  this.name = name;
}

Person.prototype.greething = function () {
  console.log(`Hi! I' m ${this.name}.`);
};

let teacher = new Person('Diana');
let student = new Person('Bob');

console.log(teacher); // Person{name: 'Diana'}
console.log(student); // Person{name: 'Bob'}
```

아래는 더글라스 크락포드가 제안판 프로토타입 객체에 메서드를 추가하는 방식.

```javascript
/**
 * 모든 생성자 함수의 프로토타입은 Function.prototype이다.
 * 따라서 모든 생성자 함수는 Function.prototype.method()에 접근 가능.
 * @method Function.prototype.method
 * @param ({string}) (name) - (메서드 이름)
 * @param ({function}) (func) - (추가할 메소드 본체)
 */
Function.prototype.method = function (name, func) {
  // 생성자함수의 프로토타입에 동일한 이름의 메서드가 없으면 생성자함수의 프로토타입에 메서드를 추가
  // this: 생성자함수
  if (!this.prototype[name]) {
    this.prototype[name] = func;
  }
};

/**
 * constructor
 */
function Person(name) {
  this.name = name;
}

/**
 * constructor - method
 */
Person.method('greeting', function () {
  console.log(`Hi! I' m ${this.name}.`);
});

let teacher = new Person('Diana');
let student = new Person('Bob');

console.log(teacher); // Person{name: 'Diana'}
console.log(student); // Person{name: 'Bob'}

```





#### 



