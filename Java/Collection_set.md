# TIL

### 오늘은 Collection의 Set에대해서 공부하였다.

### 순서가 있는 목록 형 Set

### Set 인터페이스는 Collection 인터페이스를 확장함

## Hashset

- Object는 자바의 최상위 클래스로 모든 클래스는 Object를 상속 받는다. (HashCode 사용)
- Hash 란 입력값이 들어오면 특정 값으로 변환하여 반환한다.
- 원본을 HashCode를 이용하여 변환된 Integer 코드를 기준으로 데이터를 저장한다.
- 속도가 엄청 빠르다.
- Hashset 내부 코드에 구현체가 Hashmap 이다.

-> HashMap의 구조는 List의 Array이며 이렇게 구조되어진 이유는 Random Access가 가능하기 때문의
시간복잡도가 상수의 접근시간을 가지는것을 목표로 만들어 졌다. 해당 구조로 되었을때 문제는 Hash가 충돌하는 현상이 생기는데, 해당 충돌을 해결하기 위해 리스트 또는 트리를 통해 Array를 만든다.
