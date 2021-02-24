# JavaScript Loops and iteration

### 1. LOOPS AND ITERATION

루프\(Loop\)는 어떤 것을 반복적으로 시행할 때 빠르고 간편한 제공한다. JavaScript가 제공하는 반복문은 아래와 같다.

* **for statement**
* **do/while statement**
* **while statement**
* **label statement**
* **break statement**
* **continue statement**
* **for/in statement**
* **for/of statement**

#### 1\) while statement

`while`문은 조건이 거짓\(false\)로 판별될 때 까지 반복.

```javascript
let while_condition = true;
let count = 0;

while (while_condition) {
  count = count + 1; // 1, 2, 3, 4, 5, 6, ....
  console.log(count);
  if (count > 5) {
    while_condition = false;
  }
}
```

#### 2\) do/while statement

while문은 조건이 거짓이면 반복되지 않는다. 반면에 do/while문은 조건이 거짓일지라도 최소 1회는 실행한다는 차이점을 가지고 있다.

```javascript
do {
  console.log("조건이 거짓이면 실행되지 않는다.");
} while (false);
```

#### 3\) label statement

반복문에 레이블\(label\)을 붙이고, `break` 나, `continue` 구문을 사용해 반복문의 어느 위치에서 작업을 멈추고 어느 위치에서 다시 수행할지 알려줄 수 있다.

```javascript
loop1: for (let i = 0; i < 3; i++) {
  loop2: for (let j = 0; j < 3; j++) {
    if (i === 1 && j === 1) {
      continue loop1;
    }
    console.log(`i = ${i}, j =${j}`);
  }
}

```

####  4\) break statement

 `break`문은 현재 반복문, `switch`문, 또는 `label`문을 종료하고, 그 다음 문으로 프로그램 제어를 넘긴다.

```javascript
let i = 0;

while (i < 6) {
  if (i === 3) {
    break;
  }
  i = i + 1;
}

console.log(i);
```

#### 5\) continue **statement**

`continue` 문은 현재 또는 레이블이 지정된 루프의 현재 반복에서 명령문의 실행을 종료하고 반복문의 처음으로 돌아가면 루프문의 다음 코드를 실행한다. 

`break`문과 달리 `continue`는 루프의 실행을 완전히 종료하지 않고 `for`, `while`문에서 다음과 같이 동작한다.

* `while` 루프에서는 다시 조건으로 점프한다.
* `for`루프에서는 업데이트 표현식으로 점프한다.

```javascript
let text = '';

for (let i = 0; i < 10; i++) {
  if (i === 3) {
    continue;
  }
  text = text + i;
}

console.log(text);
```

#### 6\) for statement

for 반복문은 어떤 특정한 조건이 거짓으로 판별될 때까지 반복한다. C 언어의 반복문과 비슷하다.

```javascript
// for ([초기문]; [조건문]; [증감문]) { ... }
for (let i = 0; i < 10; i++) {
  console.log(i);
}

// 콤마(,)를 사용해서 변수와 증가에 대한 부분을 묶어서 사용.
for (let i = 0, j = 4; i < 10; ++i, j -= 2) {
  if (j > 0) {
    console.log('j :', j);
    continue;
  }
  console.log('i :', i);
}
```

#### 7\) for/in statement

`for/in`문은 상속된 열거 가능한 속성들을 포함하여 객체에서 문자열로 키가 지정된 모든 열겨 가능한 속성에 대해 반복한다.

```javascript
const object = { a: 1, b: 2, c: 3 };

for (const property in object) {
  console.log(`${property}: ${object[property]}`);
}
```

#### 8\) for/of statement

`for/of`문은 반복 가능한 객체\(`Array`, `Map`, `Set`, `String`, `TypeArray`, `arguments` 객체 등을 포함\)에 대해서 반복하고 각 개별 속성값에 대해 실행되는 문이 있는 사용자 정의 반복 후크를 호출하는 루프를 생성한다.

```javascript
const array1 = ['a', 'b', 'c'];

for (const element of array1) {
  console.log(element);
}
```

#### Reference

루프와 반복 \(Loops and iteration\) [→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Loops_and_iteration)

codepen.io에서 무한 루프에 빠져 브라우저가 다운되는 경우 해결[ →\(SITE\)](https://blog.codepen.io/documentation/features/turn-off-javascript-in-previews/)

