# 오늘은 스프링 공부전 JVM 메모리 구조를 다시 공부했다.

## Method Area(메소드 영역)

- 모든 스레드가 공유하는 영역.

- 클래스에 대한 메타데이터와 정적 멤버(static), 런타임 상수 풀(Runtime Constant Pool)이 저장됩니다.

- 클래스 로드 시 한 번만 로드되며, 프로그램 종료 시까지 유지됩니다.

## Heap Area(힙 영역)

- 모든 스레드가 공유하는 영역.

- 객체와 배열이 저장되는 영역.

- 객체는 동적으로 생성되며, JVM의 **가비지 컬렉터(GC)**가 관리.

- Young Generation: 새롭게 생성된 객체가 저장.
- Eden: 새로 생성된 객체.
- Survivor 1, Survivor 2: Eden에서 살아남은 객체.
- Old Generation (Tenured): Young Generation에서 오래된 객체가 이동.
