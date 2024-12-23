# 🎲 그림이 소설이 되는, Next Novel

![logo](docs/img/logo.png)
## ⌛️ 프로젝트 진행 기간
2024.11.19(화) ~ 2024.12.27(금) <br>


## ✨ Koimang 서비스 개요
### 기획 배경
- AI 생성형 모델을 활용한 서비스 개발
- 이 프로젝트는 웹소설 작가를 꿈꾸는 초보 작가들을 위한 서비스입니다.

## 🏃 Koimang 의 이용 목적
- 자신만의 웹소설 표지를 손쉽게 만들 수 있는 도구를 제공합니다.
- AI의 상상력을 빌려 소설 집필 중 막힌 부분을 해소할 수 있습니다.
- 소설의 내용을 바탕으로 제목을 생성할 수 있습니다.
- 소설가들에게 데이터 기반의 트렌드 분석 및 생성 AI 도구를 이용한 효율적인 창작 환경 제공합니다.

## 🌞 팀원 소개
### 코리아IT의 망나니가 되었다

- 문정현 - 팀장, 데이터 분석, AI 모델링
- 최윤범 - AI 모델링, 모델 Backend
- 화철수 - Frontend, Backend, 배포

## ✔️ 아키텍처 구성도
![architecture](docs/img/architecture.png)

## ✔️ 주요 기능
### 1) 내가 원하는 상황을 바탕으로 소설 작성
- 원하는 장르(로맨스, 판타지, 무협, 로맨스 판타지, 현대 판타지)를 선택
- 원하는 장면을 입력하면 상황에 맞게 한 문단 분량의 소설 작성
- KoGPT2 를 파인튜닝하여 구현

### 2) 작성한 소설의 내용을 바탕으로 제목 생성
- 작성 완료된 소설(3000자 이상)의 txt 파일을 업로드하면 제목 생성
- Llama3 를 파인튜닝하여 구현

### 3) 소설 표지 생성
- 원하는 인물을 묘사하여 입력(검은 정장의 남자와 드레스를 입은 여자)
- 생성된 그림을 웹소설의 표지로 사용
- Stable Diffusion 을 파인튜닝하여 구현

### 4) 웹소설 트렌드 분석
- 다른 사용자가 제작한 소설을 열람하고, 한줄평 작성 가능
- 소설의 제목 혹은 소설 작성자를 기반으로 keyword 검색 가능
- 장르별 정렬로 자신이 관심있는 분야의 소설 확인 가능

### 5) MZ스러운 디자인과 친절한 이용 가이드
- GSAP 애니메이션 효과와 주황빛 컬러
- 사용자를 위한 이용가이드 페이지 제공
  ![sample_guideline.png](/docs/img/sample_guideline.png)

## ✔️ 주요 기술
### 1) KoGPT2 소설 단락 생성
- Text-to-Text 생성 모델
- KoGPT2 를 Full-Finetuning 하여 장르와 상황에 맞게 소설의 단락을 생성합니다.

### 2) Llama3 소설 제목 생성
- Text-to-Text 생성 모델
- QLoRA(양자화)기법을 활용하여 LLM(거대 언어 모델) Finetuning하여 사용자가 업로드한 소설의 내용을 바탕으로 제목을 생성합니다.

### 3) Stable Diffusion
- Text-to-Image 생성 모델
- LoRA 기법을 활용하여 Finetuning 하여 사용자가 입력한 내용을 바탕으로 그림을 생성합니다.


## ✔️ 협업 툴
- Git
- Notion

## ✔️ 협업 환경
- Git
    - 코드의 버전 관리
    - 개발 이슈 관리 및 해결을 위한 회의
    - MR과 팀원의 코드리뷰
- Notion
    - 기획 단계에서 도출된 아이디어 정리
    - 회의록과 팀미팅을 기록하여 의견과 해결사항을 정리
    - 팀 그라운드 룰을 정리


## ✔️ 프로젝트 산출물
- [기능 명세서](https://chipped-cart-851.notion.site/a96e0e004e4c4f39bab65fa821f4825f?v=f77e4329cc5e4b4fbb3a73894ba13c8c)
- [API 명세서](https://chipped-cart-851.notion.site/838d5959ec264671ac3dc8410c0983fa?v=56e9cb334ec14ee4a3634693dba9cced)
- [와이어 프레임](docs/img/wireframe.png)

## ✔️ 프로젝트 결과물
- [최종 발표 자료](docs/서울_5반_A502_최종발표자료.pptx)


## 🎲 Next Novel 서비스 화면
### 랜딩
![img](gif/홈페이지.gif)
### 로그인
![img](gif/로그인_로그아웃.gif)
### 표지생성
![img](gif/표지생성.gif)
### 제목생성오류
![img](gif/제목생성오류.gif)
### 제목생성
![img](gif/제목생성.gif)
### 단락생성
![img](gif/단락생성.gif)
### 화면넘기기
![img](gif/화면넘기기.gif)

<hr>