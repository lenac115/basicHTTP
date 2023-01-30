웹 브라우저 요청 흐름
1. DNS 조회, https port 생략
2. http 요청 메시지 생성(GET /search?q=hello&hl=ko HTTP/1.1 HOST: www.google.com)

HTTP 메시지 전송
1. 웹 브라우저가 HTTP 메시지 생성
2. SOCKET 라이브러리를 통해 전달
    - A: TCP/IP 연결(IP, PORT)
    - B: 데이터 전달
3. TCP/IP 패킷 생성, HTTP 메시지 포함
4. 요청 패킷이 서버에 도착하면 HTTP 메시지를 감싼 정보를 모두 버리고 HTTP 메시지를 해석한 후 HTTP 응답 메시지를 보냄
5. 클라이언트가 응답 패킷을 받고 웹 브라우저는 패킷을 해석