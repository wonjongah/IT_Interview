##### XML(Extensible Markup Language)

- 데이터를 나타낼 수 있는 방식 중 대표적인 것이 xml과 json이다.
- html과 유사한 문법이지만, 정해진 태그가 없어 자유롭게 태그 이름을 정해 사용할 수 있다.
- 최근 파싱의 느린 성능과 보안 이유로 json으로 대체되고 있는 추세이다.
- xml은 W3C에서 개발된, 다른 특수한 목적을 갖는 마크업 언어를 만드는데 사용하도록 권장하는 다목적 마크업 언어이다.



##### XML 문법

| 문법      | 설명                                                         |
| --------- | ------------------------------------------------------------ |
| <xml>     | xml 문서는 맨 첫 줄에 <xml> 태그를 사용해 xml 문서임을 명시한다. <?xml version="XML 문서 버전" encoding="문자셋" standalone="yes\|no"?>, 소문자만 사용, standalone 속성은 xml 문서가 외부 DTD(Document Type Definition)에 의존 여부를 xml 파서에 알려주며 기본값은 no이다. |
| 종료 태그 | 모든 xml 요소는 종료 태그를 가지며 태그는 대소문자까지 구분, 빈 태그에도 반드시 슬래시(/)를 추가해야 한다. <lecture>이 요소는 lecture 요소입니다.</lecture> |
| 순서      | 태그를 여닫는 순서를 반드시 지켜야 한다. <p><string>순서를 정확히</string></p> |
| 속성      | xml에서 속성은 반드시 따옴표로 감싸야 한다. <student name="장길산"> |
| 띄어쓰기  | html은 띄어쓰기를 인식하지 않으나, xml은 띄어쓰기를 인식한다. |
| 엔티티    |                                                              |



##### JSON(JavaScript Object Notation)

- json은 데이터를 저장하거나 전송할 때 많이 사용되는 경량의 DATA 교환 형식이다.
- json 표현식은 사람과 기계 모두 이해하기 쉬우며 용량이 작고 파싱이 빨라 xml을 대체해서 데이터 전송 등에 많이 사용한다.
- json은 일종의 데이터 포맷으로 단순히 데이터를 표시하는 표현 방법이다.



##### JSON 문법

- json 형식은 자바스크립트 객체와 마찬가지로 key/value가 존재할 수 있으며, key 값이나 문자열은 항상 쌍 따옴표를 이용해 표기해야 한다.
- 객체, 배열 등의 표기를 사용할 수 있다.
- 일반 자바스크립트의 객체처럼 원하는 만큼 중첩해 사용할 수도 있다.
- null, number, string, array, object, boolean을 사용할 수 있다.



##### SOAP(Simple Object Access Protocol)의 개념

- xml과 http 통신을 기반으로 해 <u>네트워크 상에 존재하는 각종 컴포넌트 간 호출을 효율적으로 실현하기 위한 방법을 제시하는 규약</u>이다.
- <u>네트워크상에서 Client와 Service 간에 메시지를 요청하고 이에 응답해주는 방법을 제공</u>한다.



##### SOAP의 특징

- 기존 Remote Procedure Calls의 상호 운영성과 보안 문제를 해결한다.
- Applicaion Layer 프로토콜의 TCP 또는 UDP 포트를 사용으로 인한 방화벽 제약을 SOAP의 HTTP 프로토콜 사용으로 해결한다.
- 특정 HTTP Header를 방화벽으로 필터링 부분에 보냄으로써 메시지의 통과 여부를 가릴 수 있게 하는 방법으로 보안 문제를 해결한다.

| 특징            | 설명                                                         |
| --------------- | ------------------------------------------------------------ |
| 표준 공개성     | W3C의 표준 메시지 포맷으로 다중 환경에서 상호 운영 가능      |
| 유연성          | XML기반의 확장성으로 표준을 유연하게 통합/운영 가능          |
| 확장성          | HTTP 이용으로 인터넷에서 사용 가능하며 프록시와 방화벽 제약 극복 |
| 분산 컴퓨팅     | 분산된 환경에서 원격 프로시저 호출, 데이터 전송 가능         |
| 독립성          | 특정 언어, OS, 플랫폼, 전송프로토콜에 독립적                 |
| 저용량 미들웨어 | 텍스트 처리 프로세스와 메모리 웹서버만으로 미들웨어 구성     |



##### SOAP을 이용한 웹서비스의 구성 요소

| 구성요소                                                     | 설명                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| SOAP(simple obejct access protocol)                          | xml과 http 통신을 기반으로 해 네트워크 상에 존재하는 각종 컴포넌트 간 호출을 효율적으로 실현하기 위한 방법을 제시하는 규약 |
| <u>UDDI</u>(universal description, discovery and integration) | 웹 서비스의 정보를 저장과 검색을 위한 레지스트리 명세        |
| <u>WSDL</u>(web services description language)               | 웹 서비스를 기술하기 위한 xml 기반의 언어                    |



##### AJAX(Asychronous JavaScript And XML)

- 비동기식 자바스크립트 XML의 약자로 html만으로 표현하기 어려운 다양한 작업을 웹페이지에 구현해 사용자가 웹페이지와 자유롭게 상호작용할 수 있도록 하는 기술
- 별도 프로그램을 설치하거나 웹페이지를 다시 로딩하지 않고도 메뉴 등 화면의 객체를 자유롭게 움직이고 다룰 수 있다.
- 비슷한 기능을 하는 액티브X나 플래시 등에 비해 가볍고, 속도가 빠르다.
- 예전 방식은 페이지 전체 새로고침을 했다면, <u>ajax는 페이지 일부만 갱신한다.</u>
- 기존 웹은 HttpRequest를 요청객체로 잡았지만, ajax는 <u>XMLHttpRequest</u>를 요청객체로 잡는다.
- 수신 데이터는 <u>XML(최근엔 json)</u>을 받는다.
- 또한 ajax는 플러그인이나 activeX 없이 브라우저의 기능만으로 페이지 새로 고침 없이 일부분만 업데이트를 시키기 때문에 사용자에게 즉각적인 반응을 제공할 수 있다.



##### REST(Representational State Transfer)

- REST는 기존 SOA 기반의 아키텍처의 비효율성을 극복하고, UDDI 같은 중간 매체 없이, <u>고유한 URL로 직접 전송하기 때문에 빠르다.</u>
- <u>HTTP에서 제공하는 기본 메소드인 PUT, GET, POST, DELETE, PATCH 만으로 자원에 접근할 수 있다.</u>



##### REST의 주요 구성

| 구분                  | 요소            | 설명                                           |
| --------------------- | --------------- | ---------------------------------------------- |
|                       | GET             | 모든/특정 리소스를 조회(index/retrive)         |
|                       | POST            | 리소스를 생성(create)                          |
| 주요메소드(CRUD 역할) | PUT             | 리소스의 전체를 교체(replace)                  |
|                       | PATCH           | 리소스의 일부를 수정(modify)                   |
|                       | DELETE          | 특정/모든 리소스를 삭제 (delete)               |
|                       | Resource        | 자원(HTTP URI)                                 |
| 구성요소              | Verb            | 자원에 대한 행위(HTTP Method)                  |
|                       | Representations | 자원에 대한 행위의 내용(HTTP Message Pay Load) |

