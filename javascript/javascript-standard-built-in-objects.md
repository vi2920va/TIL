# JavaScript Standard built-in objects

### 기본 내장 객체\(Standard built in object\)

###  1. Number object

JavaScript는 다른 프로그램 언어와는 달리 정수 값과 실수 값을 구분하지 않고 모든 숫자들을 실수로 표현한다.  Number object는 최대값, 무한대 값, NaN\(Not a number\)를 위한 속성들이 있다.

#### 1\) Number object - properties

미리 정의된 숫자 객체의 속성\(properties\). 

| properties | description |
| :--- | :--- |
| Number.MAX\_VALUE | 표현 가능한 가장 큰수 \(±1.7976931348623157e+308\) |
| Number.MIN\_VALUE | 표현가능한 가장 작은 수\(±5e-324\) |
| Number.NaN | "숫자가 아닌" 특수값 |
| Number.NEGATIVE\_INFINITY | 음의 무한대 값 |
| Number.POSITIVE\_INFINITY | 양의 무한대 값 |
| Number.EPSILON | 표현 가능한 매우 작은 값\(2.220446049250313e-16\) |
| Number.MIN\_SAFE\_INTEGER | 안전한 최소의 정수.\(−253 + 1, or −9007199254740991\) |
| Number.MAX\_SAFE\_INTEGER | 안전한 최대의 정수.\(+253 − 1, or +9007199254740991\) |

#### 2\) Number object - method

| method | description |
| :--- | :--- |
| Number.parseFloat\(\) | 문자열을 파싱하여, 문자열에 포함된 숫자 부분을 실수 형태로 반환한다. |
| Number.parseInt\(\) | 문자열을 파싱하여, 문자열에 포함된 숫자 부분을 정수 형태로 반환한다. |
| Number.isFinite\(\) | 전달된 값이 유한한 수인지 아닌지를 검사한다. |
| Number.isInteger\(\) | 전달된 값이 정수인지 아닌지를 검사한다. |
| Number.isNaN\(\) | 전달된 값이 NaN인지 아닌지 검사한다. |
| Number.isSafeInteger\(\) | 전달된 값이 안전한 정수\(safe integer\)인지 아닌지를 검사한다. |

### 2. Math object

수학식에 대한 내장 객체.

#### 1\) Math object - method

| method | description |
| :--- | :--- |
| Math.min\(\) | 인수로 전달받은 값 중에서 가장 작은 수를 반환한다. |
| Math.max\(\) | 인수로 전달받은 값 중에서 가장 큰 수를 반환한다. |
| Math.random\(\) | 0 보다 크거나 같고 1보다 작은 랜덤 숫자를 반환한다. |
| Math.floor\(x\) | x와 같거나 작은 수 중에서 가장 큰 정수를 반환한다. |
| Math.round\(x\) | x를 소수점 첫 번째 자리에서 반올림하여 그 결과를 반환한다. |
| Math.ceil\(x\) | x와 같거나 큰 수 중에서 가장 작은 정수를 반환한다. |
| Math.abs\(x\) | x의 절대값을 반환한다. |
| Math.pow\(x,y\) | x의 y승을 반환한다. |
| Math.sqrt\(x\) | x의 제곱근을 반환한다. |
| Math.trunc\(x\) | x의 모든 소수 부분을 삭제하고 정수 부분만을 반환한다. |

### 3. Date object

JavaScript는 날짜 데이터 타입 없기 때문에 Date object를 사용하여 프로그램에서 날짜와 시간 처리를 한다.

### 4. String object

JavaScript는 다른 언어 달리 단따옴표\('\), 쌍따옴표\("\) 문자열 간의 차이점이 없다.

#### 1\) 문자열 객체에 접근

문자열에서 개개의 문자에 접근할 수 있는 방법은 `charAt()`메서드를 이용하는 것과 문자에 해당하는 숫자 인덱를 사용하는 방법 두 가지가 있다.

```javascript
let string_text = 'I am JavaScript';
console.log(string_text.charAt(1));
console.log(string_text[5]);
```

#### 

