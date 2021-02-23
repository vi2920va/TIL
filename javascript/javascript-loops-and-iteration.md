# JavaScript Loops and iteration

### 1. LOOPS AND ITERATION

루프\(Loop\)는 어떤 것을 반복적으로 시행할 때 빠르고 간편한 제공한다. JavaScript가 제공하는 반복문은 아래와 같다.

* for statement
* do/while statement
* while statement
* label statement
* break statement
* continue statement
* for/in statement
* for/of statement

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

반복문에 레이블\(label\)을 붙이고, break 나, continue 구문을 사용해 반복문의 어느 위치에서 작업을 멈추고 어느 위치에서 다시 수행할지 알려줄 수 있다.

```javascript

```

####  4\) break statement

 `break`문은 현재 반복문, switch 문, 또는 label 문을 종료하고, 그 다음 문으로 프로그램 제어를 넘긴다.

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



#### 

#### 6\) 

