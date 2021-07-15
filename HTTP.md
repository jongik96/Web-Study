## 1. HTTP 프로토콜
- Hyper Text를 전송하기 위한 프로토콜
- Hyper Text란, 웹 문서를 구성하고 있는 언어, HTML을 의미한다.

--------------
## 2. HTTP 통신 - Request & Response
- Request(요청) 과 Response(응답)으로 이루어져 있다.
- 클라이언트가 서버에 요청을 보내면 서버는 요청에 대한 응답 결과를 보내준다.
![requestresponse](https://user-images.githubusercontent.com/68894097/125783157-5b390e94-131e-487d-a951-cd5ff5a162e4.png)

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
 - 요청과 응답에 담겨있는 정보
   - General : 요청 url 정보와 메소드, 상태 코드를 확인 가능
   - Response Header : 응답 온 패킷의 헤더를 확인 가능. 서버의 종류, 연결 상태 등이 담겨 있다.
   - Request Header : 요청을 보낸 패킷의 헤더를 확인 가능. 보낸 클라이언트의 종류, 요청한 파일의 종류 등을 볼 수 있음.
----------------------------------
## 5. HTTP Request 구조
1) Start Line (요청 내용)
   - Http 메소드
     - Request target : 요청의 의도를 담고 있다. (GET, POST, DELETE, UPDATE)
     - Http ver : 버전에 따라 요청 메시지 구조나 데이터가 다를 수 있어서, version을 명시
2) Header: HTTP 요청이 전송되는 목표 주소
3) Body
--------------------------
## 6. HTTP Request 구조 : HTTP 메소드
1. GET : GET[request-uri]?query_string
  - GET 요청방식은 URI가 가진 정보를 검색하기 위해 서버 측에 요청하는 형태이다.
2. POST : POST 요청방식은 요청 URI에 폼 입력을 처리하기 위해 구성한 서버 측 스크립트 혹은 CGI 프로그램으로 구성되고 Form Action과 함께 전송되는데
  , 이때 헤더 정보에 포함되지 않고 데이터 부분에 요청 정보가 들어가게 된다.
3. PUT : POST와 유사한 전송 구조를 가지기 때문에 헤더 이외의 데이터가 함께 전송된다.
4. DELETE : 웹 서버의 파일을 삭제하기 위해 사용되며 PUT 과 반대 개념의 메소드
    
