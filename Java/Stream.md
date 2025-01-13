# TIL

### 오늘은 Stream 에대해서 공부하였다.

## 스트림은 Java 8 에 도입된 컬렉션 데이터를 처리하기 위한 API 이다.

# 스트림은 내부 반복자로 컬렉션에 있는 데이터를 처리 하기 쉽게 나왔으며, 가독성과 로직을 구현하기 좋고 병렬처리에도 유리하다.

![alt text](image.png)

## 병렬 스트림 특징

- 병렬 스트림은 내부적으로 Fork/Join Framework를 사용해 작업ㅇ르 분할하고 병렬로 실행

- 기본적으로 CPU 코어 수에 따라 작업이 분할

- ArrayList나 배열은 쉽게 분할되지만, LinkedList는 분할 비용이 높습니다.

## 자주 사용 하는 스트림 명령들

### toMap

- Java 8의 Stream API에서 제공하는 메서드로, 스트림의 요소를 Map으로 변환하기 위한 Collector를 생성하며이를 사용하면 스트림의 데이터를 원하는 방식으로 키와 값을 매핑하여 맵을 생성할 수 있다.

- 동작 순서로는 스트림 생성 -> KeyMapper 호출 -> valueMapper 호출 -> 맵에 키-값 추가 (중복시 IllegalStateException) 발생 -> 최종적으로 생성된 Map<K, U> 반환.

### 메서드 정의

![alt text](image.png)

### 예제

![alt text](image.png)

### groupingBy

- Java 8의 Stream API에서 제공하는 Collector 중 하나로, 데이터를 특정 기준으로 그룹화하여 Map으로 반환. SQL의 GROUP BY와 비슷한 기능을 Java 스트림에서 구현할 수 있도록 도와준다.

### 예제

![alt text](image.png)
