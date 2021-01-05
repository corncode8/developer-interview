# Developer Interview
개발자 인터뷰 질문에 관련된 팁과 최소 개념입니다. 모든 내용을 자세하게 담기엔 가성비가 떨어지므로 자세한 내용을 더 학습하고 싶다면 주제를 검색하여 추가적인 학습을 하는 것을 추천합니다. 기본적인 CS 지식 정리와 실제 인터뷰 경험을 참고하여 만들었습니다. 기본 CS 지식은 동일하나 면접 본 직무가 `백앤드, 빅데이터 플랫폼, 클라우드` 관련 직무이므로 이를 감안하시길 바랍니다. 문제만 적혀 있고 정답을 적지 않은 부분은 **PR** 해주셔도 좋습니다.

## 추천 자료
##### Easy
- https://github.com/tvandame/back-end-developer-interview-questions/blob/master/Translations/Korean/README_KR.md
- https://github.com/gyoogle/tech-interview-for-developer
- https://github.com/WooVictory/Ready-For-Tech-Interview
- https://github.com/qkraudghgh/coding-interview
- https://github.com/JaeYeopHan/Interview_Question_for_Beginner
- https://github.com/KNU-CS-Study/Tech-Interview
- https://github.com/WeareSoft/tech-interview
- https://github.com/huisam/interview

##### Medium
- [코딩 인터뷰 완전 분석](https://www.aladin.co.kr/shop/wproduct.aspx?ItemId=115116545)
- [프로그래밍 면접 이렇게 준비한다](https://www.aladin.co.kr/shop/wproduct.aspx?ISBN=K172635329&start=pnaver_02)

##### Hard
- https://github.com/jwasham/coding-interview-university
- https://github.com/donnemartin/system-design-primer


## Table of Content
- [Basics](#basics)
- [OS](#os)
- [Network](#network)
- [Database](#database)
- [Datastructure](#datastructure)
- [Algorithm](#algorithm)
- [OOP](#oop)
- [Etc](#etc)
- [PL:Python](#python)
- [PL:Java](#java)
- [Design](#design)
- [Live Coding](#Live-Coding)


### Basics
* 자기소개
  * 이력 중심으로 간단하게 설명하되 신입이라면 성장 욕구를 간단히 어필하는 문구를 넣어도 좋음
* 가장 성공적이었던 프로젝트가 무엇이고 왜 성공적이라고 생각하는지
  * 현재 지원한 공고에 맞는 프로젝트를 성공적인 프로젝트로 지정하여 말하는 것이 유리
* 프로젝트 진행 시 불화에 대해서 어떻게 대처했는지
  * 솔직하게 말하되 같이 일할 수 있는 사람이라는 인식을 심어주는 것이 중요
* 프로젝트에서 본인이 기여한 부분은 어느 정도라고 생각하는지
  * 1/N보단 높되 적당한 수준으로 말하는 것이 좋음
* `우리 회사 서비스 중에 사용해본 것`
  * 지원한 공고에 맞는 회사 기술 블로그를 분석하고 그와 연관된 서비스를 말하는 것이 유리 
* 지금까지 했던 프로젝트 중 하면서 어려웠던 부분과 극복한 방법
  * 프로젝트는 지원한 회사의 직무에 연관되어 있으면 더 좋음
  * 극복한 방법은 다양한 방법이 존재하지만 `같이 일할 수 있는 정도의 사람`이라는 이미지를 심어 줄 수 있는 내용으로 답변
* 최근 관심 있게 보고 있는 기술
  * 지원한 회사의 직무에 연관되어 있으면 유리
* 이전 직장에서 아쉬웠던 부분과 왜 이직하려는지
  * 이직하고자 하는 회사만의 분명한 장점을 생각해놓고 답변하는 것이 좋음
* 우리 회사에 궁금한 점
  * 인터넷에서 검색할 수 있는 정보는 지양하고 회사 내부 또는 팀 내부나 지원한 포지션에 관련된 것이 좋음
* 본인의 장점과 단점
  * 장점은 솔직하게 말하는 것이 좋고 단점은 무조건적인 단점이 아닌 장점으로 볼 수도 있고 단점으로 볼 수도 있는 것이 좋음
* 5년 후의 나의 모습은 어떠한가
  * 기술에 대해서 진취적인 인상을 심어주는 답변이 좋음
* (사전 코딩 테스트가 있었다면) `코딩 테스트 코드`에 대한 질문
  * 부족한 구현이나 최적화 할 수 있는 부분이 있다면 생각해보거나 검색하고 가는 것이 좋음


### OS
* 운영체제
  * 하드웨어를 관리하고, `응용 프로그램과 하드웨어 사이에서 인터페이스 역할`을 하는 시스템 소프트웨어
* Process Control Block(PCB)
  * 프로세스들의 관리를 위해 정보를 저장한 커널의 자료구조
  * Process 상태, PC(다음에 수행할 명령어의 주소), CPU 레지스터, CPU 스케줄링 정보 등을 저장
* 프로세스 생성 과정
  * 프로세스 관리 정보를 갖는 `Process Control Block를 생성`하고 프로그램의 코드를 읽어 들여 `코드 영역`을 메모리에 할당
  * 초기화된 전역 변수 및 static 변수인 `데이터 영역`을 메모리에 할당
  * `힙과 스택의 초기 메모리 주소를 초기화`
  * `Queue에서 프로세스가 등록`되고 운영체제가 CPU를 할당하기를 대기
* 프로세스와 스레드의 차이
  * 프로세스: `프로그램의 실행 상태`, 운영체제로부터 자원을 할당받아 실행, `코드/데이터/스택/힙` 메모리 영역
  * 스레드: `프로세스의 독립적인 실행 단위`, `경량 프로세스`, 프로세스 안에서 프로세스로부터 자원을 받아 실행, 프로세스의 코드/데이터/힙 메모리 영역을 공유하고 `개별적인 스택`을 가짐
* 멀티 프로세싱
  * 멀티 코어 환경에서 병렬 처리를 하기 위한 방식으로 프로세스를 기반으로함
  * 멀티 코어 환경은 공유 자원(Cirical Section)이 있을 시 동기화 매커니즘이 필요
  * Pipe나 Shared Memory가 있어야 데이터를 주고 받을 수 있음 
  * 멀티 프로세스는 멀티 스레드보다 `많은 메모리 공간`을 차지하고 `IPC라는 별도 매커니즘`을 사용해야하여 `프로세스 간의 통신 비용`이 크며 문맥 교환 시에도 비용이 큼
  * 하나의 프로세스가 죽더라도 다른 프로세스에는 영향을 끼치지 않고 정상적으로 수행
* 멀티 스레딩
  * 멀티 코어 환경은 공유 자원(Cirical Section)이 있을 시 동기화 매커니즘이 필요
  * 스레드 간은 `Heap을 공유`하므로 Shared Memory가 없어도 Heap을 통해 데이터를 주고 받을 수 있음
  * 멀티 스레드는 멀티 프로세스보다 적은 메모리 공간을 차지하고 스레드 간의 통신 비용이 적으며 `문맥 교환 시에 비용이 적음`
  * 하나의 스레드의 비정상적인 활동은 전체 스레드에 영향을 끼칠 수 있음
* IPC(Inter Process Communication)
  * 프로세스 간의 통신을 하는 것으로 Pipe, 공유 메모리, 소켓 등을 통해서 구현
* Thread Safe와 Thread 
  * 멀티 스레딩 프로그램에서 일반적인 변수나 객체에 여러 스레드가 동시에 접근해도 프로그램 실행의 문제가 없는 상태
* 병렬성과 동시성의 차이
  * 병렬성: `멀티 코어`에서의 멀티 스레드, 각 코어들의 스레드가 동시에 실행
  * 동시성: `싱글 코어`에서의 멀티 스레드, 여러 개의 스레드가 번갈아가며 실행
* Critical Section(공유 자원, 임계 영역): 접근 순서에 따라 실행 결과가 달라지는 구역
* Race Condition
  * 공유 자원에 대한 여러 프로세스/스레드가 접근할 경우 `병렬 처리 상황에서 실행할 때마다 결과값이 다른 현상`
* 뮤텍스와 세마포어의 차이
  * 뮤텍스는 `스레드 기반으`로 공유 자원의 활용을 제어하는 매커니즘, 바이너리 세마포어와 비슷한 방식으로 `동기화 대상이 1개`일 때 사용 
  * 세마포어는 `프로세스 기반`으로 공유 자원의 활용을 제어하는 매커니즘, `동기화 대상이 여러 개`일 때 사용, `Deadlock`이 발생할 수 있음
    * wait(): 세마포어 변수 1감소 -> Critical Section -> signal(): 세마포어 변수 1증가
* Deadlock(교착상태)과 Deadlock 해결 방법
  * 데드락이란 멀티 프로세스/스레딩 환경에서 잘못된 동기화 매커니즘 활용 때문에 프로세스/스레드가 `block`되어 `모든 프로세스/스레드의 작업이 끝나기만을 기다리는 현상`
  * 상호 배제, 비선점, 점유와 대기, 원형 대기의 4가지 조건이 만족하면 발생
  * 모든 프로세스가 `lock을 잡는 순서를 동일`하게 코딩하는 방법 or `trylock`을 활용하여 lock을 선점한 프로세스/스레드가 없을 때만 락을 얻으려고 시도하는 방법을 통해 데드락 해결이 가능
* Pthread: POSIX Thread의 약자, 유닉스계열 POSIX시스템에서 병렬적으로 작동하는 소프트웨어를 작성하기 위하여 제공하는 API
  * POSIX: 유닉스 OS를 대상으로한 API
* 인터럽트
  * 프로그램을 실행하는 도중에 예기치 않은 상황이 발생할 경우 `현재 실행 중인 작업을 즉시 중단하고, 발생된 상황을 우선 처리한 후 실행 중이던 작업으로 복귀하여 계속 처리하는 것`
  * 문맥 교환을 구현할 때 Timer Interrupt를 통해서 제어권을 커널이 가져올 수 있도록 활용
* 문맥 교환
  * 하나의 프로세스가 CPU를 사용 중인 상태에서 다른 프로세스가 CPU를 사용하도록 하기 위해, `이전의 프로세스의 상태(문맥)를 보관하고 새로운 프로세스의 상태를 적재하는 작업`
* CPU 스케줄링 기법
  * SRT(Shortest Remaining Time): 남은 시간이 가장 적은 프로세스를 실행
  * Round Robin: 시간 조각(Time Slice)라고 하는 단위로 공평하게 프로세스 실행
  * MLFQ(Multi Level Feedback Queue): 우선 순위 개수만큼 Queue가 있으며 최상위 단계의 Queue부터 실행 후 해당 큐의 할당량이 끝나면 하위 우선 순위 Queue를 실행하는 스케줄링 기법으로 처음 시작은 모든 프로세스가 가장 높은 우선 순위 Queue에 존재하나 할당된 Time Slice를 소진하면 우선 순위를 감소시켜서 우선 순위를 정해가고 일정 주기마다 모든 작업을 가장 높은 우선 순위 큐로 이동 시켜서 Starvation을 방지
* 메모리 영역에서 힙과 스택의 차이
  * 힙은 프로그램 코드에서 `동적으로 할당하여 사용될 때 할당되는 메모리 영역`
  * 스택은 `함수를 호출할 때나 지역변수를 지정할 때 자동으로 할당되는 메모리 영역`
* 스택 영역의 장점과 단점
  * 장점: 자동으로 처리되기 때문에 `낭비되는 공간이 없고` 사용하기가 편리
  * 단점: 한계가 있어 한계를 초과하도록 삽입할 수 없고 `유연성이 부족`
* 힙 영역의 장점과 단점
  * 장점: 프로그램에 필요한 개체의 개수나 크기를 미리 알 수 없는 경우 사용하고 개체가 너무 커서 스택 할당자에 맞지 않는 경우 사용 가능
  * 단점: `할당/해제 작업`으로 인한 속도 저하
* 가상메모리와 가상메모리 사용 시의 장점
  * `프로그램에 실제 메모리 주소가 아닌 가상의 메모리 주소를 주는 방식`으로 프로그램 별로 사용 중인 메모리보다 큰 메모리를 사용하는 듯한 환상을 주는 기법
  * 실제 프로그램 전체를 적재하여 사용하지 않고 일부분만 적재하기 때문에 메모리 제약을 극복
  * 메모리의 실제 주소를 사용하지 않으므로 보안 상의 장점이 존재
* 세그멘테이션
  * 메모리 영역인 커널 영역, 스택 영역, 공유 라이브러리 영역, 힙 영역, 데이터 영역, 코드 영역 등으로 메모리를 세그먼트로 나누고 `세그먼트 테이블`에 각 세그먼트의 시작 주소와 길이 정보를 운용하여 가상 메모리를 관리하는 기법
* 페이징
  * 페이지: `가상메모리`를 최소 단위로 쪼개어 만든 일정한 크기의 블럭
  * 프레임: `물리메모리`에 페이지 크기와 같은 블럭으로 나눈 블럭
  * 프로세스를 일정 크기인 페이지로 잘라서 가상 메모리에 적재하고 페이지 테이블을 이용하여 프레임으로 변환하여 가상 메모리를 관리하는 기법
* 페이지 교체 알고리즘
  * FIFO: 페이지 교체 시점에 들어온 페이지 순서대로 페이지를 교체하는 알고리즘으로 페이지 프레임의 개수를 늘리면 Page Fault 발생이 감소해야하나, 오히려 늘어나는 `Belady의 모순` 발생
  * LRU(Least-Recently-Used): 페이지 교체 시점에 가장 오랫동안 사용되지 않은 페이지를 선택하여 교체하는 알고리즘
  * LFU(Least-Frequently-Used): 페이지 교체 시점에 참조 횟수가 가장 적은 페이지를 교체하는 알고리즘
* 캐시의 지역성
  * 시간 지역성: 최근에 참조된 주소의 내용은 곧 다음에 다시 참조되는 특성
  * 공간 지역성: 대부분의 실제 프로그램이 참조된 주소와 인접한 주소의 내용이 다시 참조되는 특성
* 컴퓨터가 부팅되는 과정
  * 처음에 부팅이 되면 `BIOS`가 실행 될 수 있도록 `메모리의 0번지에는 ROM`이 올라와있고, `CPU는 0번지를 읽어` 자동으로 ROM의 BIOS가 실행
  * `BIOS는 하드디스크의 0번지 부터 한 섹터를 읽어와 거기에 있는 부트스트랩 코드를 실행`시킨다. 부트스트랩이 `부트로더`(bootcamp, grub)를 실행시키고 그 다음 커널이 로드
* 심볼릭 링크와 하드 링크의 차이
  * 

### Network
* TCP와 UDP의 차이
  * TCP는 `신뢰성을 보장하는 연결형 프로토콜`로 `흐름제어, 혼잡제어`를 제공
  * UDP는 `신뢰성을 보장하지 않는 비연결형 프로토콜`로 흐름제어, 혼잡제어를 제공하지 않음
* TCP 흐름제어와 혼잡제어
  * 흐름제어: 수신자와 송신자 세그먼트 간의 TCP Header에 `remain window data`를 통해 남은 버퍼를 알고 흐름을 파악할 수 있음 -> `Stop and Wait`이나 `Go Back N`과 같은 정책을 사용
  * 혼잡제어: 패킷 loss 시의 확인되는 `timeout이나 duplicate ACK`을 통해서 파악 할 수 있음 -> `TCP Tahoe`나 `TCP Reno`와 같은 정책을 사용
* OSI 7계층와 각 계층 역할
  * Application - Application(7), Presentation(6), Session(5) 계층으로 분리
  * Application(7): 사용자에게 `실제 애플리케이션 서비스`를 제공하는 계층 / HTTP
  * Presentation(6): 애플리케이션의 `데이터 형태와 구조를 변환`시키는 계층
  * Session(5): 애플리케이션 간의 `TCP/IP 세션을 구축하고 관리하며 종료`시키는 계층
  * Transport(4): 통신 `양단 간의 신뢰성 있는 통신`을 보장하는 계층 / TCP or UDP
  * Network(3): 목적지까지의 경로를 선택하고 `경로에 따라 패킷을 전달`해주는 계층 / IP
  * Link(2): 인접한 `피어 간의 신뢰성 있는 통신`을 보장하는 계층 / MAC
  * Physical(1): 전기적, 기계적, 기능적인 특성을 이용해서 통신 케이블로 데이터를 전송
* HTTP와 HTTPS의 차이
  * HTTP는 웹 브라우저와 웹 서버가 통신하기 위한 프로토콜이고 HTTPS는 HTTP Secure의 약자로 HTTP에 SSL/TLS 기반의 Secure Socket을 활용한 프로토콜
  * HTTP는 평문 통신이기 때문에 `도청`이 가능하고 `변조`가 가능하며 통신 상대를 특정하지 않기 때문에 `위장`이 가능
  * HTTPS는 웹 브라우저와 웹 서버가 각각 키를 갖고 있고 `그 키를 통해 암호화/복호화하여 HTTP 통신`하므로 클라이언트와 서버만이 데이터를 열람 가능
* HTTP 상태코드  
  * 2xx: 성공
  * 3xx: 리다이렉션
  * 4xx: 클라이언트 에러
  * 5xx: 서버 에러
* 공개키
  * 비공개키와 공개키 2개의 키로 쌍으로 암호화/복호화하는 기법으로 비공개키는 자신만이 소유하고 공개키는 타인에게 제공하는 방식으로 작동
* SSL/TLS 동작방식
  * 
* 쿠키와 세션이 무엇이고 차이가 뭔지
  * 쿠키는 `클라이언트 로컬`에 저장되는 키와 값이 들어있는 작은 텍스트 데이터 파일
  * 세션은 일정 시간동안 같은 브라우저로 부터 들어오는 일련의 요구를 하나의 상태로 보고 그 상태를 객체로 `서버`에 저장하는 기술
  * 쿠키는 클라이언트 로컬에 작은 파일로 저장하지만 세션은 서버에 제한 없는 파일로 저장하고 `sessionid`를 통해 데이터를 구분하여 처리하여 보안이 좋음
* 웹 서버와 웹 애플리케이션 서버의 차이점
  * 웹 서버: Http 프로토콜을 기반으로, 클라이언트의 요청을 서비스하는 기능을 담당하는 서버로 정적 컨텐츠만 처리하는 고성능 서버
  * 웹 애플리케이션 서버: 보통 웹서버 뒤에서 DB 조회 및 다양한 로직 처리 요구시 동적인 컨텐츠를 처리하는 서버
* TCP 3-way handshake가 언제 일어나고 어떤 과정인지
  * 서버와 클라이언트가 TCP `연결을 성립할 때` 사용
  * Client -> Server: `SYN 전송`
  * Server -> Client: `SYN 전송 + ACK 전송`
  * Client -> Server: `ACK 전송`
  * TCP는 양방향성 연결이기 때문에 발생하는 매커니즘으로 연결을 성립할 때는 서버가 준비가 다 된 상태인 대기 상태에서 시작하여 3-way로 가능
* TCP 4-way handshake가 언제 일어나고 어떤 과정인지
  * 서버와 클라이언트가 TCP `연결을 종료할 때` 사용
  * Client -> Server : `FIN 전송`
  * Server -> Client : `ACK 전송`
  * Server -> Client : `FIN 전송`
  * Client -> Server : `ACK 전송`
  * TCP는 양방향성 연결이기 때문에 발생하는 매커니즘으로 연결 해제할 때는 한 쪽이 준비가 되지 않은 상태이기 때문에 연결 해제 대기 상태로 만들기 위해서 4-way로 해야 가능
* 웹 브라우저에 URL을 입력했을 때의 수행 과정
  * 사용자의 PC는 `DHCP 서버`에서 사용자 `자신의 IP 주소`, `가장 가까운 라우터의 IP 주소`, `가장 가까운 DNS 서버의 IP 주소`를 받는다.
  * `ARP`를 이용하여 IP 주소를 기반으로 가장 가까운 라우터의 MAC 주소를 받는다.
  * TCP Socket을 통해 웹 서버와 `3 way hand shaking`을 하여 연결한다.
  * `HTTP Request`가 TCP Socket을 통해 보내지고, 응답으로 웹페이지의 정보가 사용자의 PC에 전달
* 기타 네트워크 프로토콜과 기본 네트워크 주소들
  * DHCP: 호스트의 IP 주소 및 TCP/IP 설정을 클라이언트에 자동으로 제공하는 프로토콜
  * DNS: IP 주소와 도메인의 매핑정보를 관리하는 프로토콜
  * ARP: IP 주소를 물리적 네트워크 주소로 대응시키기 위해 사용되는 프로토콜
  * IP 주소: 컴퓨터 마다 부여된 고유의 주소
  * MAC 주소: NIC 카드 마다 부여된 네트워크 장비 고유의 주소
* HTTP GET 방식과 POST 방식의 차이
  * `GET은 정보를 조회하기 위한 메소드`이고 `POST는 서버로 데이터를 전송하기 위해 설계된 메소드`
  * 둘다 데이터를 서버에 전달할 수 있다는 것이 공통점이지만 GET은 URL의 파라미터로 이름과 데이터가 쌍으로 명시되어 전달되고, POST는 HTTP Request Message의 Body 부분에 데이터가 담겨있음
  * GET은 `URL의 길이는 제한적이기` 때문에 많은 양의 데이터를 전송할 수 없지만 POST는 `HTTP Request Message의 Body 부분에` 데이터가 담겨있어 제한이 없음
* HTTP POST 방식과 PUT 방식의 차이
  * 일반적으로 POST는 생성, PUT은 수정이지만 PUT으로도 생성이 가능
  * POST와 가장 큰차이는 PUT 메서드는 자원의 식별자를 이미 알고있는 상태로 POST는 request message로 포함된 엔티티를 이용해 새로운 자원을 생성해 내는 것이고, PUT은 request message와 함께 넘어온 식별자의 자원을 만드는 것
* 웹 캐시
  * 대부분의 브라우저에서는 `HTTP 헤더`에 캐시 구현이 포함되어 있어서 웹 캐시를 구현
  * 응답헤더의 `Last-Modified`, Etag, Expires, Cache-Control 항목 등과 같은 여러 부분의 여러 개의 태그를 통해서 캐싱
  * Cache-Control: HTTP 헤더를 통해 캐싱 정책을 정의할 수 있다. `no-cache` vs `no-store`
  * 브라우저는 최초 응답 시 받은 Last-Modified 값을 If-Modified-Since라는 헤더에 포함 시켜 페이지를 요청 -> 서버는 요청 파일의 수정 시간을 If-Modified-Since값과 비교하여 동일하다면 304 Not Modified로 응답하고 다르다면 200 OK -> 브라우저는 응답 코드가 304인 경우 캐쉬에서 페이지를 로드하고 200이라면 새로 다운받은후 Last-Modified 값을 갱신
  * 브라우저는 최초 응답 시 받은 Etag값을 If-None-Match라는 헤더에 포함 시켜 페이지를 요청 -> 서버는 요청 파일의 Etag 값을 If-None-Match 값과 비교하여 동일하다면 304 Not Modified로 응답하고 다르다면 200 OK와 함께 새로운 Etag 값을 응답 헤더에 전송 -> 브라우저는 응답 코드가 304인 경우 캐쉬에서 페이지를 로드하고 200이라면 새로 다운받은후 Etag값을 갱신
  * 브라우저는 최초 응답 시 받은 Expires 시간을 비교하여 기간 내라면 서버를 거치지 않고 바로 캐쉬에서 페이지를 로드
* CDN과 사용 시의 이점
  * CDN은 Contents Delivery Network의 약자로 지리적, `물리적으로 떨어져 있는 사용자에게 웹 페이지 콘텐츠 로드 지연을 최소화하는, 촘촘히 분산된 서버로 이루어진 플랫폼 기술`
  * 웹 브라우저를 실행하는 디바이스인 사용자 에이전트는 HTML, 이미지, CSS, JavaScript 파일을 렌더링하는데 필요한 콘텐츠를 요청하고 요청된 서버에 의해 `콘텐츠에 대한 각 요청이 발생하면 최적으로 배치된 CDN 서버에 엔드유저가 매핑`되고, 해당 서버는 요청된 파일의 캐싱된(사전 저장된) 버전으로 응답하여 CDN 서버에게서 데이터를 전송받도록함
* 로드 밸런싱
  * 로드 밸런서를 클라이언트와 서버 사이에 두고, 부하가 일어나지 않도록 여러 서버에 분산하는 방식
  * 로드 밸런서는 물리 장비를 이중화해서 구현하거나 nginx와 같은 웹서버를 이용하여 구현
* CIDR
  * 클래스 없는 도메인 간 라우팅 기법으로 최신의 IP 주소 할당 방법으로 정적이였던 클래스 방식에 비해 IP 주소의 영역을 여러 네트워크 영역으로 나눌 수 있기 때문에 기존방식에 비해 유연
* RESTful API
  * `REST`는 `HTTP, WWW에서 웹에 존재하는 모든 자원에 고유한 URI를 부여해 활용하는 것`으로, 자원을 정의하고 자원에 대한 주소를 지정하는 방법론
  * `RESTful API`는 `REST 기반의 규칙들을 지켜서 설계된 API`
  * 기본 설계 원칙1. `/`를 계층관계를 나타내는데 사용하되 마지막 문자에 `/`를 포함하지 않음
  * 기본 설계 원칙2. 자원에 대한 정보는 명사로 표현하고 자원에 대한 `행위는 HTTP 메소드`로 표현
  * 기본 설계 원칙3. 소문자와 `-`를 사용
  * 기본 설계 원칙4. 브라우저는 form-data 형식의 submit 으로 보내고 서버에서는 json 형태로 보내는 식의 분리보다는 둘 다 form-data 형식으로 보내든 하나로 통일
* RESTful API 장단점
  * HTTP를 사용하므로 웹 인프라를 그대로 이용할 수 있고 MSA에 적합하여 재사용에서 이점이 존재
  * HTTP를 사용하므로 HTTP 통신 모델에 제약적
* url 입력부터 응답이 오는 과정
  *
* 웹 브라우저에 http 응답이 랜더링되는 과정
  *

### Database
* DB를 사용하는 이유
  * 파일 시스템이 OS마다 다를 수 있기 때문에 OS에 종속적인 파일 시스템을 이용하는 것은 프로그램의 확장성을 해침
  * DB는 `원자적 갱신`, `동시성 제어`, `데이터 보호`, `백업 및 회복` 등의 여러 데이터 관리 기능을 두어 데이터 관리를 편하게 하기 때문에 파일 시스템을 활용하여 OS를 만듦
* 테이블
  * 행과 열로 이루어진 데이터의 집합
* 도메인
  * 데이터베이스 필드에 채워질 수 있는 값들의 집합
* 행
  * 테이블을 구성하는 데이터 셋으로 튜플이나 레코드라고 불림
* 열
  * 테이블을 구성하는 데이터 셋으로 속성이라고 불림
* 후보 키, 주 키, 외래 키
  * 후보 키: 릴레이션을 구성하는 속성들 중에서 Tuple을 `유일하게 식별`할 수 있는 속성들의 부분 집합
  * 주 키: 후보 키 중에서 선택한 Main Key
  * 외래 키: 참조되는 릴레이션의 주 키와 대응되어 릴레이션 간에 참조 관계를 표현하는 키
* 스키마와 테이블(릴레이션)의 차이
  * `스키마는 테이블(릴레이션)의 이름과 속성들의 나열`로 테이블에서의 첫 행 헤더이고 `테이블은 행과 열로 구성된 전체를 의미`
* 조인
  * 두 개 이상의 테이블이나 데이터베이스를 연결하여 데이터를 검색하는 방법으로 적어도 하나의 칼럼을 서로 공유하고 있어야 하므로 이를 이용하여 데이터 검색에 활용
* Index를 사용하는 이유와 장점 및 단점
  * 인덱스는 데이터베이스의 `검색 속도`를 위해 사용하는 추가적인 자료구조로 `테이블 내의 칼럼의 값과 해당 레코드가 저장된 주소를 키와 값의 쌍으로 정의`
  * 인덱스를 사용하면 검색이 빨리지지만 테이블의 데이터가 추가, 삭제, 수정이 자주되는 경우 인덱스도 변경해야 하여 성능이 오히려 저하될 수 있음
* Index 자료구조
  * B 트리: 이진 트리를 확장해서, 더 많은 수의 자식을 가질 수 있게 일반화 시킨 자료구조
  * B+ 트리: B 트리를 확장해서, 데이터의 빠른 접근을 위한 인덱스 역할만 하는 비단말 노드(not Leaf)가 추가시킨 자료구조
  * 인덱싱에선 등호 연산 때문에 해시 테이블을 사용하면 성능이 떨어짐
* SQL Injection
  * 해커에 의해 조작된 SQL 쿼리문이 데이터베이스에 그대로 전달되어 비정상적인 명령을 실행시키는 공격 기법
  * view를 활용하여 접근하는 에러를 볼 수 없게 하고 검증 로직을 추가하여 방어해야함
* 뷰
  * 특정 사용자로부터 특정 속성을 숨기는 기능으로 뷰를 정의하여 그 뷰를 테이블처럼 사용하게 하여 특정 속성을 숨김
* 정규화
  * 테이블의 속성들이 상호 종속적인 관계를 같는 특성을 이용하여 테이블을 무손실 분해 하는 과정
* 트랜잭션
  * 데이터베이스의 상태를 변화시킬 때 한번에 수행되어야하는 하나의 `원자적인 작업의 단위`
  * Lock과 유사한 기능을 하지만 Lock은 동일한 자원을 요청할 경우 한 시점에는 하나의 커넥션만 변경하는데에 반해 트랜잭션은 논리적인 작업의 쿼리의 개수와 관계없이 논리적인 작업 셋 자체가 100% 적용되거나 아무것도 적용되지 않아야 함을 보장
* ACID
  * 데이터의 유효성을 보장하기 위한 트랜잭션의 특징
  * `Atomicity(원자성)`: `모든 작업이 반영되거나 모두 롤백되는 특성`입니다.
  * `Consistency(일관성)`: 데이터는 `미리 정의된 규칙에서만 수정이 가능한 특성`을 의미합니다.
  * `Isolation(고립성)`: A와 B 두개의 트랜젝션이 실행되고 있을 때, A의 작업들이 B에게 보여지는 정도를 의미합니다.
  * `Durability(영구성)`: 한번 반영(커밋)된 트랜젝션의 내용은 `영원히 적용`되는 특성을 의미합니다.
* Commit, Rollback
  * Commit: 작업의 논리적 단위가 성공적으로 끝났고, 데이터베이스가 다시 일관된 상태에 있으며 이 트랜잭션이 행한 갱신 연산이 완료되어 하드 디스크에 `저장된 것을 트랜잭션 관리자에게 알려주는 연산`
  * Rollback: 트랜잭션의 실행을 취소하였음을 알리는 연산자로 `트랜잭션이 수행한 결과를 원래의 상태로 원상 복귀시키는 연산`
* 관계형 데이터베이스와 NoSQL의 차이
  * 관계형 데이터베이스는 엄격한 스키마 아래 행과 열로 구성된 테이블들의 관계로 데이터를 저장하는 데이터베이스이고 NoSQL은 스키마가 없거나 느슨한 스키마로 데이터를 저장하는 데이터베이스
  * 관계형 데이터베이스는 `속성(열)에 맞는 각각형 자료형에 따라` 데이터를 삽입해야하지만 NoSQL은 `key-value 구조`이거나 `Document 구조`의 유연한 데이터 삽입 구조를 갖음
  * 관계를 맺고 있는 데이터가 자주 변경되거나 테이블 안에서 읽어올 데이터가 불분명한 경우 또는 명확한 스키마가 있는 경우 SQL DB가 좋고 정확한 데이터 구조를 알 수 없거나 테이블 안에서 읽어올 데이터가 분명한 경우 또는 변경/확장이 쉡게 되어야하는 경우 NOSQL DB가 좋음
* 커넥션 풀
  * 사용자의 요청에 따라 Connection 을 생성하다 보면 많은 수의 연결이 발생했을 때 서버에 과부하가 걸리게 되므로 이러한 상황을 방지하기 위해 `미리 일정 수의 Connection을 만들어 pool에 담아 뒀다가 사용자의 요청이 발생하면 연결을 해주고 연결 종료 시 pool에 다시 반환하여 보관하는 것`
* DB 클러스터링과 리플리케이션의 차이점
  * 클러스터링은 `DB 서버를 다중화` 하는 것이고 리플리케이션은 `서버와 데이터를 같이 다중화` 하는 것
* PostgresSQL과 ElasticSearch의 차이점
  * PostgresSQL은 관계형 데이터베이스이고 ElasticSearch는 검색 및 분석엔진으로 다르고 ES는 데이터 모델을 JSON으로 하고 있어 NoSQL처럼 사용할 수 있음
* Redis와 MongoDB
  * Redis는 No SQL 방식을 사용하는 인메모리 데이터베이스로 `Key-Value` 형식으로 데이터를 저장하며 주로 캐쉬로 사용
  * MongoDB는 NO SQL 방식을 사용하는 데이터베이스로 JSON같은 구조의 `Document` 형식으로 데이터를 저장하고 문서에 대한 ID를 키로 표현
* Redis의 데이터 휘발을 막기 위한 방법
  * `snapshot` 기능을 통해 디스크에 백업하거나 AOF 기능을 통해 `명령 쿼리를 저장`해두고 서버가 셧다운 되면 재실행


### Datastructure
* 배열과 링크드 리스트 비교
  * 배열은 순차적으로 데이터를 저장하는 자료구조로 메모리 상에 연속적으로 할당한 자료구조이고 링크드 리스트는 따로 할당하고 이은 자료구조
  * 배열은 순서를 알고 있다면 탐색에서 O(1) 삽입 삭제에서 O(N)
  * 링크드 리스트는 탐색에서 O(N) 순서를 알고 있다면 삽입 삭제에서 O(1)
* 배열 리스트와 링크드 리스트 비교
  * 배열 리스트는 내부적으로는 배열을 활용하기 때문에 탐색에서 O(1) 삽입 삭제에서 O(N)
  * 링크드 리스트는 탐색에서 O(N) 순서를 알고 있다면 삽입 삭제에서 O(1)
  * 캐시의 특성 때문에 빈번한 삽입 삭제가 나지 않는 경우라면 배열 리스트를 사용할 때 일반 적으로 성능이 더 좋음
* 해쉬테이블
  * 배열과 리스트의 장점을 합친 자료구조로 key 값을 통해 해시 주소를 알아내어 탐색에 있어 O(1)을 보장하는 자료구조
  * `해시 충돌`이 나는 경우 그 다음 비어 있는 공간에 삽입하는 방식인 선형 조사법 또는 해시 주소로 관리되는 데이터를 연결 리스트로 관리하는 방식인 체이닝 기법을 통해서 해결
* Stack과 Queue
  * Stack은 LIFO 방식으로 삽입되고 제거되는 최근성에 포커싱된 자료구조이고 Queue는 FIFO 방식으로 삽입되고 제거되는 순차성에 포커싱된 자료구조
* Tree, Binary Tree, Full Binary Tree, Complete Binary Tree, Binary Search Tree 
  * 트리는 그래프의 스페셜 케이스로 `사이클을 가지지 않는 그래프`로 부모 자식 관계를 갖는 노드들의 집합으로 계층적 구조를 갖는 자료구조
  * `이진 트리`는 최대 2개의 자식 노드들만 가질 수 있는 트리
  * `포화 이진 트리`는 각 레벨에 노드가 꽉 차있는 트리
  * `완전 이진 트리`는 높이가 K인 트리에서 레벨 1~ 레벨 K-1까지 모두 채워져 있고 마지막 레벨에서는 왼쪽부터 순서대로 채워져 있는 트리
  * `이진 탐색 트리`는 탐색을 위해 만들어진 자료구조로 `부모 노드의 키 값이 왼쪽 자식 노드의 키값보다 크고 오른쪽 자식 노드의 키값보다 작거나 같은 구조`
* 힙
  * 힙은 완전 이진 트리의 일종으로 우선 순위 큐를 구현하기 위해 만들어진 자료구조인데 이진 탐색 트리가 전체 노드를 탐색하기 위한 자료구조라면 힙은 최소값 또는 최대값을 쉽게 뽑아내기 위한 자료구조
  * `부모 노드의 키 값이 자식 노드의 키 값보다 항상 큰 완전 이진 트리`로 힙은 자식 노드에도 구분 조건이 필요한 이진 탐색 트리보다 느슨한 정렬 상태를 유지
* Binary Search Tree의 최악의 시간복잡도와 최악의 시간복잡도를 유발하는 케이스
  * 밸런싱이 된 BST는 O(logN)이지만 밸런싱이 되지 않지 않고 `한쪽으로만 삽입된 경우 O(N)`
* Graph 자료구조
  *
* Graph를 구현하는 두 가지 방법과 장점
  * 인접 행렬을 사용하는 방법: 인접 행렬의 해당하는 위치의 value 값을 통해서 vertex 간의 연결 관계를 `O(1`)으로 파악하는 방법으로 `정점과 엣지가 많을 경우 사용`
  * 인접 리스트를 사용하는 방법: 각 vertex의 adjacent list를 통해서 연결 관계를 `O(정점에 연결된 노드의 수)`로 파악하는 방법으로 `정점과 엣지가 적을 경우 사용`


### Algorithm
* 빅오 표기법
  * Big O 표기법는 컴퓨터 공학에서 알고리즘의 시간복잡도(실행시간)이나, 공간 복잡도(사용 메모리)에 대한 최악의 경우를 표현하는 표기 방법
* 정렬 알고리즘에서 `stable` 하다는 것의 의미
  * 정렬 기준으로 봤을 때 값이 `동일한 Element가 있어도 정렬 전의 순서와 정렬 후의 순서가 동일함을 보장`하는 것
* 정렬 알고리즘의 가짓수가 많은 이유
  * `공간 복잡도`에 따라 사용해야할 알고리즘이 다름 -> Merge Sort는 공간 복잡도는 Selection Sort와 Insertion Sort에 비해 큼
  * `안정 정렬`이냐 `불안정 정렬`이냐에 따라 사용해야할 때가 다름
* Selection Sort
  * 선택 정렬은 가장 작은 값을 가지는 데이터를 찾아서 가장 작은 값을 앞에서부터 채워 나가면서 정렬하는 방식으로 동작하는 O(n^2) `불안정 정렬 알고리즘`으로 1번의 순환마다 맨 앞의 값이 고정
* Bubble Sort
  * 버블 정렬이란 처음부터 끝까지 현재 자신과 자신의 다음 데이터를 비교해가면서 큰 값을 맨 뒤로 보내는 방식으로 동작하는 O(n^2) `안정 정렬 알고리즘`으로 1번의 순환마다 맨 뒤의 값이 고정
* Merge Sort
  * 병합 정렬은 배열을 반으로 쪼개 가면서 하나의 원소를 가진 배열로 만든 이후에 쪼개진 각 배열을 정렬하면서 병합하여 최종 정렬된 배열을 완성하는 O(NlonN) `안정 정렬 알고리즘`
* Heap Sort
  * 완전 이진 트리를 기본으로 하는 힙에 데이터를 삽입하고 꺼내서 힙을 통해 정렬하는 O(NlogN) `불안정 정렬 알고리즘`
* Quick Sort
  * 분할 정복 알고리즘으로 `파티셔닝` 아이디어를 재귀적으로 활용
  * `파티셔닝`이란 pivot 원소를 기준으로 왼쪽은 pivot보다 작은 원소들로 모으고 오른쪽은 pivot보다 큰 원소로 모으는 것을 의미하는데 pivot을 기준으로 파티셔닝이 완료되면 pivot을 고정하고 재귀호출 하여 구현하는 O(NlonN) `불안정 정렬 알고리즘`
  * Quick Sort가 통상적으로 가장 빠른 정렬을 지원하지만 `Worst Case에서 O(n^2)`이므로 Tim Sort나 Heap Sort를 사용하기도 함
* 이분 탐색
  * 이분 탐색은 `이미 정렬되어 있는 자료구조`에서 특정 값을 탐색할 때 탐색 범위를 반으로 쪼개서 값을 찾아가는 알고리즘
  * O(logN)으로 순차 탐색보다 빠르지만 탐색을 위해 정렬을 하면 순차 탐색보다 더 높은 시간복잡도를 갖게 됨
* Fibonacci 공식을 재귀적인 방법과 동적 계획법을 이용했을 때 각각의 차이
  * 재귀적인 방법인 경우 재귀 호출 시에 중복되는 연산이 계속 수행되지만 동적 계획법의 경우 이전 값을 `메모리제이션`하기 때문에 중복 연산이 수행되지 않음
* DFS와 BFS
  * DFS는 `스택이나 재귀호출`로 구현할 수 있는 탐색 방법으로 한 정점으로부터 연결되어 있는 한 정점으로만 나아가는 방식
  * BFS는 `큐`를 통해서 구현할 수 있는 탐색 방법으로 한 정점으로부터 연결되어 있는 모든 정점을 나아가며 탐색하는 방식으로 BFS로 구한 경로는 최단 경로라는 장점이 존재
* 재귀호출을 이용할 때의 문제점
  * 스택의 범위를 초과할 수 있음

### OOP
* 객체지향 프로그래밍과 장점
  * 프로그래밍에서 필요한 데이터를 추상화시켜 상태와 행위를 가진 객체를 만들고 그 객체들 간의 유기적인 상호작용을 통해 로직을 구성하는 프로그래밍 방식으로 `추상화`가 쉽고 상속을 통해 코드 `재산성성`을 높일 수 있으며 객체 단위 코드가 나눠져 있기 때문에 `디버깅과 유지보수`에 용이
* 객체지향 프로그래밍의 특징
  * `추상화`: 필요한 정보만을 표현함으로써 공통의 속성이나 기능을 묶어 이름을 붙이는 것
  * `캡슐화`: 속성과 기능을 정의하는 멤버 변수와 메소드를 클래스라는 캡슐에 넣는 것
  * `상속`: 부모 클래스의 속성과 기능을 그대로 이어 받아 사용할 수 있게 하고 기능의 일부분을 변경해야 할 경우, 상속 받은 자식 클래스에서 해당 기능만 다시 수정(정의)하여 사용할 수 있게 하는 것
  * `다형성`: 하나의 변수명, 함수명 등이 상황에 따라서 다른 의미로 해석될 수 있는 것
* 다형성의 구체 사례
  * 부모 타입으로 자식 객체를 참조하여 부모 타입에 대한 메소드들을 쓸 수 있음
  * 부모 타입으로 자식 타입의 객체를 참조할 때는 묵시적으로 형변환, 부모 타입의 객체를 자식 타입으로 참조하게 할때는 명시적으로 형변환할 수 있고 그 객체가 원래 자식 객체였는지 부모 객체였는지에 따라 사용 가능한 필드나 메소드가 정해짐
* 객체지향 설계의 5원칙
  * `SRP(Single Responsibility Principle)`: 단일 책임 원칙, 클래스는 단 하나의 책임을 가져야 하며 클래스를 변경하는 이유는 단 하나의 이유이어야 한다.
  * `OCP(Open-Closed Principle)`: 개방-폐쇄 원칙, 확장에는 열려 있어야 하고 변경에는 닫혀 있어야 한다.
  * `LSP(Liskov Substitution Principle)`: 리스코프 치환 원칙, 상위 타입의 객체를 하위 타입의 객체로 치환해도 상위 타입을 사용하는 프로그램은 정상적으로 동작해야 한다.
  * `ISP(Interface Segregation Principle)`: 인터페이스 분리 원칙, 인터페이스는 그 인터페이스를 사용하는 클라이언트를 기준으로 분리해야 한다.
  * `DIP(Dependency Inversion Principle)`: 의존 역전 원칙, 고수준 모듈은 저수준 모듈의 구현에 의존해서는 안된다.
* 클래스와 인스턴스의 차이
  * 클래스는 객체를 만들기 위한 템플릿, 객체는 클래스라는 템플릿을 토대로 `메모리에 할당한 실체`
* Immutable
  * 생성 후 변경 불가한 객체로 변경을 하려면 복사 이후 변경해야함
* Call by Value vs Call by Reference
  * Call by Value와 Call by Reference는 `값을 복사를 하여 처리를 하느냐, 아니면 직접 참조를 하느냐 차이`로 Call by value는 인자로 받은 값을 복사하여 처리하고 Call by reference는 인자로 받은 값의 주소를 참조하여 직접 값에 영향을 줌
* 디자인 패턴
  * 소프트웨어 코드 작성 시에 생기는 `공통적인 문제를 해결하는데 도움이 되는 코드 패턴`
* 디자인 패턴 중 싱글톤 패턴
  * 전체 프로그램에서 단 1개의 객체를 생생하고 공유하는 코드 패턴으로 한번의 객체 생성으로 재사용이 가능하기 때문에 메모리 낭비를 방지하고 객체가 전역성을 띄기 때문에 공유가 용이
* 디자인 패턴 중 MVC 패턴
  * Model, View, Controller라고 하는 컴포넌트로 분리하여 `비지니스 처리 로직`과 사용자 `인터페이스 요소`를 분리시켜 서로 영향없이 개발하기 수월
* 디자인 패턴 중 팩터리 패턴
  * 팩토리 패턴은 클래스의 `인스턴스를 만드는 것을 서브클래스에서 결정하는 패턴`으로 팩토리 메서드 패턴과 추상 팩토리 패턴으로 구체화됨
  * 팩토리 메서드 패턴: 객체를 생성하기 위한 인터페이스를 정의하는데, 어떤 클래스의 인스턴스를 만들지는 서브클래스에서 결정
  * 추상 팩토리 패턴: 인터페이스를 이용하여 서로 연관된, 또는 의존하는 객체를 구상 클래스를 지정하지 않고도 생성
* MVC 패턴을 강화시키는 방법
  * 


### Etc
* 학부 때 가장 재미있게 공부한 과목은 무엇이고 그 이유는 무엇이며 그 과목에 대해서 추가적으로 어떤 공부를 하였는가\
  * 
* 포인터
  * 메모리 상의 주소를 저장하는 공간
* 컴파일 언어와 스크립트 언어의 차이
  * `컴파일 언어`는 컴파일러를 통해 사전에 컴파일 되어 기계어 상태로 실행되고 `스크립트 언어`는 컴파일 단계 없이 인터프리터에 의해 실행 단계해서 한 줄씩 기계어로 번역하여 실행
  * 일반적으로 컴파일 언어가 스크립트 언어에 비해 빠르고 안정적임
* 동기식과 비동기식의 차이
  * 동기식은 요청에 대한 응답을 기다린 후 `응답이 오면 실행`하는 방식이고 비동기식은 요청에 대한 `응답을 기다리지 않고 실행`하는 방식
  * 동기식은 구성이 단순하나 멀티태스킹이 불가능하고 비동기식은 멀티태스킹이 가능하나 요청량이 많아질 경우 부하 컨트롤과 데이터의 일관성 유지 등 추가적인 처리가 필요
* 블락킹과 논블락킹의 차이
  * 블락킹은 I/0 처리 함수가 끝날 때까지 기다리고 처리가 끝나면 결과를 리턴하는 방식이고 논블락킹은 I/0 처리 함수가 끝나지 않더라도 기다리지 않고 다른 작업을 처리하는 방식
* 블락킹과 비동기의 차이
  * 블락킹과 비동기 모두 응답을 기다리지 않는 공통점이 있지만, 재실행 시점이 비동기는 `요청에 대한 응답`이라는 관점이고 블락킹은 `I/O처리(시스템 함수 호출의 리턴)`이라는 관점에서 다름
* TDD
  * `테스트 코드를 작성 한 후 그것을 통과하는 실행 코드를 작성`하는 cycle로 개발을 해가는 방법으로 디버깅이 쉬워지고 코드의 신뢰성이 높아짐
* 크롬 탭은 프로세스인지 스레드인지
  * 크롬은 탭마다 PID를 가지고 있는 Process이며 각 Tab마다 랜더링 정보나 기타 데이터를 따로 관리, 그로 인해 메모리를 많이 잡아먹기도 하지만 하나의 Tab에 오류가 생겼다고 모든 Tab에 영향을 끼치진 않는 장점이 존재
* 함수형 프로그래밍
  * 함수형 프로그래밍은 계산을 수학적 함수의 조합으로 생각하는 방식
  * 1급 객체와 데이터 불변성 그리고 고차함수, 합성함수, 순수함수와 같은 다양한 함수 개념으로 구성
* Git에서 merge와 rebase의 차이
  * git merge를 하면 브랜치를 브랜치의 커밋 로그는 사라지고 `병합하는 커밋 로그가 master에 head에 추가`
  * git rebase를 하면 브랜치를 base로 master를 `커밋을 재정렬하여 브랜치의 커밋 하나 하나가 master에 정리되어 추가`
* 도커와 가상 머신의 차이
  * 
* 쿠버네티스 및 가상 플랫폼이 핫해진 이유
  * 
* 클라우드로의 전환이 필수적인 이유
  * 비용이 낮음: 서버 장비를 구매하고 유지하는 비용이 장기적으로 봤을 때 클라우드 시스템을 이용하는 비용보다 비쌈
  * 효율적인 인적자원 운영: 직접 방문해야하는 On-premise에 반해 웹에서 100% 제어 및 모니터링이 가능하기 때문에 개발(혹은 설계) 인력과 공존이 가능
  * 안정성: 클라우드는 다양한 공간으로 분산하기 때문에, 분선돤 모든 곳에 동시다발적으로 문제가 생기지 않는한 장애가 발생하지 않음
  * 확장성: 트래픽이 임계점에 도달하면 빠르게 서버를 확장할 수 있음
* HDFS
  * 
* 하둡 에코 시스템
  * 
* 주키퍼의 지노드에 저장되는 데이터
  * 
* Hot Warm 아키텍처
  *
* Spark의 RDD
  *
* nginx 설정에서 성능을 높이는 방법
  * 
* 적정 샤드의 개수를 정하는 방법
  * 
* ElasticSearch에서 마스터가 하는 역할
  * 
* 카프카
  * 
* flume과 logstash의 역할
  * 
* 리눅스의 파일 권한
  * 
* 

### Python
* Generator와 사용 시의 장점
  * `Iterator를 생성해주는 루틴`으로 `yield` 키워드를 통해서 만드는데, Generator는 한번에 모든 데이터를 메모리에 적재할 필요가 없어서 메모리 효율이 높고 계산 결과가 필요할 때 수행되므로 수행 시간을 꼭 필요한 시간까지 늦츨 수 있음
* Decorator와 사용 시의 장점
  * 기존의 코드에 여러 가지 기능을 추가하는 파이썬 구문으로 데코레이터를 함수나 클래스로 정의하고 수행하고자 하는 함수에 `@` 키워드를 통해서 삽입하여 실행시켜 생산성을 극대화할 수 있음
* Python Garbage Collection 동작 방식
  * 각각의 객체마다 `reference count`를 갖고 있고 몇 곳에서 객체를 참조하는지를 나타내는데 인터프리터가 계속 이를 확인하다가 이 count가 0이 되는 경우 그 객체를 삭제
* GIL과 GIL을 보완하는 방법
  * 파이썬은 하나의 스레드만이 인터프리터의 제어권을 가질 수 있는 개념인 GIL(Global Interpreter Lock)은 멀티 코어 환경에서도 어느 시점에서나 1개의 스레드만 실행될 수 있기 때문에 `threading`이 아닌 `multiprocessing` 모듈을 통해 스레드 단위가 아닌 프로세스 별로 인터프리터 락을 잡아 보완해야함
* Duck Typing
  * 동적 타입을 가지는 프로그래밍 언어에서 많이 사용되는 개념으로, 객체의 실제 타입보다는 객체의 변수와 메소드가 그 객체의 적합성을 결정하는 것을 의미


### Java
* JVM과 Java 프로그램 실행 과정
  * JVM은 Java Virtual Machine의 약자로 자바 프로그램을 실행하는 역할을 하고 프로그램이 시작되면 컴파일러를 통해 바이트 코드로 변환하고 변환된 파일을 JVM에 로딩하여 실행
  ![jvm](https://user-images.githubusercontent.com/38900338/103631397-46626e80-4f86-11eb-8d28-3ef22c4ecc52.JPG)
* Java에서 Garbage Collection이 필요한 이유에 대해서 설명
  * 자바는 메모리를 명시적으로 해제하지 않기 때문에 GC를 통해서 필요없는 객체를 지우는 작업을 수행
* JVM 메모리 구조
  * 크게 `메소드 영역, JVM 스택, JVM 힙`으로 나뉘며 JVM 힙은 `Young Generation, Old Generation, Permanent Generation`으로 나뉘고 Young Generation은 `Eden, Survivor0, Survivor1`으로 나뉨
* Java Garbage Collection 동작 방식
  * 새롭게 생성된 객체는 `Young의 Eden 영역`으로 들어가게 되고 `Eden 영역이 다 차면 Minor GC`가 발생하여 참조 횟수에 따라 증가하는 `age bit`를 보고 불필요한 객체를 삭제하고 생존한 객체는 S0으로 이동
  * Minor GC가 발생할 때마다 각각 Young 영역의 객체들은 삭제와 이동을 하게되는데 (Eden -> S0 / S0 -> S1)
  * S1이 가득 차면 필요한 객체는 `OLD 영역`으로 이동하고 `OLD 영역이 가득차면 Major GC`를 통해서 값을 삭제
  * GC가 실행될 때마다 `STOP THE WORLD`가 발생하여 프로그램이 중지
* Overriding과 Overloading
  * `오버라이딩은 부모 클래스에 존재하는 메서드를 하위 클래스에서 재정의하는 것`이고 `오버로딩은 같은 메서드 이름을 갖게 하지만 시그니처가 다르게 정의하는 것`
* 추상 클래스와 인터페이스
  * 추상 클래스는 반드시 구현(오버라이딩)해야하는 추상 메소드를 1개 이상 갖고 있는 클래스로 추상 메소드에도 abstract 키워드를 붙여주고 추상 클래스에도 abstract 키워드를 붙여서 표기
  * 인터페이스는 추상 메소드만 갖고 있는 개념으로 class 대신 interface 키워드를 붙이고 메소드에도 abstract 키워드를 붙이지 않고 표기
  * 두 가지 개념 모두 독립 생성이 불가능하고 상속을 목적으로 사용하는데 추상 클래스는 1번만 상속받을 수 있지만 인터페이스는 여러번 상속 가능
  * 인터페이스는 추상 클래스와 달리 구현을 강제함으로써 구현 객체의 같은 동작을 보장하여 인터페이스를 이용하여 `표준화를 확립할 수 있으므로 서로 관계가 없는 객체들이 상호 작용을 가능하게 함`
* Collection
  * List: 대표적인 구현체로는 `ArrayList`가 존재한다. 이는 기존에 있었던 `Vector`를 개선한 것이다.
  * Map: 대표적인 구현체로 `HashMap`이 존재한다. 해시테이블처럼 `key-value`의 구조로 이루어져 있으며 key를 기준으로 중복된 값을 저장하지 않으며 순서를 보장하지 않는다. 
  * Set: 대표적인 구현체로 `HashSet`이 존재한다. `value에 대해서 중복된 값을 저장하지 않는다.`
  * Stack과 Queue: Stack은 직접 new 키워드로 사용할 수 있으며, Queue는 LinkedList에 new 키워드를 적용하여 사용
* Annotation
  * 어노테이션이란 본래 주석이란 뜻이지만, 자바에서는 인터페이스를 기반으로 한 문법으로 주석과 다른 점은 주석처럼 `코드에 달아 클래스에 특별한 의미를 부여하거나 기능을 주입함`
* Generic
  * 제네릭은 다양한 타입의 객체들을 다루는 메서드나 컬렉션 클래스에서 사용하는 것으로, `컴파일 과정에서 타입체크를 해주는 기능`
* Access Modifier
  * public: 어떤 클래스든 접근할 수 있다는 것을 의미
  * protected: 자기 자신, 같은 패키지, 서로 다른 패키지다 하더라도 상속받은 자식 클래스에서만 접근할수 있다는 것을 의미
  * private(default): 자기 자신의 스코프에서만 접근할 수 있다는 것을 의미
* final 키워드
  * final 키워드는 상수로 정의하는 키워드
  * final class: 다른 클래스에서 상속하지 못한다.
  * final method: 다른 메소드에서 오버라이딩하지 못한다.
  * final variable: 변하지 않는 상수값이 되어 새로 할당할 수 없는 변수가 된다.
* Wrapper class
  * 
* Synchronized
  * 
* ThreadLocal
  * 
* String, StringBuilder, StringBuffer
  * 
* ==와 equals()의 차이
  * == 연산자는 참조형을 비교할 때 `레퍼런스를 비교`하고 eqals()는 참조형을 비교할 때 `값을 비교`
* 기본형과 참조형의 차이점
  * 기본형: boolean, char, byte, short, int, long, float, double
  * 참조형: 기본형 8가지를 제외한 나머지 타입
  * 참조형은 할당연산자 사용 시에 값의 주소가 전달되고 기본형은 값 자체가 전달
* non-static과 static 멤버의 차이
  * 
* 변수의 종류와 메모리 구조
  * 
* reflection
  * 
* Java Thread
  * 
* Java String
  * 
* int와 short
  * 
* equals() 메소드 동작 원리
  * 
* Integer vs int
  * 
* Casting(업케스팅, 다운케스팅)
  * 
* 고유 락
  * 
* Promotion & Casting
  * 
* Error & Exception
  * 
* Java7에서 Java8로 올라오면서 달라진 점
  *


### Design
* 영화관 좌석 예매 프로그램을 만들려고 한다. 해당 좌석에 대해 어떤 자료구조를 사용할 것인가?
  * 영화관 자석 예매 시 좌석에 대해 동시적인 접근이 이뤄지므로 동기화 처리가 이뤄진 자료구조를 사용해야한다.
  * 탐색 관점에 있어서는 Array가 빠를 것 같다.
* 은행에서 송금을 하는 과정이 3단계로 되어 있는데 3단계에서 오류가 났다. 어떻게 해야하는가?
  * ACID의 A의 원칙에 따라 전체를 Rollback 해야한다.
* DB 관점에서 제한된 리소스로 인해 트래픽의 요청이 많아 대해서 어려움을 겪고 있을때 해결할 수 있는 방법은 무엇인가?
  * 커넥션 풀을 이용하거나 메모리 캐시 DB를 이용한다.
* 서버 인스턴스를 여러 개 돌릴 때 어떤 걸 고려해야되나?
  * 공유 자원에 대한 쓰기가 있을 경우 동기화가 이뤄져야한다.
* 다수의 서버에서 어떻게 로그를 모니터링할 것인가?
  * 


### Live Coding
* (트리 형태의 숫자를 주고) 주어진 모양의 트리를 정의하고 DFS 알고리즘을 구현하라.
* (1이상 100이하 숫자 N개가 주어 지고) 이 N개의 수의 최소 공배수를 구하라.
* 주어진 문자열이 반대로 뒤집어도 같은 글자인지 찾는 알고리즘을 구현하라.
* 숫자가 들어있는 배열이 있을 때, 중복되는 숫자가 있는지 찾는 알고리즘을 구현하라.
* Factorial을 구하는 함수를 재귀로 짜보세요.
* 대각선이 고정인 행렬인 pivotal 3x3, 4x4를 뒤집는 로직을 재귀로 짜보세요.
* atoi 함수를 구현하세요.
* String으로 있는 출근 시간/퇴근 시간의 나열에서 내림차순으로 정렬하는 함수를 구현하세요.
* 10진수로 입력받은 수를 입력받은 진수로 변환하는 함수를 구현하세요.
* Binary Search(이진 탐색)를 구현해보세요.
