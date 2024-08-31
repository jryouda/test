# **🏃 OpenRun** 

**당신 만의 캐릭터, 함께 달리는 즐거움!**
<p align="center">
<img src="https://github.com/user-attachments/assets/e96fa83f-a005-4ff9-96c3-67cd9c71e8d2">
</p>
<br>

# 프로젝트 소개

언제든지 다양한 사람들과 달리기 모임에 참여하고, NFT 아바타를 획득하여 나만의 개성을 표현할 수 있는 

커뮤니티 기반 **'함께 뛰는 M2E' dApp** 입니다.

- Open + Run, 러닝을 여는 서비스입니다. 러닝 모임(벙)을 열고, 함께 달릴 사람들을 모아, 함께 달릴 수 있습니다.
- 사용자들이 러닝을 즐기기만 하면, NFT 아바타라는 보상을 제공합니다.
- 사용자들은 서비스 내 다양한 활동(도전 과제)으로 NFT 아바타 파츠를 얻을 수 있고, 이를 조합해 나만의 아바타를 꾸밀 수 있습니다.
- 블록체인에 대한 기초 지식이나 NFT 구매 없이, 낮은 진입 장벽으로 NFT에 다가갈 수 있습니다.

# 팀 소개
## Backend
Yejin Kelly Joo [@yjkellyjoo](https://github.com/yjkellyjoo)

Son Jun Hyung [@sonjh919](https://github.com/sonjh919)

Yoo Jae Rin [@jryouda](https://github.com/jryouda)

Kim Dong Hwan [@Dunn-Kim](https://github.com/Dunn-Kim)

## Frontend
Jeong SeungRyong [@windragon0807](https://github.com/windragon0807)

JungDae Choi [@VEA22](https://github.com/VEA22)
## Design
Younsoo Kim

Hayul Jeong [@mechakawai](https://github.com/mechakawai)

# 기술 스택

## Frontend

TypeScript

Next.js

## Backend

JAVA

Spring Boot

MySQL

xrpl4j

# 프로젝트 구조

```
openrun
├── frontend
│   ├── public
│   ├── src
...
├── backend
│   ├── src
...

```

# 실행 방법

## Frontend
bash 

cd frontend

npm install

npm run dev
...


## Backend

cd backend

./gradlew bootRun

...

혹은 배포 URL에서 확인 가능

frontend: https://open-run.vercel.app/

backend API swagger: https://open-run.xyz/swagger-ui/index.html

# 페이지별 기능(데모 버전)

### [초기 화면]

- 데모 초기 화면으로, 벙 만들기 동작을 실행 할 수 있습니다.
- 사용자의 NFT 아바타를 보여줍니다.

| 초기 화면 |
|----------|
|![splash](https://github.com/user-attachments/assets/4fb32841-4b33-4c9d-893d-45a4ae9a1212)|

### [벙 만들기]

- 벙 만들기 버튼 클릭 시 나오는 화면으로, 빈 칸 내용을 입력하여 DataBase에 저장합니다.
    - 벙 이름, 장소, 시작 일시, 거리, 페이스 등을 입력 받습니다
- 벙 만들기 완료 시, 초기 화면으로 이동합니다.

| 벙 만들기 |
|----------|
|![splash](https://github.com/user-attachments/assets/37114465-b887-4473-beb2-27a52a61ae67)|

### [생성된 벙 확인하기]

- 다시 데모 초기화면으로 돌아오며, 생성된 벙을 확인할 수 있습니다.
- 생성된 벙을 클릭하여 상세 정보를 확인할 수 있습니다.

| 생성된 벙 확인하기 |
|----------|
|![splash](https://github.com/user-attachments/assets/2b87828c-a880-4066-ab89-c1683d2a9d00)|

### [벙 상세정보 화면]

- 벙 상세정보를 표시하기 위한 화면으로, 장소, 시작 시간, 거리, 페이스 등을 확인할 수 있습니다.
  - 현재 참여자는 더미 데이터 입니다.
- 주소를 지도로 표출하여 보여줍니다.
- 벙 참여완료 버튼 클릭 시, 도전 과제 완료합니다.

| 벙 상세정보 화면 |
|----------|
|![splash](https://github.com/user-attachments/assets/851cdba8-cb57-43bd-b34c-42d6b45c53ee)|

### [발급된 NFT 아바타]

- 도전 과제 완료 시, 발급된 NFT 아바타를 표출하는 화면입니다. 
- xrpl 자바 라이브러리를 활용하여 NFT 민팅 후 발급된 NFT 정보를 가져와 표출합니다.
  - category 값(총 9가지 enum 값으로 정의되어 있음 -taxon 정보), serial number(본인의 nft임을 확인하기 위한 정보), memodata(common, rare, hidden 에 대한 아바타 정보)

| 벙 상세정보 화면 |
|----------|
|![splash](https://github.com/user-attachments/assets/a44a4966-9658-42d9-8c76-04645fd26dd8)|

