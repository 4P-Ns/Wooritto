
<img src="https://capsule-render.vercel.app/api?type=waving&color=ed9824&height=300&section=header&text=Wooritto&fontSize=70&fontColor=FFFFFF&animation=fadeIn&width=1200" width="1200" />


## <div align="center" style="font-size: 70px; color: #000080; animation: glow 1.5s infinite;">💳 우리도 쓸 때는 쓴다 😎</div>

<div align="center">
  <img src="https://github.com/user-attachments/assets/911b4b16-f2cc-423a-995a-00493e2206be" width="60%">
</div>


<br>

## 📍 Contents
- [1️⃣ Contributors](#1%EF%B8%8F⃣-overview)
- [2️⃣ Overview](#2%EF%B8%8F⃣-contributors)
- [3️⃣ Insight](#3%EF%B8%8F⃣-insight)
- [4️⃣ New Strategy](#4%EF%B8%8F⃣-new-strategy)
- [5️⃣ Environment Settings](#5%EF%B8%8F⃣-environment-settings)
- [6️⃣ Trouble Shooting](#6%EF%B8%8F%E2%83%A3-trouble-shooting)
- [7️⃣ Retrospective](#7%EF%B8%8F%E2%83%A3-retrospective)

<br>
<br>

## 1️⃣ Contributors
<br>

|<img src="https://avatars.githubusercontent.com/u/80048007?v=4" width="220" height="200"/>|<img src="https://avatars.githubusercontent.com/u/60309978?v=4" width="220" height="200"/>|<img src="https://avatars.githubusercontent.com/u/193213283?v=4" width="220" height="200"/>|<img src="https://avatars.githubusercontent.com/u/115103394?v=4" width="220" height="200"/>|
|:-:|:-:|:-:|:-:|
|박영진<br/>[@DoomchitYJ](https://github.com/DoomchitYJ)|박정호<br/>[@Jeongho427](https://github.com/Jeongho427)|박진현<br/>[@jinhyunpark929](https://github.com/jinhyunpark929)|이현정<br/>[@nanahj](https://github.com/nanahj)|

<br>

## 2️⃣ Overview

<br> 

이 프로젝트는 **실제 카드 데이터**를 기반으로 VVIP/VIP의 카드 사용 내역을 분석하여 하위 등급 회원들의 **카드 사용을 촉진**시키기 위한 전략 수립 및 데이터 분석 프로젝트이다.

최근 소비 트렌드로 주목받은 **Ditto 소비**를 모티브로, VVIP/VIP의 선호 소비 분야에 맞추어 해당 분야에 특별 혜택을 제공한다.

본 프로젝트는 **Elasticsearch**와 **Kibana**를 활용하여 **대규모 카드 데이터를 분석하고, 시각화 및 인사이트 도출**에 중점을 두었다.

<br>

### 💡 Background<br>

<br>

**Ditto소비란?**

> 우리는 평소에 관심 있던 연예인의 착장, 나와 *추구미가 같은 인플루언서의 광고 등의 영향을 받아 제품을 구매한다. 이번 주제기획에서는 2024 소비 트렌드로 선정된 ‘디토 소비(Ditto Consumption)’에 대해 다루며 사회를 이해하고, 현명한 소비자로 나아가고자 한다.
>
> 출처 : 홍대신문([http://hiupress.hongik.ac.kr](https://hiupress.hongik.ac.kr/news/articleView.html?idxno=10826))
> 

> 많은 수고를 들이지 않고서도 좋은 결과를 갖고 싶은 마음에 나를 대신해 구매 의사결정을 내려줄 사람, 콘텐츠, 커머스를 추종하는 방식을 택한 것이다.  
출처 : Ditto 소비의 핵심 - 추종을 통한 제품 구매(https://magazine.cheil.com/55182)
>

<br>

## 3️⃣ Insights

<br>

### ✏️ 가설1. VVIP/VIP 회원의 비율이 전체의 약 10%를 차지할 것이다.
<img src="https://github.com/user-attachments/assets/c6c01e6a-09fc-4633-a5b1-86f402a11abf" width="400">

> VVIP는 표본 전체의 1.31%, VIP는 5.13%로 약 6.44%를 차지하였다.

<br>

### ✏️ 가설2. VVIP/VIP 회원이 사용한 총 금액이 전체의 50%를 차지할 것이다.
<img src="https://github.com/user-attachments/assets/a2f2db66-6ce4-4551-ba2c-16c209e4e14b" width="400">

> VVIP는 3.95%, VIP는 12.41%로 전체의 약 16%를 차지하였다.
> 가설에 비해 VVIP/VIP가 차지하는 금액이 크지 않았다. 

<br>

### ✏️ 가설3. VVIP/VIP 회원은 ‘외식’에 소비를 많이 할 것이다.
<img src="https://github.com/user-attachments/assets/c878ff24-9b89-4c09-aa4a-ea6fe6553eac" width="700">

> 소비금액이 다른 등급 회원들과 유의미하게 차이가 나지 않았다.

<br>

### ✏️ 가설4. VVIP/VIP 회원은 레저/취미생활에 소비를 많이 할 것이다.
<img src="https://github.com/user-attachments/assets/1f7b15f5-418b-4525-b099-a7bc2954ad87" alt="문화" width="600">

<img src="https://github.com/user-attachments/assets/edaeedd7-7fdb-4a81-895f-b7e098c8ee2f" alt="레저" width="600">

> VVIP/VIP회원이 문화생활/레저업소에 소비한 평균 금액이 타 회원에 비해 약 3배 높았다.

<br>

### 📝 추가사항

<img src="https://github.com/user-attachments/assets/70c056fe-ae13-4da7-8cdc-62f1081b389f" alt="결제분야" width="600">

> 주요 소비 분야 몇 가지를 뽑아보았다. 팀원끼리 직관적으로 가설을 세웠던 분야를 제외하고, 서적/문구에서 멤버 등급별 유의미한 차이를 보였다.

<br>

<img src="https://github.com/user-attachments/assets/61de8aa8-69df-49f9-9e6e-6cd983ea15b5" alt="도서" width="600">

> 서적/문구에서 VVIP와 ‘해당없음’ 등급 고객들의 차이는 약 9.71배 차이가 났다.

<br>

## 4️⃣ New Strategy

### 📚 결론

<p align="center">
  <img width="100%" src="https://github.com/user-attachments/assets/7c2f64ef-a372-447b-8ea9-16a38d0a1c30" alt="CARD_BANNER">
</p>

<br>

#### 우리도 쓸 때는 쓴다, 'WOORITTO'

이 카드는 고객의 라이프스타일 전반을 **프리미엄화**하는 것을 목표로 설계되었습니다. 

**독서**와 **문화 활동**을 중심으로 **지적 성장**을 도모하며, 다양한 **마일리지 적립과 할인 혜택**을 통해 **자기계발의 동기**를 부여합니다.

테마파크, 스포츠 시설, 공연장 등의 **여가 시설 이용 혜택**으로 균형 잡힌 라이프스타일을 지원하고, 온/오프라인 쇼핑 전반에 걸친 혜택으로 **스마트한 소비 생활을 장려**합니다.

특히 실적 달성 회원을 위한 프리미엄 서비스를 통해 고객의 지속적인 성장과 특별한 경험을 제공합니다.

<br>

### 💳 카드 기본 서비스 - 프리미엄 라이프스타일로의 첫걸음

**📚 Book & Culture - 독서와 문화생활의 시작**  
- 전국 오프라인 서점/문구점 이용금액 1% 마일리지 적립 서비스 - **[오프라인 독서 문화 체험]**
- 온라인 서점/문구점 결제금액 0.5% 마일리지 적립 - **[디지털 시대의 독서 습관]**
- 월간 도서 구매금액 30만원 이상 시 추가 5,000 마일리지 적립 - **[독서량에 따른 보상]**
- [신규] 전자책 구독 서비스 20% 할인 + 구독료의 3% 마일리지 적립 - **[디지털 전환 촉진]**
- 적립된 마일리지로 도서 구매 시 추가 5% 할인 - **[독서 순환 생태계 조성]**
  
**🎡 Leisure & Entertainment - 여가생활의 품격 상승**
- 제휴 테마파크 연간이용권 구매 시 무료이용권 2매 제공 - **[프리미엄 레저 문화 체험]**
- 스포츠 시설 이용금액 5% 청구할인 (골프장, 스키장, 스케이트장, 볼링장, 수영장) - **[고급 스포츠 입문 지원]**
- [신규] 제휴 공연장 예매 시 10% 할인 - **[문화생활 진입장벽 낮추기]**
- 마일리지로 레저 시설 이용권 구매 시 20% 추가 할인 - **[여가활동 순환 촉진]**

**🛍️ Shopping & Commerce - 스마트한 소비생활 설계**
- 국내 오프라인 가맹점 1% 청구할인 - **[기본적인 소비 혜택]**
- 간편결제 시 2% 청구할인 + 1% 마일리지 적립 - **[디지털 결제 전환 유도]**
- [신규] 프리미엄 온라인몰 3% 추가 할인 - **[고급 소비로의 진입]**
- 마일리지 사용 시 온라인몰 5% 추가 할인 - **[소비 순환 극대화]**

<br>

### 💳 실적 달성 회원 전용 프리미엄 서비스 - 프리미엄 라이프스타일의 완성
  
**📚 Book & Culture - 지적 성장의 특별한 경험**  

- 분기별 프리미엄 북콘서트 초청 (오프라인 도서 구매 실적 보유 고객 한정) - **[문화적 소속감 제공]**
- VIP/VVIP 고객 도서 큐레이션 서비스 + 분기별 인기 도서 5종 20% 특별 할인 - **[프리미엄 독서 경험]**
- [신규] 프리미엄 독서모임 멤버십 무료 가입 + 참여 시 마일리지 2배 적립 - **[독서 커뮤니티 형성]**

**🎡 Leisure & Entertainment - 특별한 여가생활의 완성**  
- 제휴 리조트 객실 무료 업그레이드 서비스 - **[프리미엄 휴식 경험]**
- 연 2회 마일리지 5배 적립 이벤트 참여 기회 - **[혜택의 집중]**
- [신규] 프라이빗 골프 레슨 50% 할인 + 레슨비 3% 마일리지 적립 - **[고급 스포츠 생활화]**
  

<br>


## 4️⃣ Environment Settings

### 🛠 Skills

**Tech Stack**

<div>
<img src="https://img.shields.io/badge/linux-FCC624?style=for-the-badge&logo=linux&logoColor=black"> 
<img src="https://img.shields.io/badge/elasticsearch-3db9ac?style=for-the-badge&logo=elasticsearch&logoColor=white"> 
<img src="https://img.shields.io/badge/kibana-f04e98?style=for-the-badge&logo=kibana&logoColor=white">   
</div>

<br>

**Co-work Stack**

<div>
<img src="https://img.shields.io/badge/notion-000000?style=for-the-badge&logo=notion&logoColor=white"> 
<img src="https://img.shields.io/badge/github-303a50?style=for-the-badge&logo=github&logoColor=white">
<img src="https://img.shields.io/badge/slack-e01e5a?style=for-the-badge&logo=slack&logoColor=white">
</div>

<br>

### 🖥️ Architecture

<img src="https://github.com/user-attachments/assets/d76d01f2-45c8-4cb0-b4e0-04f875ac5b91" width="70%">

<br>

### 🛠 Configuration

---

### Virtual Machine에서 ELK를 설치할 각각의 서버 생성

<details>
<summary>각 서버에서 SSH 가능하게 설정</summary>

<img src="https://github.com/user-attachments/assets/700959c1-7bf6-40dc-8350-fb6c25756db1" width="60%">


<img src="https://github.com/user-attachments/assets/b9a455da-1731-4d9d-bb5d-aac56f4b82f2" width="60%">


- 기본 메모리 용량 늘려주기

- ELK를 모두 실행하면 10GB가 조금 넘는 용량이 필요하다. 이 때문에 서버를 각각 둔 것

- 각각 4GB정도로 설정

<img src="https://github.com/user-attachments/assets/8caa04a7-dcc4-4705-951e-9867e75704d6" width="60%">


- ssh 설치

```bash

sudo apt update

# openssh 설치시 y옵션 자동 적용하면서 설치하는 명령어
sudo apt install openssh-server -y

sudo systemctl status ssh
```

  
</details>

<details>
  <summary>SSH 접속 확인</summary>

- 로컬 머신에서 SSH를 테스트하려면 자신의 IP 주소를 확인

```bash
ip addr
```
  
</details>

<details>
  <summary>SSH 서버 설정 변경 (옵션)</summary>

- SSH 설정 파일 :  `/etc/ssh/sshd_config`에 있습니다.
- 필요 시 설정 파일을 편집

```bash
sudo nano /etc/ssh/sshd_config
```

```
# 기본 포트 변경
Port 22

# 루트 로그인 허용/비허용
PermitRootLogin no

```
설정을 변경한 후 SSH 서비스 재시작

</details>




### VirtualBox에서 서버들 같은 네트워크로 묶어주기

<img src="https://github.com/user-attachments/assets/011013d3-bb1a-40a5-b4e7-130a84da96f0" width="60%">


- NAT 네트워크 설정

<br>

<img src="https://github.com/user-attachments/assets/16f35fbb-c193-4a16-95a9-bd4e533be27e" width="60%">



- 서버 각각 포트포워딩 해주기

<br>

<img src="https://github.com/user-attachments/assets/5b623e03-6580-4b66-b7f3-c6c892846312" width="60%">

<br>

### Ubuntu에 ElasticSearch 설치하기

```bash
# Elasticsearch 7 버전 설치
wget -qO - https://artifacts.elastic.co/GPG-KEY-elasticsearch | sudo apt-key add -
sudo apt-add-repository "deb https://artifacts.elastic.co/packages/7.x/apt stable main"

# Elasticsearch 설치
sudo apt update
sudo apt install elasticsearch

# 시작
sudo systemctl start elasticsearch

# 상태 확인
sudo systemctl status elasticsearch

## 자동실행 설정(선택사항)
$ sudo systemctl enable elasticsearch
```

<br>

- elasticsearch.yml 파일 수정하기

```bash
# elasticsearch.yml 파일 vim으로 열기
sudo vi /etc/elasticsearch/elasticsearch.yml

# yml 파일 수정
network.host = 0.0.0.0
http.port: 9200

# 실제로는 클러스터에 참여할 다른 노드의 IP만을 기입해야 함.
discovery.seed_hosts: ["0.0.0.0"]

```

<img src="https://github.com/user-attachments/assets/7826b525-4f43-47b5-b2cb-d291aed6f427" width="60%">

<br>

<br>

- ES 재실행

```bash
# ES 재실행
sudo systemctl restart elasticsearch
```

<br>

- 포트 개방 후 window에서 접속 시도

<img src="https://github.com/user-attachments/assets/d61177da-39d6-4572-a513-49b5ddadb33f" width="60%">

<img src="https://github.com/user-attachments/assets/b5f419f6-e1b8-4a45-b9ae-ccaa5b986417" width="60%">

<br>

### Ubuntu에 Kibana 설치

- 서버 세팅 작업은 위와 동일
- 세팅 후 mobaxterm으로 접속

```bash
# kibana 설치
sudo apt update
sudo apt install kibana

# 시작
sudo systemctl start kibana

# 상태 확인
sudo systemctl status kibana

## 자동실행 설정(선택사항)
$ sudo systemctl enable kibana
```

<br>

- ES와 연동을 위한 kibana.yml 수정

```bash
$ sudo vi /etc/kibana/kibana.yml

# kibana.yml 주석 해제
server.port: 5601

# server.host: localhost 에서 변경
server.host: 0.0.0.0

# elasticsearch와 연결
elasticsearch.hosts: ["http://localhost:9200"]
```

<br>

- 현재 다른 서버에 설치된 ES와 연동을 해야 하기 때문에 위의 elasticsearch.hosts의 ip를 elasticsearch가 있는 서버 ip로 해줘야 함

<img src="https://github.com/user-attachments/assets/87ea59f9-9522-4f2f-92e6-12fc89b79b4a" width="60%">

<img src="https://github.com/user-attachments/assets/d1fd3aa3-f033-4bd2-9996-491e3b4afc6c">

<br>

<br>

- kibana 접속 확인

```bash
# 재시작
sudo systemctl restart kibana

# 상태 확인
sudo systemctl status kibana
```

<br>

- window에서 kibana 접속

<img src="https://github.com/user-attachments/assets/5c470607-88a7-4fef-b00e-ab588177d5b2" width="60%">


<br>


## 5️⃣ Trouble Shooting

### ⚔️ Window에서 ElasticSearch 접속이 안되는 문제
- 설치 후, ubuntu에서는 curl -X GET 명령어를 통해 잘 되는 것을 확인 했지만 Window에서는 접속이 되지 않는 문제 발생

<br>

**👌 해결방안**
- elasticsearch.yml에서 포트와 host ip를 설정

```bash

# elasticsearch.yml 파일 vim으로 열기
sudo vi /etc/elasticsearch/elasticsearch.yml

# yml 파일 수정
network.host = 0.0.0.0
http.port: 9200

# 실제로는 클러스터에 참여할 다른 노드의 IP만을 기입해야 함.
discovery.seed_hosts: ["0.0.0.0"]
  
```

<img src="https://github.com/user-attachments/assets/8b629d71-4f8f-45b1-bba1-630402431f45" alt="image" width="600">

<br>

### ⚔️ kibana와 ElasticSearch가 연동이 안되는 문제
- kibana가 active 상태이지만 ES와 연동이 되지 않아 페이지가 로드되지 않는 문제 발생

<br>

**👌 해결방안**
- kibana.yml에서 server의 host와 port 설정 및 elasticsearch와 연결

```bash

# kibana.yml 파일 vim으로 열기
$ sudo vi /etc/kibana/kibana.yml

# kibana.yml 주석 해제
server.port: 5601

# server.host: localhost 에서 변경
server.host: 0.0.0.0

# elasticsearch와 연결
elasticsearch.hosts: ["http://localhost:9200"]

```

<img src="https://github.com/user-attachments/assets/9aa2d4f8-8a50-4f07-a621-a018a471a77a" alt="image" width="600"> <img src="https://github.com/user-attachments/assets/ddb88ca5-54e0-46ed-b4ca-ad4e7b143bec" alt="image" width="600">


### ⚔️ ElasticSearch와 kibana 연동을 위한 네트워크 설정
- ES와 kibana 모두 설정을 맞췄지만 연동이 안되는 문제 발생

<br>

**😭 원인**  

- VirtualBox에서 ES와 Kibana가 각각 다른 가상 머신에 설치되어 있는 상황

- NAT 네트워크의 기본 설정에서는 외부에서 VM으로의 직접 접근이 차단되기 때문에, Elasticsearch와 Kibana가 서로 연결되지 않음

<br>

**👌 해결방안**

**1. NAT 네트워크 사용 및 포트 포워딩 설정**

- VirtualBox의 NAT 네트워크를 활용하여 두 VM을 묶어 같은 네트워크 내에서 통신할 수 있도록 설정
- 외부와의 연결이 필요하기 때문에, 포트 포워딩을 설정하여 Elasticsearch와 Kibana의 서비스 포트를 각각 호스트에 노출

**2. Kibana 설정 변경**

- kibana.yml 파일에서 Elasticsearch의 주소를 가리키는 elasticsearch.hosts을 포트 포워딩에 맞게 수정
- localhost -> elasticearch가 설치된 가성머신의 ip 주소

<img src="https://github.com/user-attachments/assets/27d4facf-50ba-4a9b-aff9-8415ea5591ab" alt="image" width="600">

## 6️⃣ Retrospective



<img src="https://capsule-render.vercel.app/api?type=waving&color=ed9824&height=150&section=footer" width="1000" />
