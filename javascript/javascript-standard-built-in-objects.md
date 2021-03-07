# JavaScript Standard built-in objects

### 기본 내장 객체\(Standard built in object\)

###  1. Number Object

JavaScript는 다른 프로그램 언어와는 달리 정수 값과 실수 값을 구분하지 않고 모든 숫자들을 실수로 표현한다.  Number object는 최대값, 무한대 값, NaN\(Not a number\)를 위한 속성들이 있다.

#### 1\) Number object - properties

미리 정의된 숫자 객체의 속성\(properties\). 

| properties | 설명 |
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

| method | 설명 |
| :--- | :--- |
| Number.parseFloat\(\) | 문자열을 파싱하여, 문자열에 포함된 숫자 부분을 실수 형태로 반환한다. |
| Number.parseInt\(\) | 문자열을 파싱하여, 문자열에 포함된 숫자 부분을 정수 형태로 반환한다. |
| Number.isFinite\(\) | 전달된 값이 유한한 수인지 아닌지를 검사한다. |
| Number.isInteger\(\) | 전달된 값이 정수인지 아닌지를 검사한다. |
| Number.isNaN\(\) | 전달된 값이 NaN인지 아닌지 검사한다. |
| Number.isSafeInteger\(\) | 전달된 값이 안전한 정수\(safe integer\)인지 아닌지를 검사한다. |



