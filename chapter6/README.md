## 챕터 6 브루트 포스

### 6.3 소풍

오랜만에 알고리즘 문제였으나 문제 자체는 어렵지 않았다.<br>
다만 처음에 다차원 배열 할당할 때 요소들이 하나의 변수를 참조하여서 시간을 조금 허비했다.<br>
정리가 잘 되어있는 책으로 공부하니까 구글링으로 공부할 때 보다 정리가 되는 느낌이다.<br>

- 브루트 포스 알고리즘 사용시 완전 탐색을 위해 재귀 호출을 사용한다.
- 문제와 부분 문제를 나누는 연습을 한다.
- 중복 카운트를 피하기 위해 순서를 강제하면 된다.
- 주어진 조건(여기선 짝지을 수 있는 경우의 수)을 배열로 만든다.

### 6.5 게임판 덮기

시각적인 설명이 있으나 역시 특정한 규칙을 강제하면 쉽게 풀수 있다.

- 재귀 호출 각 단계마다 가장 윗 줄, 가장 왼쪽 칸을 덮도록 한다.(중복 카운트 방지)
- 칸을 덮는 함수 set 실행시 타입을 넣어줘서 덮어지는지 안되는지 불린값을 반환한다.
- set 실행시 실제 판을 수정한다. 추가와 삭제기능이 같이있다.(이미 채워진 칸을 삭제하는 것을 방지하기 위함)
- 덮는 함수 cover 에서 좌표를 찾고 set함수에 넣어 테스트한다.(테스트 후 항상 삭제하게 호출한다.)
