# Ajax 개요

## Ajax

Ajax는 JavaScript의 라이브러리 중 하나이며 **Asynchronous Javascript And XML\(비동기식 자바스크립트와 XML\)**의 약자이다. 브라우저가 가지고 있는 **`XMLHttpRequest`** 객체를 이용해서 전체 페이지를 새로 고치지 않고도 페이지의 일부만을 위한 데이터를 로드하는 기법 이며 Ajax를 한마디로 정의하자면 **JavaScript를 사용한 비동기 통신, 클라이언트와 서버 간에 XML 데이터를 주고받는 기술**이라고 할 수 있겠다.

#### 1\) Ajax  장점

* 요청과 응답을 과정을 통해 불필요한 부분까지 처리하지 않는다.
* 즉, 필요한 부분만 별도로 요청 가능하다.
* 모든 데이터가 업데이트 될 필요 없으므로 불필요한 대역폭 감소 가능하고 비용 절감의 효과를 볼 수 있다.
* 사용자의 대기시간 감소, 페이지를 새로고침 하지 않고도 필요한 데이터의 내용을 업데이트 가능하다.
* 기존의 동기 방식이 아닌, 비동기식 방식으로 데이터\(data\)를 요청 및 처리 하기 때문이다.
* Ajax를 사용해서 전송한 가능한 데이터는 XML, TEXT, HTML, JSON 등이 있다.

### 1. XMLHttpRequest Object

Ajax는 비동기 통신을 위해서는 XHR\(XMLHttpRequest\) 객체를 사용해야 한다. XHR 객체는 생성자 함수 이기 때문에 반드시 new 키워드를 통해서 생성해야 한다. XHR객체가 요청\(request\)을 하게 되면 응답\(response\)를 받아온다.

{% code title="Sytax" %}
```javascript
let xhr = new XMLHttpRequest();
```
{% endcode %}

#### 1\) 서버 요청\(Request\)

Ajax에서 XMLHttpRequest 객체를 사용하여 서버와 데이터를 교환한다. 따라서 서버에 요청을 보내기 위해서는 XMLHttpRequest 객체를 생성하고 난 후에 open\(\), send\(\) 메서드를 사용하여 요청을 보낼 수 있다. 여기서 open\(\) 메서드는 서버로 요청을 준비하기 위한 설정을 말하고, send\(\)메서드는 준비된 요청을 서버에 전달한다.

{% code title="Sytax" %}
```javascript
let xhr = new XMLHttpRequest();
xhr.open(method, url[, async]);
xhr.send();
```
{% endcode %}



