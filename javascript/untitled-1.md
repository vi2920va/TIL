---
description: 'JavaScript function call, apply, bind'
---

# 함수 호출

### 1. call 

함수를 호출 할 때, 첫 번째 인자에 `this`키워드 설정, 두 번째 부터는 **배열이 아닌 각 인자**로 받는다.

```text
func.call(thisArg[, arg1[, arg2[, ...]]])
```

### 2. apply 

함수를 호출 할 때,  첫 번째 인자 `this` 키워드 설정, **두 번째 인자로는 배열** 받는다.

```text
func.apply(thisArg, [argsArray])
```

### 3. bind

`bind`  method가 호출되면 **새로운 함수를 생성**, 첫 번째 인자 `this` 키워드 설정, 나머지 인자들은 `bind`된 함수의 인수로 제공된다.

```text
func.bind(thisArg[, arg1[, arg2[, ...]]])
```

#### Reference

bind [→\(MDN](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Function/bind)\)

