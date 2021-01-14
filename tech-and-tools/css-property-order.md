# CSS PROPERTY ORDER

### 1. PROPERTY ORDER

CSS 속성은 보통 편한대로 적을 수 있다. 왜냐하면 딱히 규칙이 없기 때문이다. 그래서 협업 할 때에 다른 사람이 작업한 CSS Stylesheet를 보면 분석하느라 시간이 많이 소모되기도 한다. 

지금 정리하는 CSS 속성 순서는 모질라\(mozilia\), 네이버\(naver\)에서 기술해서 쓰는 CSS 속성 순서이다.

#### 1\) mozila

모질라에서 제안한 CSS 속성 기술 순서로 위치 &gt; 윤곽 &gt; 외곽 &gt; 디테일 &gt; 채색 &gt; 타이포그래피와 같이 밖에서 부터 안쪽의 흐름.

1. display - 객체의 노출여부/표현방식
2. list-style
3. position - 위치/좌표
4. float
5. clear 
6. width / height - 크기/여백
7. padding / margin
8. border / background -윤곽/배경
9. color / font - 글자/정렬
10. text-decoration
11. text-align / vertical-align
12. white-space
13. other text
14. content - 내용

#### 2\) naver

네이버에서 제안한 CSS 속성 기술 순서.

1. display - 표시
2. overflow - 넘침
3. float - 흐름
4. position - 위치
5. width/height - 크기
6. padding/margin - 간격
7. border - 테두리
8. background - 배경
9. color/font - 글꼴
10. animation
11. 기타 



