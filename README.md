# sk infosec cloud ai 전문가 양성 과정

# 클라우드 


***
#### 20/08/04
#### 
1. 4차 산업 혁명
    * I C B M -> A B C D
    * AI > 예측 & 추천 시스템 => 데이터 처리의 목적은 예측이다.
    * CLOUD > 데이터 저장 공간
    * POINT 는 위 모든 것들은 네트워크가 필수다.
        * HYPER CONNECTIVELY
    * __WHAT & HOW & INSIGHT__
        - 데이터 처리할때 알려주신 FLOW로 해야한다.
        - 활용할때 기획부터 생각해야한다.
    
    + __기획>수집>저장>처리>분석>시각화>활용__
           

2. 데이터 처리의 종류
    - 데이터 베이스의 목적 __1) 저장 2) 검색 3) 중복처리__
* RDMBS(관계형 데이터 베이스)
    - 1. 오라클
    - 2. MS SQL
    - 3. My SQL
    - 4. SYBASE
    - 5. DB2 (은행권)
    - 6. SQL LITE (모바일)
* NOSQL
    - 1. MONGO DB
    - 2. HADOOP = HBASE
    - 3. RE1+4


3. INTRO
    * 인공지능 적용 기술 
        - HADOOP, SPARK, 등등
    * 머신러닝/디벌닝 프로젝트 단계
        - INPUT으로 DATA와 결과값이 같이 들어간다.
            - 그러면 패턴을 찾아낸다.
    * 

***
***
#### 클라우드 컴퓨팅 basic

1. 클라우드 가상기술
    * 가상머신 : OS 중심
    * 컨테이너 : 이미지(DB 서버 서비스 중심)

    + __방법__
        - 1) 통합
            - EX) 그리딩 컴퓨팅
                - 슈퍼컴퓨터만큼의 성능이 나온다.
        - 2) 분할
            - EX) 서버를 10개로 나눠줌. OS 뿐만 아니라 CPU, MEMORY 등 다~ 가능하다!
    + __기술__
        - 1) CPU
        - 2) MEMORY -> 가장 먼저 가상화 기술을 적용한 분야
        - 3) STORY
        - 4) NETWORK
    + __Scale Out__, __Scale Up__
        - up> 이건 잘 안함
        - out> 박스를 여러개 만들어서 확장시켜줌(늘려줌)
            - 도커 컴포스, 쿠버네틱스 등에서 scale out에서 갯수를 정할 수 있다. 
            - ★용어 알아두기★

    * 가상화 기술의 핵심
        - 하이퍼바이저(virture box)와 가상화
        - pc에 리눅스 깔기(가상머신 올려서 설치)
        - 금요일에 openstack을 할 예정이다.  

***

##### principles of cloud computing
* 정의
    - 정의 : 클라우드 컴퓨팅은 __인터넷__ 기술을 이용하여 내 외부 고객들에게 __확장성(scalable)__ 있고 __탄력적인(elastic)__ it서비스가 제공되는 형식
    - cloud is a style of computing where scalable and elastic it-related capabilities are provided as a service to customer using internet technologies
    - __회복성__
    - 확장성(범위성)은 늘어나는 것만이 아니라 줄어드는 것도 포함
    - 컴퓨팅 자원이 필요한 만큼 늘어나거나 적정 수준으로 줄어들 수 있음
    - 이러한 작업이 수분에서 수십분 이내로 가능
    - 확장성은 범위, 탄력성은 시가
    - ★용어 알아두기- 확장성, 탄력성, 회복성, scale up, scale out★ 
    - <img src="/uploads/950ec59c2162630d5bc7f204b0667ee9/image.png" width = "60%"></img>
    - scale up/out 알아둬라
    - 위 확장성, 탄력성, 회복성은 가상화 기술 덕분이다.

    ***
    * *최근 사람들이 클라우드로 하고 싶은 것*
    1. 자동화
    2. 관리(장애대응(복구), 보안)
        - 최근 관리를 __오케스트레이션__ 이라는 단어를 쓴다.
    3. 오토 -> ai로 어떠한 시간대에 빠른 곳이 어딘지 확인할 수 있다.

***
***
***

#### 20/08/05

* __Service (at IT)__
    - 최종목표 : 고객 만족(CREATE VALUE)
        + 요구사항 (기능)
            - DATA 분석의 목적이 고객의 요구사항을 만족하는 것
            - EX) APPLE은 고객에게 요구사항을 만족시키기 위해 노력한다.
            - 뉴코아) VIP에게 요구사항을 물어봤다 <- 유럽풍으로 만들어 줄 것을 요구
        + 유지(복구 & 보안)
            - EX) ATM기기 24시간 서비스 -> 장애, 서비스 점검 기간 등등
            - 원래 24시간 약속을 하였으나, 서비스를 받으려고 했는데 받고싶을때 갔는데 안되는 것이 많아서 못하는 등등 유지가 잘 안되서 고객이 불만을 이야기하기 시작했다.
        ##### 결국 __요구사항__ 과 __유지__ 는 AND 조건이다!! 
        - <img src ="/uploads/6dc74b196840d16382d4efb862bd247c/image.png" width = "60%"></img>
        - ITIL
            - ITIL(Information Technology Infrastructure Library)은 'IT 서비스 관리' 분야에서 전세계적으로 검증 및 적용되는 유일한 표준모델(Best Practice)이다.
            - 1986년 영국정부 산하의 CCTA에 의해 개발된 IT 서비스 관리 분야의 업계 최고 실행 지침서이면서 IT 서비스 관리(ITSM)를 위한 품질 모델이기도 하다. (전세계 10,000여개 이상의 기업에서 적용)
            - IT에서 있어서 필요한 6개의 프레임워크(Key process & Best practice)로 구성되어 있다.
                1. Planning for Service Management
                2. Business Perspective
                3. Application Management
                4. Infrastructure Management
                5. Service Delivery
                6. Service Support
        - ITSM 
        - ISO20000 : ITIL과 ITSM이 잘 되고 있는지 인증하는 제도
        - [ITIL과 ITSM의 내용 블로그](https://cutewebi.tistory.com/720)

#### __★ 용어정리__
- .
    1. EVENT : 프로그램에 의해 감지되고 처리될 수 있는 동작이나 사건을 말한다
        - 상태가 조금이라도 변하면 EVENT가 발생한다고 말한다. 여러가지에 대한 로그가 있지만 변화가 있으면 발생되는 것이 이벤트이다. 
    2. INCIDENT : 장애, 임시 방편의 복구
        - 예를 들어 네트워크 선이 끊겼는데 이것을 손으로 잡고 있는 것 정도이다.
    3. PROBLEM : 근본원인
        - 예를 들어 끊긴 선을 새것으로 교체하는 것이다.
    4. BCP / DRP
        - 재해복구
        - BCP(Business continuity planning)
        - DRP(Disaster recovery planning )
        - BCM(Business continuity Management)
            - BCM 체계는 재난 또는 재해 발생시 고객에게 제품 또는 서비스를 지속적으로 공급하고 내부적으로는 재무 또는 운영적 영향을 최소화 시키고 비즈니스의 연속성을 확보하기 위한 경영관리 기법입니다.
            - BCM이 가장 잘 된 곳이 영국이다. 홍수 예방 훈련을 한 이후, 홈페이지에 올리구 보완점을 적어놓는다.
            - 런던시 홈페이지 들어가면 이런거 잘 되어있다.
        - 교육 = 지식전달 / 훈련 = 직접 해보고 몸으로 느끼는 것
        - 국제표준 ISO22301
        - 보안 ISO27001

    * 클라우드 활용 프로그램
        - 직방, 음악 스트리밍, 모바일 비즈니스 플랫폼 등등

    * 처음 들어가는 비용 -> CAPITAL 비용(Capex)
    * 나중에 들어가는 비용 -> OPERATION 비용(Opex)
        - it 부서는 벌어오기 보다는 돈을 자꾸 쓴다. 
        - 설득을 위한 tip : __1> 법 2> 돈 많이 벌어준다.(수악창출) 3> 비용을 절감한다고 이야기한다.(비용 절감)__ 
        - ex) 종이 -> 비용 절감, 보안 -> 방어를 못할 경우 피해액을 돈으로 계산

* 클라우드 컴퓨팅의 정의
    - 클라우드 컴퓨팅은 서비스 제공자의 최소한의 관리나 개입만으로도 신속하게 생성/제거/구성 할 ㅜㅅ 있는 공유 공간의 컴퓨팅 자원들을 언제, 어디서, 어떤 단말인지와 관계없이 필요할 때 편리하게 네트워크에 접속할 수 있게 하는 모델
    - [국가법령정보센터](http://www.law.go.kr/)
    - it를 해도 정보보호법 등이 필요하다. 
    
    - [클라우드컴퓨팅 발전 및 이용자 보호에 관한 법률](http://www.law.go.kr/lsSc.do?section=&menuId=1&subMenuId=15&tabMenuId=81&eventGubun=060101&query=%EA%B0%9C%EC%9D%B8%EC%A0%95%EB%B3%B4%EB%B3%B4%ED%98%B8%EB%B2%95#undefined)
    - <img src="/uploads/8b5cb3c60cf0c31bbe51392160e5fb86/image.png" width = "60%"></img>
    - <img src="/uploads/40f482b942c265f109e6c4f5544403f0/image.png" width = "60%"></img>
    - 인프라, os 전쟁의 이유 -> 표 참고
    - 드론 요즘 it 센터도 드론으로 한다.
    - 클라우드 마켓들이 많이 쓰고 있다.
* __클라우드로 얻는 이익들__
    - 1. 비용이 줄어든다.
    - 2. 자동화(automated)
    - 3. 온디멘드(확장성, 유연성, 탄력성)
    - 4. 이동성
    - 5. 자원에 대한 공유(multi tenancy)
    - 6. agility and scalability
    - 7. back to core business
    - 8. More IT functionality for a lower price
    - 클라우드 <-> 온프레미스

* __클라우드의 단점들__
    - 1. 인터넷이 안되면 클라우드를 못쓴다
    - 2. 보안
    - 3. 개인정보
    - 4. vendor에 종속됨 (aws->azure / azure->aws가 쉽지 않다)

* __★ 클라우드 용어(시험)__
======
- ![image](/uploads/169f55cebc10421af9e30c67c5a1b577/image.png)
    1. NIST
    2. CLOUD FOUNDATION 
    3. SaaS PaaS IaaS
    4. deployment model은 public, private, hybrid, community 가 있다.

* __클라우드 특징__
    1. 주문형 셀프 서비스
    2. 광대역망 액세스(네트워크를 이용한 any time, any place, any device로!)
    3. 자원 공동관리
    4. 빠른 요구탄력성
        - 비즈니스 상황에 따른 컴퓨팅자원의 탄력적 사용
    5. 도수제
        - pay per use, pay as you go
        - 기준을 만들고 평가한다.   
        * 네트워크란? : 쉽게 생각하면 통신이다. 서로 왔다갔다 메세지를 던지는게 규약이고 그렇게 정의된게 네트워크이다. 정확하게 규약대로 통신하자고 만든게 네트워크이다. 쓸 때 규약하는 것은 파일을 전송할때는 ftp로 21:21 쓴다. 이래야 파일이라고 생각한다.
        * 그렇닌까 네트워크는 통신이고 규약이다.

* DEPLOY MODEL

    1. PUBLIC
    - <img src="/uploads/1b8eae03311893814a38b1d3ed0be97a/image.png" width = "60%"></img>
        - 퍼블릭클라우드인프라는인터넷을통해공개적으로사용가능
        - IT 인프라는퍼블릭클라우드서비스를제공하는업체가소유
        - 클라우드서비스이용자를제한하지않는방식
        - 인터넷접속이가능한모든사용자를위한클라우드서비스
        - 서비스내부에저장된데이터나서버자원은사용자별로권한관리
        - 사용자간에데이터간섭이없도록관리(Multi-Tenancy)
    2. PRIVATE
    - <img src="/uploads/ac7d715236aa74b27cb332f773421fb4/image.png" width = "60%"></img>
        - 프라이빗클라우드는폐쇄적인구조로운영
        - 특정기업의특정사용자만을대상으로하는클라우드서비스
        - 컴퓨팅자원과저장데이터가기업내부에저장
        - 자원과데이터의제어권을기업자체에서가지고있음
        - 물리적인데이터보안측면이퍼블릭클라우드보다강함
        - IT 인프라는해당기관또는타사에의해관리
    3. COMMUNITY
    4. HYBRID
    ***
    - ![image](/uploads/25628abb9d5a4124773cc18f5fa4bb10/image.png)
    * __차세대 네트워크__
        - 송신자 수신자만 있으면 좋은데 그게 안되서 SWITCH, ROUTER 등 여러가지 경로에 의해 공유한다. 이게 다 장비였는데, 네트워크에 관한 용어 중에서 SDN, NFV 등이라는 게 나왔다.
        - "영국의 손흥민 VS 서울의 아이" SK 광고 다~ 차세대 네트워크를 활용한거다.
            - __SDN : SOFT DEFINE NETWORK__
                - 소프트웨어도 네트워크로 지정하자
            - __NFV : NETWORK FUNCTION VIRTURE__
                - 네트워크도 가상기술을 활용하자
    <span style = "color:gray">
    + 알고리즘 = 프로그래밍
        > 무엇을 할까를 고민을 많이 해봐라
        > 어떻게 업무를 할까?
        > 회사에 간다고 할때 제일 중요한 것은 업무이다.
        > __업무를 빨리 파악하는게 중요하다.__
    + 인공지능과 보안
        > - __인공지능을 활용한 보안__ 
        >       - 결정할 수 있는 사람이 별로 없다. 인공지능이 이러한 결정을 도와줄 수 있다.
                - 잘 못 결정하면 뒤집어진다. 관제에서는 이러한 상황에 해결이 아니라 결정을 물어본다. 이럴때 AI로 도움을 주기 위한 이러한 것들을 하면 좋다.
                - 한국 전파 연구소에서 VNP 테스트 해서 인가 허가가 나야 공공에 솔루션이 들어갈 수 있다.
                - 백신 프로그램에 대한 인공지능 접목
                - __보안 안에서 인공지능 활용__
        > - __인공지능 기능에 대한 보안__
                - 인공지능 칩셋 위협 및 취약점
                - 머신러닝/딥러닝 모델링 위협 및 취약점
                - 데이터 처리 취약점
    </span>
    
<span style = "color:red">
point  1. 네트워크  2. virture machine
</span>
    
***
- ![image](/uploads/0aadad92410f6b29a6a0b031cb6c631d/image.png)
- container는 보통 리눅스로 깐다.
- container는 서비스 단위이다. os랑은 별 상관 없다.
***
#### 가상화(virtualizaion)
* __이거 시험문제로 출제될 예정이다. ★__
         
* 실제로 존재하지 않는 것을 존재하는 것처럼 보여줌 
    - 70's IBM에서 시도
    - 대상 : 모든 IT 자원들
    - 방법
        1. 자원 가상화
            - 물리적 자원을 다른 특성을 지닌 별도의 논리자원으로 보여주는 것
                - HDD(하드웨어)는 FS(WINDOW = NTFS / LINUX = EXT4)
                - MEMORY(메모리)는 주소(address)형식이다.
            - 가상메모리 = 주기억장치(물리적 메모리) + 보조기억장치(하드디스크)
            - 특히 메모리쪽에 있는 것들!!
        2. 자원 분할
            - 단일 물리 자원을 논리적으로 분할하여 별도의 물리자원으로 인식, 동작
            - 서버 가상화 : 한대의 서버 위에서 여러 개의 os를 동시에 운영
        3. 자원 통합 
            - 복수의 물리 자원을 논리적으로 통합하여 단일한 물리 자원처럼 동작
            - 서버 클러스트링
            
        + __즉, 모드 it자원에 가상화를 적용할 수 있다.__

        ***

        1. 서버 분할
            * 파티셔닝
            * 가상머신
        2. 서버 통합
            - 클러스터링
            * HA 클러스터링 : 복수의 서버를 통합하여 단일 서버 이상의 높은 가용성 지원
            * 부하분산 클러스터링 (= 로드밸런스) 
                + (1) 로드 밸런스(ROAD BALANCE) : 이것들을 분산하는 것의 기능을 알아야한다.
                + (2) 우선순위를 만든다
                + (3) 로드밸런스를 할때 서버 통합들을 한다.
                + 컨테이너 만드는데 활용한다.
                + [정리하기 다음의 링크 보고](https://asfirstalways.tistory.com/320)

        ***
        <img src = "/uploads/fe69a9b914c2357b97012e18ff4ab553/image.png" width = "60%"></img>


        
|레이드 |설명|
|-------|------------------------------------------:|
|raid 0|Striped disk array without fault tolerance|
|raid 1|Mirroring and duplexing|
|raid 2|Hamming code ECC|
|raid 3|Parallel transfer with parity|
|raid 4|Independent data disks with shared parity disk|
|raid 5|Independent data disks with distributed parity blocks|
        * raid5라면? 디스크를 5개를 만드는 것
        * [raid 개념](https://raisonde.tistory.com/entry/RAID0%EB%B6%80%ED%84%B0-RAID7%EA%B9%8C%EC%A7%80-%EB%AA%A8%EB%93%A0-RAID%EA%B5%AC%EC%84%B1%EC%9D%84-%EC%95%8C%EC%95%84%EB%B3%B4%EC%9E%90)

        ***
        * __SDN__ : 개방형 API를 사용하여 소프트웨어 애플리케이션을 통해 중앙에서 제어되는 방식으로 네트워크 동작을 프로그래밍할 수 있도록 해줍니다. 기존의 폐쇄형 네트워크 플랫폼을 개방하고 공통 SDN 제어 계층을 구현함으로써 사업자는 기본 네트워크 기술의 복잡성에 상관없이 전체 네트워크와 해당 장치를 일관성 있게 관리할 수 있습니다.
|부분|방법|
|----------|-----|
|APPLICATION|S/W|
|CONTROL|S/W|
|DATA 통신|H/W|
                - 위 표를 하드웨어 하나로 3개 다 만드는게 SDN이다. 
                - 각 부분들을 각각 연결해야한다.
                - CONTROL -> APPLICATION : NBA
                - CONTROL -> DATA통신 : SBA
            - 가상화를 하드웨어로 만들 때 장점 : 속도가 빨라진다.
            - 가상화를 소프트웨어로 만들 때 장점 : 비용이 절감된다.
        ***
        * __NFV__ : 범용PC에 NETWORK기능을 가상화한다. 스위치 10개 라우터 2개, 방화벽 2개 등 만든다.
            - 장비를 살 필요 없이 가상화로 기능을 구성할 수 있다. 이게 바로 NFV 기능이다.
        + __SDDC__ : soft design data center
            : 기능들을 전부다 가상화시키고 소프트화한다. 기기가 온도 습도 다 알아준다. 정말 하드웨어에 관한 것은 어쩔 수 없지만 컨트롤하는 부분을 소프트웨어로 define해준다. 따라서 it 센터가 작아도 할 수 있다.
                + 전력적으로 줄일 수 있다.(__비용 감소__)
        
        <span style = "color:blue">
        

        - *__비용감소__*
        - *__자원 활용성__*
        - *__높은 확장성(서버 등)__*
        - *__가용성__*
        - *__운영관리__*    
    </span>  
    + ![image](/uploads/924757138bd472e48f6b413605213a4c/image.png)
    - 이런 것들도 다 알아야 한다.
    - __VLAN__ : 물리적인 포트들을 논리적으로 가상화 시키는 것이다.
    * TYPE
        -  하드웨어 구성요소 
            - 서버 
            - 스토리지 
            - 네트워크 인터페이스 카드 
            - 스위치 
        - 기능 
            - 서버수, 
            - CPU, 캐시, 
            - 스토리지 시스템 
            - I/O • 하이퍼바이저 
            - 가상머신 
            - 가상 네트워크 
            - 가상 네트워크 기능(VNF) 
            - 확장성

******


### vagrant 실습
- ![image](/uploads/3425778d59d107ecb6ff68b7f856995d/image.png)
1. 가상머신 설치
2. vagrant 설치
3. vagrant 설치 후 실행
4. cmd창 열어서 다음 입력
<pre><code>
vagrant version
C:\> mkdir virtual-test
C:\> cd virtual-test
C:\virtual-test> vagrant box add ubuntu/trusty64
C:\virtual-test> vagrant init ubuntu/trusty64
</code></pre>
5. 메모장으로 열어서 수정하기
- <img src="/uploads/b6f59345a3c90d8981af7629e4f0e72e/image.png" width ="40%"></img>
- <img src="/uploads/132a51a7093b0a40957468fb81a1c173/image.png" width ="40%"></img>
- <img src="/uploads/7bf40afbcac289762f35eeeeb8799d3f/image.png" width ="40%"></img>
- 위와 같이 수정 후 저장
6. ```vagrant up``` 입력
- ![image](/uploads/a35ff3b4b3782bd0f67c5a5abf44ebaa/image.png)
7. id, pw는 vagrant로 초기화
8. window와 linux 공유하기
    - ![image](/uploads/3df20a068a320f979decd07a732e9d0a/image.png)
    - 1) mkdir로 testing 파일 만들기
    - 2)<img src="/uploads/afc70ba203eded38462a39d55ae27990/image.png" width ="80%"></img>
    - halt로 재시작 후 up한다.
    - 이후 virture box 내에서 ls하면 화면이 추가된 것을 확인할 수 있다.


***
***

#### 20/08/06

* 책 추천 : 모두의 딥러닝

* 복습 및 추가
    * 가상화의 장점
        - 비용 감소
        - 자원(리소스)의 유효 활용
        - 높은 확장성
        - 가용성 향상
            - 가용성이란? 얼마나 계속해서 쓸 수 있도록 하는가?
            - 보안의 3요소 
                1. 기밀성 : 비 인가된 사람이 들어올 수 없다.
                    - by 암호화
                2. 무결성 : 자산의 완전성과 정확성을 보장
                    - by __해시__ 알고리즘
                    - 해시는 블록체인에서 많이 쓴다. 그리고 비밀번호에도 많이 씀!!!
                    - sam파일에 가면 window pw알 수 있다. 
                3. 가용성 : 인가된 사람이 쓸 수 있다.
                    - 고객의 서비스 만족등 기능 + 유지이다. 이게 보안에서도 실제저으로 사용하기 원하는데 사용ㅇㄹ 못하면 문제가 있다고 판단한다. 가용성을 떨어뜨리게 한다.
                    - 가용성 계산식 >  운영-장애난 시간 / 운영시간
                    - 99.88%이상 되어야 한다.
                    * __downtime__ 이란
                        - __planed down time__ : update, upgrade
                        - __unplaned down time__ : 장애
                            - sla 작성 시 이런 내용 주의해야한다.
                            - point는 planed down time이 가용성 계산식에 어떻게 처리되어야 하는가(장애난 시간 포함 불포함)
                    - __가용성__ 이란 그럼 무엇인가?
                        
        - 운영관리 개선
            - PDCA이론이란?
                - PLAN DO CHECH ACT
                - 미국 데밍이론 / IT 프레임워크
                - 목적 : __개선__
                    - 기준 -> 평가 -> PDCA를 계속함 -> 개선
                    - EX) 공공기관의 기준 = 법, 선진사례, 
            - 데이터 분석하러 가서 젤 먼저 할일 : __현황파악__
                - 즉, 업무분석
                - 경영 컨설팅 -> 돈 많이 범
            - 현황파악 과정
                1. 조직도 보기
                    - 직무기술서가 정확하게 DEFINE되어 있는게 직무기술서. 조직도라함. 연봉 협상에 해당됨
                2. 시스템 구성도 / 네트워크 구성도 확인
                3. 사내 업무 분석

### 도커

* 컨테이너 어플리케이션이 중요해서 사용한다.
* virture machine에 비해 성능 손실이 적고 가볍고 이식성이 좋다
* 단 인터넷이 안되는 회사의 경우 
    - 인트라넷 안에서도 도커 이용할 수 있다.
    - 대부분 리눅스에서 사용한다. 
    - 컨테ㅣ너가 하나의 os를 고유한다.
    - cpu를 가상화하지는 않는다. 
    - EC2로 컨테이너를 해볼 기회가 있다.
    
### DB
* <img src = "/uploads/5ad885ba7cbfd8f825ff52d8a69b94fe/image.png" width = "60%"></img>

<span style = "color:gray">
* 포트폴리오 -> 이 병원에 10년간 다닌다는 전제하에 포트폴리오로 작성한 사람이 합격했다.
* sk에서 합격시켜준다고 하더라도 공부 많이 하고 들어가라!
</span>

### MSA (마이크로 서비스)
* 서비스를 작게 쪼개는 것
* 회원관리
    - 회원 등록
    - 회원 조회
    - 회원 수정
    - 회원 탈퇴 등등...
- 그렇게 다 나누면 장애가 발생하더라도 ok
- 카카오, 배민 쪽은 MSA를 많이 도입하고, 대기업도 도입하고자 한다.
- 왜냐하면 유연한 조직이 됨
- [MSA를 통한 유연한 조직&서비스](https://velog.io/@tedigom/MSA-%EC%A0%9C%EB%8C%80%EB%A1%9C-%EC%9D%B4%ED%95%B4%ED%95%98%EA%B8%B0-1-MSA%EC%9D%98-%EA%B8%B0%EB%B3%B8-%EA%B0%9C%EB%85%90-3sk28yrv0e)
- MSA를 도입하기 가장 좋은 환경은 __컨테이너 -> 도커!__

* __MSA를 구현할 때 고려사항__
    - <span style = "color:red">(1) 업무파악(현황분석)</span>
    - <span style = "color:red">(2) 식별(분할)</span>
    - <span style = "color:red">(3) 인터페이스</span>
    - <span style = "color:red">(4) 관리(장애,보안)</span>

  
    * bridge방식
        - .
    * host방식
        - 리눅스와 연결하는 것
    ##### docker file로 서버구축 명령어

    |명령어|설명|명령어 |설명|
    |:------|:-------------------|:------|:-------------------|
    |FROM| 베이스 이미지 지정 |ADD| 파일 및 디렉터리 추가|
    |MAINTAINER| Dockerfile 생성자 |COPY| 파일 복사|
    |RUN| 커맨드 실행 |VOLUME| 볼륨 마운트|
    |CMD| 데몬 실행 |ENTRYPOINT| 데몬 실행|
    |LABEL| 라벨 설정 |USER| 사용자 설정|
    |EXPOSE |포트 export |WORKDIR| 작업 디렉터리 지정|
    |ENV |환경 변수 설정 |ONBUILD |build 완료 후 실행될 명령어|

---
* 기업에서 젠킨스, 일렉트리 서치 등을 많이 쓴다.

    ##### 컨테이너통합관리(Docker Compose)
    |서브| 커맨드 설명|
    |-----|----------|
    |up | 컨테이너 생성 및 구동|
    |scale | 생성할 컨테이너 개수 지정|
    |ps | 컨테이너 목록 확인|
    |logs | 컨테이너 로그 출력|
    |run | 컨테이너 실행|
    |start | 컨테이너 구동|
    |stop | 컨테이너 중지|
    |restart | 컨테이너 재기동|
    |kill | 실행중인 컨테이너 강제 종료|
    |rm | 컨테이너 삭제|


* YAML파일
    - TXT로 썼지만, YAML로 해야한다.

#### Apache Hadoop
* 하둡
    * 수집 및 정제된 데이터를 효과적으로 분석하는 기술 필요
    * 대량의 작업을 병렬 및 분산 처리하여 성능 향상
        - 과거의 BIG DATA -> GFS(google file system) 
            - : 구글에서 생각하다 보니, 빅데이터 하다 인공지능하면 시간이 너무 많이 들었다. GFS를 고안했다. __MapReduce__ 를 써서 했더니 속도도 빨랐다. 엄청난 속도로 검색 가능
            - 이에 hadoop진영에서 이러한 것들을 만들었다. 그래서 hadoop이 이겼다.
    * 병렬시스템 : 처리를위해CPU 등자원을데이터버스나로컬통신시스템             등으로연결하여분할된작업을병렬로동시에처리하여속도를빠르게한 시스템

    * 분산시스템 :  네트워크상의분산된컴퓨터를단일시스템형태로운영하는
        시스템으로써분산시스템에속한각노드는독립된시스템이있어야하며
        독립컴퓨터의집합으로만들었으나단일시스템의역할을수행

    * HDFS(Hadoop Distributed File System)
        - 맵리듀스 : 하나의 큰 데이터를 여러개의 조각으로 나누어 처리하는 map단계이다.
        - map으로 들어가서 reduce로 나오는 알고리즘이다.

    * 기본 data block의 크기는 64mb가 기본이며 여러 node에 복사본을 생성한다.
    * [맵리듀스](https://terms.naver.com/entry.nhn?docId=3386313&cid=58370&categoryId=58370)
    * ![image](/uploads/41cf4e41c531b6da889541d513475856/image.png)
    * ![image](/uploads/ef1e07530817e760dffe74383a089665/image.png)
    * ![image](/uploads/5a973538238fe759db49043b84be2dbd/image.png)
    * ======================================================================
    * 여기서 이에 대한 대체점으로 SPARK를 만들었다.

#### OPEN STACK
* Cloud Computing Platform software
    - iaas cloud에서 사용됨
    - 라이센스 없이 사용 가능하다
    - 사람들이 클라우드를 쓴다 = 가상서버 내 서비스를 선택해서 서버를 구현하여 쓰겠다는 소리이다.
    - 서비스 선택은 내가 하는 것이다.
    - *실습은 azure로 하면 들어가서 설정하는 방법을 하는 것이다. file server 만들라고 하면 만들고, 방화벽 만들어서 셋팅할 예정이다. 이게 aws와 azure에서 배우는 내용이다.*
    - point는 aws와 azure의 용어를 알아들어야 한다.
    - ex) E2C != ? 있긴 있음
    - *시험문제는 다룰 수 있는 방법을 이야기하는 것이다.*
        1. GUI 마우스로 할 수 있다.
        2. command(명령어)로 할 수 있다. -> powershell로 명령어 쳐서 쓴다.
        3. program 프로그램 돌릴 수 있다.

* single sign이 보완적으로 더 낫다.
    - tocken에 따라서 왔다고 확인하고, 이것을 키스톤이라고 한다.
    - ![image](/uploads/98564e61eddf08244213e6a64ead2e13/image.png)
    - aws와 azure가 이러한 open stack을 더 사용하기 쉽게 만들어준다.


* nova
    - 
* glance
    - 
* cinder
    - 
* swift
    - 오브젝트 스토리지 서비스 저장
    - 다른 서비스와 달리 단독으로 구성
    - 클라우드 스토리지 서비스 구성
* neutron
    - 버전에 따라 다른데 네트워크 설정을 담당한다.
    - 

***
* 오픈스텍 실습
    - user1, user2등 이름(영문)으로 적기!
    - 유니크한게 좋다.
    
### 2020/08/07
### 오픈스택 설치
<span style = "color:gray">
심사갈 때 보통 리눅스 명령어, 도스 명령어들을 알아야 한다. 
net share은 안된다고 말한다. c는 기본공유하면 안된다. 

그 이유는???

    - ipc는 프린트 할때 쓰는 것(어쩔 수 없는 부분)
    - 해커가 해킹을 했을 때 보통 하는게 기본공유를 찔러서 금방 들어올 수 있다.
    - 한대라도 기본공유가 풀려있는 경우 네트워크를 통해서 다 다들어올 수 있다.
아이피 주소를 알면 바로 크래킹 가능하기 때문이다.
[net share1](http://blog.daum.net/99lib/336)
[net share2](http://itwiki.kr/w/%EC%9C%88%EB%8F%84%EC%9A%B0_net_share)
</span>

#### SDN
- SDN/OPEN FLOW 기술 개요
- 5G는 갔다. 이제 6G를 준비해야한다.
- 3가지 부분으로 만든다.
1. DATA PLANE 영역 : 데이터 전송을 담당하는 하드웨어 영역
2. CONTROL PLANE 영역 : 운영체제 기능을 담당하는 소프트웨어 영역
3. APPLICATION 영역 : 네트워크 지능화 기능을 담당하는 소프트웨어 영역
* __여기 이야기 2번하심, 개중요함__
- 원래는 중앙집중형 환경에서는 소프트웨어 영역과 하드웨어 영역을 분리함으로써 전체 네트워크는 중앙의 컨트롤 플레인을 통해 단일화
- 이렇게 중앙집중형 환경을 하려면 표준화가 필요하다. 그게 바로 다 소프트웨어로 표준화 시키겠다는 이야기이다.
- 시스코의 벤더에 종속되어서 사람들이 싫어한다. 그래서 이것들을 종속되지 않도록 전체적ㅇ로 다 같이 쓰기 위해서 __표준화__ 가 필요한 것이고, 이것들을 위해 만들어 놓고 OPEN FLOW가 그거고 여기서 상태 확인하고 명령 내리는게 OPEN INTERFACE이다.
- 위로 간다 : NORTH BOUND INTERFACE => __NBI__
- 아래로 간다 : SOUTH BOUND INTERFACE => __SBI__
- ![image](/uploads/dc04c26cfc62dd86651e6c65562936f6/image.png)
* 데이터 분석
<span style = 'color:red'>
    - __1> 회귀분석__
    - __2> 상관관계__
    - __3> 가설검증__
</span>


#### NFV

* 가상화 네트워크 기능을 만든다.
    - (1) 분리
    - (2) 유연성
    - (3) 동적운영
1. NFVI(Network Functions Virtualization Infrastructure, 네트워크 기능 가상화 인프라스트럭처) 블록 
    - 전체 아키첵처의 기반 
    - 가상 머신을 담은 하드웨어, 가상화를 구현하는 소프트웨어 및 가상화된 자 원이 이 블록에 포함 
    - *__가상화__ 를 SDN으로 구현한다!!*
2. VNF(Virtualized Network Function, 가상화 네트워크 기능) 블록
    -  VNF블록은 NFVI에서 제공하는 가상 머신을 사용
    - 그 위에 가상화된 네트워크 기능을 구현하는 소프트웨어를 추가해 NFVI위 에 구성
3. 관리 : mano블록 
    - 자원을 생성하고 삭제한다. => management

<span>
- 4번 오케스트레이터가 판단
- 5번 만들어야 한다고 말함 -> 가상화 vim에 명령을 입력하고 다 만들면 다시 7번 오케스트레이션에서 확인하다.
- 8번 그렇다면 이후 vnf 관리자에게 넘어가서 기능들을 vnf로 만들어야 한다고 명령한다.
- 그러면 em이라던가 vnf가 만드니 이후 다 만들었다고 보고한다. 
</span>


***
- window에서는 activity directory라는 것을 많이 사용한다.
- cloud에서의 자격과 각각의 instance라던가 할 수 있는지 정해놓는게 중요
- r back이 역할기반이라고 한다. 역할에 따라서 권한을 주고 뺏는 등 인증에 대한 것들 여러가지 것들이 필요하다


### issue
1. 가용성에 대한 issue
    - sk, kt화재 등등
2. aws 서울 리전 장애 발생
    - 쿠팡, 나이키 등 여러가지 서비스 에서 영향을 받음(클라우드)
3. city은행
    - 

* __iso/iec 27001 domains & controls__

* BYOD(Bring Your Own Device)

* __보안__

|취약점|위협|
|-------------------|------------|
|내부 |외부|
|접근통제(root, admin)와 같은 슈퍼권한을 통제|해킹 해커 들이 공격하는 것|
|불필요한 서비스 통제 (test계정 같은 것, 유지보수 업체가 쓰는 계정 등)|    |

이러한 것들을 리스크라고 한다.
* 리스크(risk)란?
- <img src = "/uploads/0ef50c6ad147e4329448ea1d75914fb5/image.png" width = "60%"></img>
- mitigration : 리스크를 줄인다
- __★ risk는 클라우드 보안 시험문제 나온다 ★__

* 공용계정 사용 x인 이유
    - 누가 했는지 모른다. 그래서 1인 1계정을 사용한다.

* 유지보수 업체가 쓰는거 사용 ㄴㄴ
    - 왜냐하면 유지보수 업체가 바뀔 수 있기 때문이다.
* tirple -A
    - __인증과 인가의 차이__

    |인증|인가|
    |:---------------:|:--------------------:|
    |너가 맞는지 확인하는 것|그사람이 가지고 있는 권한이 무엇인지 , 부여하는 것|
    - 3A가 무엇이냐

* __SLA란?__
    - Service Level Agreement
    - 총 5페이지인데 다 잘 보기
    - 결론 : __cloud내에 sla를 잘 구성해야한다.__
    - [SLA](http://blog.naver.com/PostView.nhn?blogId=bnhuyf3&logNo=220248595259)

* __클라우드 컴퓨터 이전 과제__
    - 어떤시스템을클라우드서비스로전환할것인가?
    - 현재사용하고있는데이터를어떻게전환할것인가?
    - 기존시스템과의연계가필요하거나통합이기술적으로가능한가?
    - 기존소프트웨어라인선스를클라우드환경에서사용가능한가?
    - 가상CPU 코어환경에서소프트웨어라이선스비용은합리적인가?
    - 마이그레이션에어떠한기술을사용할것인가?
    - 클라우드로전환시점은언제로정할것인가?

***
***
***
## AZURE

* 네트워크를 보는 순간 문제점을 찾아내는 눈을 키워라
- 외부망, 내부망과의 연결 ?
    - ![image](/uploads/6d293f537e8323ea4bbe2c06b3511d3f/image.png)
    
    * __<클라우드 공부 순서>__
    * 사용자 및 그룹의 중요성
    * 시스템(인스턴스) 생성 및 설정
    * 인스턴스 서비스 구성
    * 인스턴스 서비스 운영 *(모니터, 관리)* => BACK UP은 어떻게? 장애대응은 어떻게? 이러한 것들을 설정하고 만들어야 함!
    * 과금 청구(기준, 평가 등등)

1. AZURE 사용자 및 그룹
* 사용자 및 그룹 관리
    - 권할을 주고 뺏을 수 있다.
    - 사이트를 보면 사용자 및 그룹 계정 만들 수 있다.
    - 사용자 관리에 대한 것들!
* ACTIVE DIRECTORY
    - AWS에는 없고 AZURE에만 가능하다
    - 한꺼번에 계정관리를 할 수 있다.
* LAB같은거 하면 할 수 있당.

* 시험 많이 나옴
    * MAC
    * DAC
    * RBAC

* 권한 설정
    - 적절성(적합성) => 최소권한 -> 과도
        - IAM (ID ACCESS MANAGEMENT)
        - 그래서 이런거 다 해놔야 한다!
    - 관리자 권한
        - ADMIN, ADMINISRATER이란 명을 쓰지 말라
* 리소스 범위
    - 리소스 그룹 및 개별 리소스에 대한 역할을 할당 할 수 있다.
    - 리소스는 상위 리소스에서 역할 할당을 상속받음
* 역할 할당
    1. 사용자
        - 구독과 관련된 AD의 조직 사용자에게 할당
        - OR 같은 디렉터리에 있는 외부 MICROSOFT 계정
    2. 그룹
        - AZURE AD 보안 그룹에 할당 됨
        - 우수 사례 : 그룹을 통한 액세스 관리, 역할 추가 및 사용자 할당
    3. 서비스 주체
        - 디렉토리에서 서비스 프린시 펄로 표현된 서비스 ID 
        - AZURE AD로 인증하고 서로 안전하게 통신

    * 최근 음성인식이 HOT ISSUE
* RBAC
    - RBAC을 사용한 사용자 엑세스 부여
* ENTERPRISE ADMINISTRATOR
    - 전체 다 관리하는 것

***

2. 모니터링 기능
[AZURE 사이트](https://docs.microsoft.com/ko-kr/azure/azure-monitor/overview#:~:text=%EB%B6%84%EC%84%9D,%20%EA%B2%BD%EA%B3%A0,%20%EC%99%B8%EB%B6%80%20%EC%8B%9C%EC%8A%A4%ED%85%9C%EC%9C%BC%EB%A1%9C%20%EC%8A%A4%ED%8A%B8%EB%A6%AC%EB%B0%8D%20%EB%93%B1%EC%9D%98%20%EC%97%AC%EB%9F%AC%20%ED%95%A8%EC%88%98%EA%B0%80%20%EC%9E%88%EC%8A%B5%EB%8B%88%EB%8B%A4.On%20the)
* 주요 기능
    - MONITOR&VISUALIZE METRICS
    - QUERY & ANALYZE LOGS
    - SETUP ALERT&ACTIONS
* Alerts 띄우기 가능
    - 통합된 저작환경
    - 향상된 작업 흐름 및 경고 알림
    - 하나의 보기로 통합
    - 사람이 설정할 수 있다. 새롭게 ~하겠다공
* 경고 규칙 만들기
    - 대상 기준 논리를 사용하여 경고 조건 정의
    - 메일로도 보내고 여러가지 확인할 수 있다.
* 이벤트 카테고리
* 활동 로그 및 로그 분석
    - power bi라는 시각화 툴을 사용하여 쓸 수 있도록 한다. 
    - 이거는 안들어가있다.

3. 스토리지
* azure 저장소
* 세가지 범주
    - 가상 컴퓨터용 저장소
    - 비정형 저장소
 
* 스토리지 액세스 도구들
    - azure port
    - storage explorer
    - power shell

4. 가상머신
    - 가상 머신 계획
    - 가상 머신 만들기
    - 가상 머신 구성
    - 가상 머신 저장소 구성
    - 가상 머신 관리
    * web, db 서버 등등 만들고~ 방화벽 만들어서 연동하는 것들!

5. 온 프레미스 대 azure가상 머신
    - 가상머신 만들기
        - 가상머신 배포 도구
[azure 기본사항 학습 경로](https://docs.microsoft.com/ko-kr/learn/paths/azure-fundamentals/)
- 총 9시간 48분이면 azure 다 배운다.