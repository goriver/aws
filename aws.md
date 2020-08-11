# sk infosec cloud ai 전문가 양성 과정

# 클라우드(aws)


***
#### 20/08/10
#### 

* 이도원 강사님
* edowon0623@gmail.com

### stackoverflow
- 1. 죽은 프로그래머 -> 다익스트라, 도널드 커누스
- 2. 성공적인 프로그래머 -> 빌게이츠, 존 카맥
- 3. 유명한 프로그래머
- 4. 일하는 프로그래머 ★
- 5. 평균적인 프로그래머
- 6. 아마추어 프로그래머

- 영어로 6하원칙에 맞게 작성해야한다.
- 여기에 글을 올리면서 올려야할 질문에 대해서 곱씹게 된다.

* hot한 기술 & 언어
    - golang
    - kafka / cassandra(nosql) / dynamondb(nosql)
        - __map reduce(deep learning)__ : 가지고 있는 데이터를 쪼개서(mapper) + 쪼갠 데이터를 다시 모은다(reduce)
        - HANA
        - CLOUDERA
* 최근 AI 기술 방향의 TREND
    * 가트너 2019 trend

# AWS 클라우드 책

# AWS를 이용한 운영 서버 환경 구축

* CLOUD 서비스를 가장 잘 활용하는 회사
    - NETFLEX : 마이크로 서비스, 데봅스 등을 잘 활용하고 있다.
        - SPRING CLOUD NETFLEX라는 오픈소스로 활용한다.
        - 서비스 중 인프라 구축에 관련된 서비스 
    - GOOGLE, AWS
* AWS는 IaaS, PaaS, SaaS가 다 있다
    * 서비스 모델 중 IaaS에 대한 정의
    - aws에서의 인프라 스트럭쳐 제공이란?
        - : 운영체제는 하드웨어가 아니다. 데이터 베이스는 middle ware라고 부른다.
        -  운영체제는 하드웨어가 있어야 하고, middle ware는 운영체제가 있어야 한다.
        - 이러한 모든 것들을 제공하는 것이 infra structure이라고 한다.
        - __aws에서 infrastructure을 제공하는것이 EC2이다.__
        - relation, storige, road balance도 하고, auto scale도 한다.
        - select 기능이 많은 서비스 -> 쇼핑몰 홈페이지
        - insert delete 기능이 많은 서비스 -> 로그 파일로 남겨야할 경우
        - 로그 파일은 짧으면 6개월 길면 몇년으로 저장
        - __즉 하나의 데이터 베이스에 쓰기와 읽기를 같이 쓰면 비 효율적이다. 그래서 같이 쓴다.__
        - 이 두 데이터 베이스는 같은 contents를 가지고 있어야한다. 이 데이터가 서로 동기화가 되어있어야한다.
        - 데이터베이스의 복제 기능은 자동으로 써달라고 하는 기능을 요청한다. 이처럼 middle ware에서는 쓸 일이 많다. 
        * __auto scale__
            - __scale up/ scale out(옆으로 늘림 -> 돈을 많이 쓸 필요 x, 복제) / scale down__
            - 즉 cpu파워에 따라 늘렸다 줄였다 하는 것이 auto scale이다.
            - 클라우드 서비스의 필수요소이다.
        * database를 제공 
            - 방법 1> iaas = 리눅스에 저장한다
            - 방법 2> paas = 클라우드에서 제공하는 db => 더 안정적이다.
    * saas
        - 바로 서비스를 사용할 수 있는 공간
    * paas
        - sdk가 설치되어있고 or db가 설치되어 있고 or tool도 설치되어 있다면, 즉 개발할 수 있는 환경을 제공해준다면 paas이다.

* instance란?
    - EC2를 이용해 실체화한 서비스

## 운영서버와 AWS 소개
- 프리티어는 한달에 750시간 까지만 무료이다. 
- 한달 내내 써도 된다. 
- 근데 서버 1개 기준이다. 10대하면 돈 더 내야할 것이다.
* POINT 
* 원칙은 리전별로 서비스가 나누어져 있다.
    - 이는 비용을 계산할 때도 중요하다. ACCOUNT당 720시간이다. 
    - 반드시 리전을 확인해라. AWS메뉴 안에서 리전을 파악하는 기능은 있지만
    - 리전은 서비스 별로 다 다르게 구축되어있는게 리전이다.
    - 사용작 많은 리전의 경우 가용 영역이 나뉘어져 있다.
    - ![image](/uploads/ad50b05b8bb8585247fe86c5f112052e/image.png)
    - 가용영역 내 데이터 센터들은 물리적으로 나뉘어져 있는데 이는 __안정성__ 과 __보안성__ 때문이다.
    - ![image](/uploads/2875229e3f8fd43a3b18601e37ad5151/image.png)
    - __VPC__ :
        - Virtual Private Cloud(VPC) — 사용자의 AWS 계정 전용 가상 네트워크입니다. 서브넷 — VPC의 IP 주소 범위입니다. 라우팅 테이블 — 네트워크 트래픽을 전달할 위치를 결정하는 데 사용되는 라우팅이라는 규칙 집합입니다. 
        - 앞쪽의 서버와 우리의 서버를 같이 해준다. 
* IAM 용어
    - 권한
        - 
    - 정책
        - 
    - 사용자
        - 
    - 그룹
        - 
    - 역할
        - 

### aws 실습
#### 애플리케이션/데이터베이스 서버 분리
* aws 프리티어 사이트 이동
* get(값을 얻음) / push(값을 보냄) 에 20,000건까지 가능
* 머신러닝 -> sagemaker로 2개월까지 가능하다.

#### AWS EC2를 이용한 서버 인스턴스 생성과 관리
* EC2 : Elastic Compute Cloud
    * 하드웨어를 선택하고 그 위에 어떠한 리소스를 가지고 할 것인지 정하고, 하드웨어 스펙을 정ㅎㄴ다음 그 위에 운영체제를 설치할 예정이다.
    - 이미지화 되어있다. 근데 그 이미지를 원래 사용할 수 있는 형태로 압축을 풀어서 사용할 수 있도록 제공하고 있다. 사용할 수 있는 이미지의 종류는 몇가지가 있는데 window / linux로 나눠진다.
    - cloud computing을 이용해서 ec2를 선택할 때는 하드웨어도 선택하고 그래야한다. 그러면 3~5분 사이에 서버가 생성된다.
    - linux서버를 사용할 경우 command에 익숙해져야한다.
* 요금 종류
    1. 사용량에 따라 지불
    2. 예약을 통한 비용 절감
        - 훨씬 저렴하게 사용 가능하다.
        - 
    3. 더 많이 사용하여 더 적은 비용 지불
    - <image src="/uploads/2d00818f91fd694565794e39157fef43/image.png" width="60%"></image>
        * Amazon Elastic Container Service
            - ecs의 컨테이너 사용시 이미지를 저장 및 검색이 가능하다.
            - docker의 가상화 서비스를 ecs 사이트에서 사용도 가능하다.
        * Beanstalk
            - python이나 java라는 플랫폼 기초에서 알아서 서버가 된다.
    - <image src="/uploads/bc5e7e000e5046b48cad57dc368a5a65/image.png" width="60%"></image>
    * 온디멘드란?
        - : 설치용으로 사용하겠다는 의미이다.
    * 미국 쪽이 속도가 저렴하다.

#### EC2를 생성하려면 꼭 알아야하는 개념
1. AMI(Amazon Muchine Image)
    - EC2 인스턴슬의 기반이 되는 이미지
    - AMAZON에서 머신들을 관리하기 위해 배포하는 것
    - 이미지란 운영체제를 압축해서 저장해놓은 것
2. 보안그룹
    - 서버에 접근하기 위해 모아놓은 집합
    - 서버 1개에 ip address 1개 할당
    - 1024 port는 우리가 쓸 수 있다.
    - 각 서비스마다 본인들이 어떠한 서비스를 쓰겠다고 할당한 포트번호가 있다,
    - 이러한 것들을 잘 분리하면 잘 사용할 수 있다.
    - 즉, __보안을 위해 ip와 포트 번호를 이용해 정의해두는 서버 접속 규칙__
    - [sg의 inbound, outbound](https://docs.aws.amazon.com/ko_kr/vpc/latest/userguide/VPC_SecurityGroups.html)

    |Inbound | Outbound|
    |--------|---------|
    |외부 사용자가 서버에 접속하기 위한 것|외부 사용자가 서버에 나가기 위한 것|

3. 키페어
    - 서버에 접속하기 위한 열쇠
    - centos/ ubuntu등의 이미지 파일 이용
    - 근데 amazon linux로 로그인하라면 ec2 -user이다.
    - password는 가상서버를 만들때 pw를 생성하는데 이건 key가 필요하다.
    - 이러한 키에 대한 정보가 들어간게 keyfair이다.
    - 육안으로 볼 때는 알 수 없다.
    - key fair파일이 노출된다는 것은 다른 사람의 key를 가지고 접속 가능하다는 것이다.
    - key fair파일 보관은 internet을 끊으면 된다. 
    - 그렇지 못하다면 usb같은 미디어에 넣어두고, 한다.
    - 파일을 특정한 장비에 저장해두고 쓴다.
    - 즉, __key fair방식은 다양한 방법으로 저장할 수 있고, 꼭 잃어버리면 안된다....__
    - 

기타. vpn, 등등


* ![image](/uploads/c45707b2c7309e7f4822c4ea1be22fdc/image.png)
- vpc가 1개로 표시 -> 가상 네트워크가 1개이다.
- key fair 분실시 더이상 데이터를 사용할 수 없다.
* 탄력적 ip
    - ![image](/uploads/b5747a5bc3173e5e8bcba2df638f833e/image.png)
* 볼륨
    - 볼륨 mount
    - 볼륨을 할당받아서 쓴다. 
    - 기본 공간은 8g 바이트
    - ![image](/uploads/6b84966e3ee184a92812e4a7837ddb3e/image.png)
- ![image](/uploads/4835cceea021dbe25ebb030e0022389c/image.png)
    - 근데 root 계정이 권한을 주지 않으면 인스턴스 생성을 못한다.


* 인스턴스 만들기
- ![image](/uploads/cae274174702dadfefd1183e5a89e6b6/image.png)
    1. 2018인거 생성
    2. 다음으로 누르기 micro로
    3. 인스턴스 개수 1개
        - ![image](/uploads/67442dd24dadc455973c9558de1ab9e9/image.png)
    4. ![image](/uploads/dee18c9ee637e7c7e7b670bfb5d6aafe/image.png)
    5. 보안 그룹 -> 중요
    * ipv4
        - 사용자 데이터 수정
* 보안그룹 확인
- ![image](/uploads/07e1ba8f9d7a09cdd3a4beff38fdaf9b/image.png)
    - ![image](/uploads/ea108c9b7152e51995ad885d4eab3745/image.png)
    - 사이다 표현법 
    - ![image](/uploads/02a4b6922f548cc3747ee3686f5e6492/image.png)
    - ![image](/uploads/1c670fe3da165e874a7107a253123778/image.png)
    - ![image](/uploads/cff2008a6f5793fc9a72c5d00e09adc1/image.png)
    -![image](/uploads/73543b49cc0d0ec78029594a15b55c9a/image.png)
    - ![image](/uploads/55a9cc0360a8c21a0278b72c0891f0c0/image.png)

* vi
    - a, i , o -> i는 입력/ a는 명령 

- ![image](/uploads/11e32df1a1f806f4c56cb4684aae407c/image.png)
- ![image](/uploads/432fe47046201da97d035e548257b3e0/image.png)
- ![image](/uploads/95dba9766c5ee7bba21858903a67b7e0/image.png)
- ![image](/uploads/864fb20d945d1e431d314067bce65d89/image.png)
- ![image](/uploads/a1977601fcfcee4ca3a55a63e3b0e2f0/image.png)
- ![image](/uploads/fe8748dfe4a109ae53dc5e57e9c643f6/image.png)
- ![image](/uploads/4902ec88696f9ea993872e791e1b58a5/image.png)




***
#### 20/08/11
#### 

* 포트 죽이는 법
    1. 리눅스
        - ```kill -9 pid```
        - [홈페이지 참고](https://121202.tistory.com/45)

#### simple storage service
* 이미지, 사진파일, 동영상 등을 스토리지 서비스에 올릴 수 있다.
    - byte에 띠리 부과되기 때문에 사이즈를 잘 생각해야한다.
* 아마존 s3
    * 스토리지 클래스    
        - ![image](/uploads/cb72fe4dac216a109c880bbc9ee5c5d5/image.png)
        - 스탠다드 ; 표쥰
        - ia : 한달에 한번
            - infrequency access
        - glacia : 정말 사용 안함
    * 
* __az__
    - 리전 내에 격리된 위치, 개별 데이터 센터
        - 1개의 데이터 센터에는 일반적으로 물리적 서버
    - 물리적으로는 떨어져 있지만 논리적으로 연결
        - 이때 사용되는 개념이 __vpc__ 이다.
    - 1개의 리전당 2개 이상의 az
* 개념
    1. 버킷
    2. 폴더
    3. object
    - 오브젝트는 필요에 따라 폴더(옵션 사항)에 담고 그러한 폴더들을 버킷에 넣는다.
    - ![image](/uploads/55bcf38179254bb266a992f23af949c1/image.png)
    - bucket이름은 dns형식, 즉 unique한 이름으로 정해야한다.


* s3의 장점
    - image, html, mv등등을 자유롭게 올릴 수 있다.
    - html css 등도 가능!
    - 링크를 걸어두면 자동적으로 가능하다.
    - Router 53에 도메인과 링크를 연결시키면 가능하다.
    - 