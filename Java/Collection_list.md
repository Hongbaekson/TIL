# TIL

### 오늘은 Collection의 List에대해서 공부하였다.

### 순서가 있는 목록 형 List

### List 인터페이스는 Collection 인터페이스를 확장함

## ArrayList

- 내부적으로 동적 배열(Dynamic Array)을 사용
- 요소가 추가될 때 내부 배열 크기가 부족하면 새로운 배열을 생성한 뒤 기존 요소를 복사하는 방식으로 확장.
- public Object clone() {} 으로 선언 되어있다.
- Random Aceess 가능

## LinkedList

- 내부적으로 이중 연결 리스트(Doubly-Linked List)를 사용.
- 요소가 추가/삭제될 때 노드 연결만 바꿔주면 되므로 특정 위치에서의 삽입/삭제가 빈번한 경우 유리.
- 하지만 인덱스로 접근하는 get(index) 연산은 O(n) 시간 복잡도를 가지므로 랜덤 접근에 비효율적이다.
- 하나의 노드가 다음 노드의 참조값을 가지고 있다. 체인처럼 연결 되어있다.
- Random Access가 불가능하다.

## Vector

- ArrayList와 유사하게 동적 배열을 내부적으로 사용합니다.
- 큰 차이는 **Vector는 모든 메서드가 Synchronized(동기화)**되어 있어 **멀티쓰레드 환경에서 안전(Thread-safe)**합니다.
- 하지만 동기화 비용 때문에 단일 스레드 환경에서는 ArrayList보다 성능이 떨어집니다.

- public synchronized Object clone() {} 으로 선언 되어있다.
