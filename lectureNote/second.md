인터넷 프로토콜
1. 장거리 통신시 일종의 주소를 정해 규약으로 정하여 통신하게 되는데, 이것이 인터넷 프로토콜
2. 인터넷 프로토콜의 역할은, 지정한 IP 주소(IP Address)에 데이터를 전달하고 전달물은 패킷이라는 통신 단위로 전달된다.

IP 패킷의 정보로는 출발지 IP, 목적지 IP 그리고 데이터 정보, 기타로 이루어져있다.
패킷의 구성 정보로 인터넷 통신을 하게 되는데, 여러 노드를 거치면서 목적지 IP를 향해 전송되게 된다.
목적지 IP와 출발지 IP를 함께 갖고 있기 때문에, 상호 통신에 문제는 없다.

IP 프로토콜의 한계
1. 비연결성 : 패킷을 받을 대상이 없거나 서비스 불능 상태여도 패킷 전송
2. 비신뢰성 : 중간에 패킷이 사라지면?, 패킷이 순서대로 안오면? / 패킷 소실이 일어나도 알 수 없고, 인터넷 상태에 따라 패킷의 순서가 뒤죽박죽이 되는 경우도 많음
3. 프로그램 구분 : 같은 IP를 사용하는 서버에서 통신하는 애플리케이션이 둘 이상이면?