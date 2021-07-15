## 1. HTTP 프로토콜
- Hyper Text를 전송하기 위한 프로토콜
- Hyper Text란, 웹 문서를 구성하고 있는 언어, HTML을 의미한다.

--------------
## 2. HTTP 통신 - Request & Response
- Request(요청) 과 Response(응답)으로 이루어져 있다.
- 클라이언트가 서버에 요청을 보내면 서버는 요청에 대한 응답 결과를 보내준다.
- HTTP Request Message
  - 요청라인 : Method/URL/버전
  - General Header ㄱ
  - Request Header ㅡ > 메시지 정보
  - Entity Header  ┘
  - CRLF : 공백
  - BODY : 본문

- HTTP Response Message
  - 상태라인 : HTTP / 버전 / 응답코드
  - General Header ㄱ
  - Response Header ㅡ>  메시지 정보
  - Entity Header ㅡ┘
  - CRLF : 공백
  - Body : 본문
 ---------------------
 ## 3. HTTP통신 - Stateless
 - HTTP 통신은 state 개념이 존재하지 않는다.
 - 통신을 주고 받아도 클라이언트와 서버는 연결되어 있는 것이 아니라 각각의 통신은 독립적이다.
 - 서로 요청한 것들을 기억하지 못한다 -> 상태를 저장하지 않는다.
 ------------------------
 ## 4. HTTP 패킷
 - HTTP 통신은 요청을 보내고 응답을 받을 때 해당 정보들을 패킷에 넣어 보낸다.
 - 패킷 구조 : Header / Body
 - Header : 보내는 사람의 주소, 받는 사람의 주소, 패킷 생명시간
 - Body : 실제 전달하고자 하는 내용
 - 
