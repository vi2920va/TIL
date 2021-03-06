# JavaScript Array

## 배열\(Array\)

**배열\(array\)**은 정렬된 값의 집합이다. 배열 안의 각 값은 **요소\(element\)**라고 한다. 각 요소는 배열에서 위치를 가리키는 번호를 배정 받는데, 이를 **인덱스\(index\)**라고 한다. JavaScript에서는 배열은 타입이 고정되어 있지 않다. 즉, 같은 배열에 있는 요소는 값의 타입은 서로 다를 수 있다. 배열의 요소는 객체가 될 수도 있고, 또 다른 배열이 될 수도 있다. 

### 1. 자주 사용하는 연산

####  1\) 배열 만들기

배열을 만드는 가장 쉬운 방법은 배열 리터럴을 사용하는 것이다. 배열 리터럴은 대괄호\(`[ ]`\) 안에 배열의 요소를 쉼표\(`,`\)로 구분해 나열하는 것.

```javascript
let misc = [1, true, 'a'];
console.log(misc.length); // 3
```

**2\)  인덱스로 배열의 요소에 접근**

배열의 각 요소에 접근할 때에는 `[ ]` 연산자를 사용한다. `[ ]` 연산자 왼쪽에는 배열 참조 변수가 와야하며, `[ ]`안에는 정수값으로 평가되는 임의의 표현식이 위치할 수 있다. JavaScript는 사용자가 명시한 숫자 배열 인덱스를 문자열 형태로 바꿔서 프로퍼티 이름으로 사용한다. 

```javascript
let first = misc[0]; // 1

let last = misc[misc.length - 1]; // 'a'
```

#### 3\) 배열의 요소들을 순환하며 처리

`forEach()` 메서드는 배열을 순회하는 메서드로, 첫 번째는 인자로 넘긴 함수를 각각의 요를 대상으로 호출한다.  `forEach()`는 첫 인자로 전달된 함수를 호출할 때 세 가지 인자를 넘긴다. 각 인자는 배열의 요소 값과,  요소의 인덱스 값, 그리고 배열 그 자체다.

```javascript
misc.forEach(function(item, index, array){
  console.log(item, index); 
  // 1 0
  // true 1
  // 'a' 2
})
```

#### 4\) 배열 끝에 요소 추가

JavaScript의 배열로 **FILO\(First-in, Last-out\)** 스택을 구현할 수 있다. `push()`메서드는 하나 이상의 받은 요소들을 배열 끝부분에 추가한다.

```javascript
let newLength = misc.psuh('java'); // [1, true, 'a', 'java']
```

####  5\) 배열 끝에서부터 요소 제거

`pop()`메서드는 `push()`메서드와 반대로 배열의 마지막 요소를 제거.

```javascript
let last = misc.pop(); // [1, true, 'a'] 
```

####  6\) 배열 앞에서 요소 제거

`shift()` 메서드는`pop()`메서드와 유사하게 동작하는데, 배열의 끝이 아니라 배열의 맨 앞에서 요소를 제거하는 점이 다르다.

```javascript
let first = misc.shift(); // [true, 'a']
```

#### 7\) 배열 앞에 요소 추가

`unshift()`메서드는 `push()` 메서드와 유사하게 동작, 배열의 맨 앞에 요소를 추가.

```javascript
let newLength = misc.unshift(101); // [101, true, 'a']
```

#### 8\) 배열 안에서 요소의 인덱스 검색

`indexOf()`메서드는 배열의 요소 중에서 특정한 값을 찾는다. 값이 존재하면 해당 인덱스를 반환하고, 존재하지 않을 경우에는`-1`를 반환한다.

```javascript
let str = misc.indexOf('a'); // 2
```

#### 9\) 인덱스 위치에 있는 요소 제거

`Array.splice()`메서드는 배열의 요소를 삽입하거나 요소를 제거하려 할 때 범용적으로 사용할 수 있는 메서드이다. `splice()` 메서드는 `slice(), concat()` 메서드와는 달리 호출 대상 배열을 바로 수정한다. `slice()`와 이름이 유사하지만, 수행하는 작업은 완전히 다름을 유념하자.

```javascript
let removeItem = misc.splice(str, 1); // [101, true]
```

#### 10\) 인덱스 위치에서 부터 여러개의 요소 제거

splice\(\) 메서드의 첫 번째 전달인자는 배열에서 삽입 또는 삭제할 위치를 지정하며, 두 번째 전달인자는 배열에서 삭제할 요소의 개수를 지정.

💻 배열의 삭제 →[\(GITBOOK\)](https://app.gitbook.com/@vi2920va/s/algorithm-javascript/chapter1-1/1)

#### 11\) 배열 복사

Array.slice\(\) 메서드는 부분 배열을 반환한다. 여기서 "부분 배열"이란 배열에서 잘라낸 요소들을 새 배열 이다. slice\(\) 메서드는 전달인자를 두 개 받는데, 각 인자는 반환될 부분의 처음과 끝을 명시한다. 반환되는 배열은 첫 번째 전달인자가 지정하는 위치부터 두 번째 전달인자가 지정하는 위치 이전 까지의 모든 요소들을 포함한다.

```javascript
let shallowCopy = misc.slice(); // [101, true] 
```

###  2. 배열 요소에 접근

배열의 인덱스는 0부터 시작한다. 즉, 배열의 첫 번째 요소는 0이고, 마지막 요소의 인덱스는 배열의 length - 1과 같다. 잘못된 인덱스를 사용하년 undefined를 반환한다. 

```javascript
let arr = ['item1','item2', 'item3'];
console.log(arr[0]); // item1
console.log(arr[arr.legnth - 1]); // item3
```

### 3. length 와 숫자형 속성의 관계

배열의 내장 메서드 join, slice, indexOf 등은 호출 했을 때 배열의 length 속성 값을 참조한다.  length 속성은 직접 늘릴 수도 있고, length 속성을 감소시키면 요소를 제거하게 된다.













\*\*\*\*

