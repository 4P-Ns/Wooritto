
<img src="https://capsule-render.vercel.app/api?type=waving&color=ed9824&height=300&section=header&text=Wooritto&fontSize=70&fontColor=FFFFFF&animation=fadeIn&width=1200" width="1200" />


## <div align="center" style="font-size: 70px; color: #000080; animation: glow 1.5s infinite;"> Ditto </div>



<br>

## 📍 Contents
- [1️⃣ Overview](#1%EF%B8%8F⃣-overview)
- [2️⃣ Contributors](#2%EF%B8%8F⃣-contributors)
- [3️⃣ Environment Settings](#3%EF%B8%8F⃣-environment-settings)
- [4️⃣ ERD](#4%EF%B8%8F⃣-erd)
- [5️⃣ Trouble Shooting](#5%EF%B8%8F⃣-trouble-shooting)
- [6️⃣ Retrospective](#6%EF%B8%8F⃣-retrospective)


<br>

<br>

## 1️⃣ Overview
이 프로젝트는 ?

### 💡 Background


### ❗ Customer Needs


### 📊 Core Features


</br>


<br>

## 2️⃣ Contributors

|<img src="https://avatars.githubusercontent.com/u/80048007?v=4" width="220" height="200"/>|<img src="https://avatars.githubusercontent.com/u/60309978?v=4" width="220" height="200"/>|<img src="https://avatars.githubusercontent.com/u/193213283?v=4" width="220" height="200"/>|<img src="https://avatars.githubusercontent.com/u/115103394?v=4" width="220" height="200"/>|
|:-:|:-:|:-:|:-:|
|박영진<br/>[@DoomchitYJ](https://github.com/DoomchitYJ)|박정호<br/>[@Jeongho427](https://github.com/Jeongho427)|박진현<br/>[@jinhyunpark929](https://github.com/jinhyunpark929)|이현정<br/>[@nanahj](https://github.com/nanahj)|

<br>

## 3️⃣ Environment Settings

### 🛠 Skills

**Tech Stack**

<div>
<img src="https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white"> 
<img src="https://img.shields.io/badge/linux-FCC624?style=for-the-badge&logo=linux&logoColor=black"> 
<img src="https://img.shields.io/badge/dbeaver-846d5e?style=for-the-badge&logo=dbeaver&logoColor=white"> 
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

<br>

### 🛠 Configuration


<br>

## 4️⃣ ERD

### Elasticsearch


<br>

## 5️⃣ Trouble Shooting

### Window에서 ElasticSearch 접속이 안되는 문제
- 설치 후, ubuntu에서는 curl -X GET 명령어를 통해 잘 되는 것을 확인 했지만 Window에서는 접속이 되지 않는 문제 발생

**해결방안**
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

### kibana와 ElasticSearch가 연동이 안되는 문제
- kibana가 active 상태이지만 ES와 연동이 되지 않아 페이지가 로드되지 않는 문제 발생

**해결방안**
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


### ElasticSearch와 kibana 연동을 위한 네트워크 설정
- ES와 kibana 모두 설정을 맞췄지만 연동이 안되는 문제 발생

**원인**  

- VirtualBox에서 ES와 Kibana가 각각 다른 가상 머신에 설치되어 있는 상황

- NAT 네트워크의 기본 설정에서는 외부에서 VM으로의 직접 접근이 차단되기 때문에, Elasticsearch와 Kibana가 서로 연결되지 않음

**해결방안**

**1. NAT 네트워크 사용 및 포트 포워딩 설정**

- VirtualBox의 NAT 네트워크를 활용하여 두 VM을 묶어 같은 네트워크 내에서 통신할 수 있도록 설정
- 외부와의 연결이 필요하기 때문에, 포트 포워딩을 설정하여 Elasticsearch와 Kibana의 서비스 포트를 각각 호스트에 노출

**2. Kibana 설정 변경**

- kibana.yml 파일에서 Elasticsearch의 주소를 가리키는 elasticsearch.hosts을 포트 포워딩에 맞게 수정
- localhost -> elasticearch가 설치된 가성머신의 ip 주소

<img src="https://github.com/user-attachments/assets/27d4facf-50ba-4a9b-aff9-8415ea5591ab" alt="image" width="600">

## 6️⃣ Retrospective



<img src="https://capsule-render.vercel.app/api?type=waving&color=ed9824&height=150&section=footer" width="1000" />
