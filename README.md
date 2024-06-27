# C#을 이용한 TCP통신
> C#을 이용해서 서버와 클라이언트 통신

## TCP 통신이란?
> TCP란 Transmission Control Protocol의 약자로 전송 제어 프로토콜을 말한다.
> OSI Layer의 4번째 Layer인 Transport Layer에서 사용하는 규약이며, 보통 하위 계층의 IP와 함께 TCP/IP로 표현한다.
> 말 그대로 전송 제어를 위한 작업을 해주는 역할이며 근거리 통신망, 인트라넷, 인터넷에 연결된 컴퓨터에서 실행되는 프로그램간 옥텟(8비트)를 안정적으로, 순서대로 교환 가능 하도록 한다.
> 웹 브라우저가 WWW에서 서버 연결 시, 이메일 전송 시, 파일 전송 시 사용한다.
> TCP는 DataStream으로부터 데이터를 받아 청크단위로 분할하고 여기에 TCP Header를 붙여 TCP Segment를 생성한다. 이 TCP Segment가 IP Datagram에 Packet화 되어 상대방과 이를 주고 받는다.
>
> ![image](https://github.com/hjyoon99/Csharp_TCP/assets/108658882/9ddf0907-2c6a-49e7-924e-e4b81e885098)
> (출처: 위키피디아)
> 
> server와 client 간 연결은 3-way Handshake를 바탕으로 이루어진다.
> SYN: 클라이언트가 서버에게 SYN ("나 너랑 통신하고 싶어.")
> SYN-ACK: 서버가 클라이언트에게 SYN-ACK ("그래? 나랑 진짜로 할거야?")
> ACK: 클라이언트가 서버에게 ACK ("응! 통신하자!")

### 실행방법
1. TCP_client 실행
2. TCP_server 실행

![image](https://github.com/hjyoon99/Csharp_TCP/assets/108658882/a460179a-7ae4-4e2b-b8a1-76123837cd85)

해당 통신은 로컬ip인 127.0.0.1에서 통신이 이루어집니다.
