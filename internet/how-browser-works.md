---
description: 브라우저의 작동원리
---

# How browser works ?

### Browser 개요

브라우저\(browser\)의 핵심 기능은 사용자가 보고자 하는 페이지를 서버에 요청하고 서버로 부터 받은 응답을 브라우저에 표시하는 것이다.

### Browser의 기본 구조

![&#xC6F9; &#xBE0C;&#xB77C;&#xC6B0;&#xC800;&#xC758; &#xAE30;&#xBCF8; &#xAD6C;&#xC870;](../.gitbook/assets/layers.png)

* User Interface
  * 주소창, 이전/다음 버튼, 북마크 메뉴 등을 포
* Browser Engine
  * UI와 렌더링 엔진\(rendering engine\)사이에서 중간 매체 역할을 수
* Rendering Engine
  * 웹 서버로 부터 응답 받은 내용은 UI 상에서 나타내주는 렌더링 엔
  * 사용자 요청해서 웹 서버가 응답한 HTML문서를 HTML과 CSS로 파싱해서 화면을 구성.
* Networking
  * 웹 서버와 통신이 가능하게 하는 네트워
* UI Backend
  * UI 구동이 가능하게 하는 UI 백엔
* JavaScript Interpreter
  * JavaScript 코드를 파싱하고 실행하는 자바스크립트 해석
* DataPersistence
  * 쿠키와 로컬 데이터를 저장하는 데이터 스토리지\(data storage\)로 구성된다.

### Rendering engine

렌더링 엔진의 역할은 요청 받은 내용을 브라우저 화면에 표시하는 일이다.





