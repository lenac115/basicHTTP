URI와 엡 브라우저 요청 흐름

URI(Uniform Resource Indentifier), URL(Uniform Resource Locator), URN(Uniform Resource Name)
URI 안에 URL, URN이 포함된다. URL은 위치정보, URN은 이름이다.
URL ↓
foo://example.com:8042/over/there?name=ferret#nose
URN ↓
urn:example:animal:ferret:nose

URI의 단어 뜻
1. Uniform 리소스를 식별하는 통일된 방식
2. Resource 자원, URI로 식별할 수 있는 모든 것(제한 X)
3. Identifier 다른 항목과 구분하는데 필요한 정보

URN, URL 단어 뜻
1. URL - Locator : 리소스가 있는 위치 지정
2. URN - Name : 리소스에 이름을 부여
3. 위치는 변할 수 있지만, 이름은 변하지 않는다.
4. urn:isbn:8960777331 (어떤 책의 isbn URN)
5. URN 이름만으로 실제 리소스를 찾을 수 있는 방법이 보편화 되지 않음
6. 앞으로 URI를 URL과 같은 의미로 이야기하겠음

URL
전체문법
1. scheme://[userinfo@]host[:port][/path][?query][#fragment]
2. https://www.google.com:443/search?q=hello&hl=ko

3. 프로토콜(https)
4. 호스트명(www.google.com)
5. 포트 번호(443)
6. 패스(/search)
7. 쿼리 파라미터(q=hello%hl=ko)

scheme
1. scheme://[userinfo@]host[:port][/path][?query][#fragment]
2. https://www.google.com:443/search?q=hello&hl=ko

3. 주로 프로토콜 사용
4. 프로토콜 : 어떤 방식으로 자원에 접근할 것인가 하는 약속 규칙 ex) http, https, ftp
5. http는 80 포트, https는 443 포트를 주로 사용, 포트는 생략 가능
6. https는 http에 보안 추가(HTTP Secure)

userinfo
1. URL에 사용자 정보를 포함해서 인증할 때 사용
2. 거의 사용 X

host
1. 호스트명
2. 도메인 명이나 IP 주소를 직접 사용 가능

PORT
1. 접속 포트
2. 일반적으로 생략, 생략시 http는 80, https는 443

path
1. 리소스 경로(path), 계층적 구조
2. ex) /home/file1.jpg , /members , /members/100 ,  /items/iphone12

query
1. key = value 형태
2. ?로 시작, &로 추가 가능 ?keyA=valueA&keyB=valueB
3. query parameter, query string 등으로 불림, 웹 서버에 제공하는 파라미터, 문자 형태

fragment
1. html 내부 북마크 등에 사용
2. 서버에 전송하는 정보가 아님