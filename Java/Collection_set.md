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
