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

어떤 문장에라도 그 앞에 식별자 이름과 콜론\(:\) 을 넣음으로써 레이블\(labeled\)을 붙일 수 있다.  어떤 문장에 레이블을 붙이면 프로그램의 다른 곳에서도 그 문장을 참고할 수 있는 이름이 생기는 셈이다. 레이블은 어떤 문장에라도 붙일 수 있다. 하지만 루프 또는 조건문 같이 몸체가 있는 문장에 쓰는 편이 유용하다.

```javascript

```

####  4\) break statement



```javascript

```

#### 5\) continue **statement**



#### 

#### 6\) 

