# REST API란 무엇인가

## REST API : REST 아키텍쳐 스타일을 따르는 API
### REST : 웹을 위한 아키텍쳐 스타일
### REST를 구성하는 스타일
- client-server
- stateless
- cache
- *uniform interface*
- layered system
- code-on-demand (optional) -> 서버에서 코드를 클라이언트에 보내 실행할 수 있어야한다 (Javascript)
-------------------
### Uniform Interface의 제약조건
- identification of resource  -> 리소스가 uri로 식별되면 된다.
- manipulation of resource through representations -> representation 전송을 통해 리소스를 조작해야한다.
- *self-descriptive message*   
- *hypemedia as the engine of application state (HATEOAS)*
----------------
### Self-descriptive message
- 메시지만 보고 해석할 수 있어야 한다.

GET/HTTP/1.1 
- 이 HTTP 요청 메시지는 뭔가 빠져 있어서 self-descriptive 하지 못하다.

GET/HTTP/1.1
Host: www.example.org
- 목적지를 추가하면 이제 self-descriptive 하다

### HATEOAS
- 애플리케이션의 상태는 Hyperlink를 이용해 전이되어야 한다.
---------------------
## Uniform interfacae 가 왜 필요한가?
### 독립적 진화
- 서버와 클라이언트가 각각 독립적으로 진화한다.
- *서버의 기능이 변경되어도 클라이언트를 업데이트 할 필요가 없다.*
- REST를 만들게 된 계기 : "How do I improve HTTP without breaking the Web."

### REST가 잘 지켜지고 있는 사례 : 웹
- 웹페이지를 변경했다고 웹 브라우저를 업데이트할 필요는 없다.
- 웹 브라우저를 업데이트 했다고 웹페이지를 변경할 필요도 없다.
- HTTP 명세가 변경되어도 웹은 잘 동작한다.
- HTML 명세가 변경되어도 웹은 잘 동작한다.

참고영상 : youtube - 'Day1, 2-2 그런 REST API로 괜찮은가'
