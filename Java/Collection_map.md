# TIL

### 오늘은 Map에 대해서 공부하였다.

## HashMap

-> Map은 키-값 쌍(key-value pairs)을 저장하는데 초점이 맞춰져 있고, 이와 관련된 메서드를 제공한다.

-> Map과 Collection은 서로 다른 용도로 설계된 인터페이스. 다만, Map은 keySet()이나 values(), entrySet()
같은 메서드를 통해 Collection을 반환할 수 있다. 이를 이용해 Map의 데이터에 대해 컬렉션 연산을 수행할 수 있다.

-> thread safe 하지 않다.

-> key에 null값 허용한다.

# HashMap 구동원리

-> HashMap의 구조는 List의 Array이며 이렇게 구조되어진 이유는 Random Access가 가능하기 때문의
시간복잡도가 상수의 접근시간을 가지는것을 목표로 만들어 졌다. 해당 구조로 되었을때 문제는 Hash가 충돌하는 현상이 생기는데, 해당 충돌을 해결하기 위해 리스트 또는 트리를 통해 Array를 만든다.
