# TIL

# Http

- 웹은 HTTP를 기반으로 통신한다. (클라이언트에서 서버로 데이터를 전송할 때, 그리고 서버에서 클라이언트로 데이터를 응답할 때, 모두 HTTP 프로토콜을 기반으로 동작한다.) 모든 것이 HTTP - HTTP 메시지에 모든 것을 전송

- HTML, TEXT ,IMAGE, 음성, 영상, 파일 ,JSON, XML (API) 거의 모든 형태의 데이터 전송 가능

- 서버간에 데이터를 주고 받을 때도 대부분 HTTP 사용

## WEB-SERVER (웹 서버)

- HTTP 기반으로 동작

- 정적 리소스 제공, 기타 부가기능

- 정적(파일) HTML, CSS, JS, 이미지, 영상

- 예: NGINX, APACHE

## WAS (웹 어플리케이션 서버)

- HTTP 기반으로 동작

- 웹 서버 기능 포함+ (정적 리소스 제공 가능) 프로그램 코드를 실행해서 애플리케이션 로직 수행

- 동적 HTML, HTTP API(JSON)

- 서블릿, JSP, 스프링 MVC

- 예: 톰캣(Tomcat)

## WAS / WEB-SERVER 차이점

- 웹 서버는 정적 리소스(파일), WAS는 애플리케이션 로직

- 웹 서버도 프로그램을 실행하는 기능을 포함하기도 함.

- 웹 애플리케이션 서버(WAS)도 웹 서버의 기능을 제공함.
- 자바는 서블릿 컨테이너 기능을 제공하면 WAS. 서블릿 없이 자바코드를 실행하는 서버 프레임워크도 있음

- WAS는 애플리케이션 코드를 실행하는데 더 특화되어 있다.
  (크게는, 웹 서버는 정적 리소스(파일)를 제공하는 서버, WAS는 애플리케이션 로직을 실행하는 서버.)
