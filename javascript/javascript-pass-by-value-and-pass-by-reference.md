# JavaScript Pass by value and Pass by reference

### 1. 값 복사\(Pass by value\)

불변\(immutable\) 데이터 경우 그 값이 복사 된다. 변수에 할당된 값이 변경되었을 때, 다른 변수에 담긴 값이 변경되지 않았단 것은 값이 복사 되었음을 의미한다. 

```javascript
const repeating_count = 3;
const display_headline_content = "값 복사 vs 값 참조";
const is_toggle_menu = false;

// a에 repeating_count를 할당, repeating_count 값은 변경되지 않는다.
let a = null;
a = repeating_count;
a += 6;
console.log(`a : ${a}, repeating_count : ${repeating_count}`);

// replace()- 문자열 변경 메소드
let b = display_headline_content;
b = b.replace("복사", "copy");
console.log( `b : ${b}, display_headline_content : ${display_headline_content} `);

let d = is_toggle_menu;
d = !d;
console.log(`d : ${d}, is_toggle_menu : ${is_toggle_menu}`);
```

### 2. 값 참조\(Pass by reference\)

 가변\(mutable\) 데이터의 경우 그 값이 참조된다. 변수에 참조된 값이 변경되었을 때, 다른 변수에 담긴 값이 변경된다면 값이 참조되었음을 의미한다.

```javascript
let my_family = {
  size: 4,
  moto: "정직하게 살자",
  members: ["아버지", "어머니", "나", "동생"],
  getMembers: function () {
    return this.members;
  },
  addMembers: function (new_member) {
    this.members.push(new_member);
  }
};

let home_tasks = ["청소기 돌리기", "침구류 정리", "화장실 청소", "설거지", "분리수거"];

// j에 my_family를 할당 했기 때문에 j 또한 my_family를 객체를 가리킨다.
let j = my_family;
j.size = 6;
j.members = ["나", "아버지", "어머니", "고양이"];

let p = home_tasks;
p.pop();

// unshift: 배열 앞에 데이터 추가
home_tasks.unshift("마당 쓸기");

// for문 이용한 배열 복사
var name = ["영희", "철수", "기철", "난희", "숙희"];
for (let my_friends = [], i = 0; l = name.length, i < l; ++i) {
  my_friends[i] = name[i];
}

// 참조형 데이터 복사
let y = {};
for (var prop in my_family) {
  console.log(my_family[prop]); // prop - 속성 값
  y[prop] = my_family[prop];
}
```

