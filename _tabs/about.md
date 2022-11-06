---
# the default layout is 'page'
icon: fas fa-info-circle
order: 4
toc: true
---

## 🧑🏻‍💻 권기남 (Kwon, Ginam)

---

> 10살 때부터 컴퓨터를 너무 좋아해서 개발자 외에는 다른직업은 생각하지 않았습니다. 인생의 절반 이상을 개발자 목표 하나 만을 바라 봤습니다.  
새로운 기술과 필요성에 맞게 커스터마이징 하여 피드백을 받는 것을 좋아하는 백엔드 개발자 권기남 입니다.  
동료들과의 협업은 물론 비효율적인 업무 프로세스를 개선하고, 일정 관리와 관련한 목표를 달성하는 것을 좋아합니다.  
성공은 남이 가져다주지 않듯이 개발자로 성공을 위해 제 자신의 믿음과 노력을 바탕으로 큰 개발자가 되겠습니다.  
> 

## 🛠  Stacks

---

### Back-End

- NodeJS, ExpressJS, TypeScript,JavaScript(ES6, ES7), NestJS,
- C++, Python
- passportJS, bcryptJS, express-async-handler, jsonwebtoken, gravatar, mongoose, multer
- Swagger, Postman
- Docker

### Infra

- OpenStack
- AWS EC2, AWS Beanstalk, AWS CodePipeline, AWS Lambda, AWS CodeCommit
- Bash script
- K8s

### DataBase

- MySQL
- MongoDB
- AWS RDB

## 🎈  Experiences

---

### [**㈜** 케이투시스템즈](http://k2systems.kr/)

IT인프라팀 인턴, 2022.03.02 ~ 2022.06.30

- CentOS7 자동 설치 및 설정
    - 기존 방식 문제점: Raid 1 이용 디스크를 복제하여 새로운 운영체제 설치 서버당 약 3시간 소요
    - 사용기술: Kickstart
    - 맡은 내용
        >Partition 및 기본 설정 선택 할 필요 없이 자동으로 설정  
        kickstart 파일 및 패키지 추가한 Custom iso 생성  
        설치후 자동으로 설정 스크립트 실행  
        Kickstart 메뉴얼 작성  
        >
    - 효과: 운영체제 설치 시간이 3시간에서 40분으로 단축
- 문서 작성 자동화 프로그램
    - 기존 방식 문제점: 보안 점검 스크립트의 결과 약 4000 라인. 따라서 문서화에 걸리는 시간이 서버 당 2시간 소요
    - 사용기술: Python, openpyxl
    - 구현 방법
        >결과 값을 저장할 템플릿 문서 제작  
        각 점검 항목에 따라 결과 값 파싱  
        템플릿 문서에 지정된 셀에 결과값 저장  
        >
    - 효과: 서버 하나당 문서작성 소요 시간 2시간에서 3초 미만으로 개선
- 서버 보안 점검 및 취약점 개선 스크립트
    - 필요한 이유: 서버의 보안 점검와 취약점 개선을 모두 수행하는 스크립트가 존재하지 않았다.
    - 사용 기술: Bash script
    - 구현 방법
        >설정 파일의 Key Value 분리  
        해당 설정 내용의 Value 수정  
        Key 존재 유무 판단 후 설정 내용 추가  
        >

---

### [전북대학교 운영체제 연구실](https://oslab.jbnu.ac.kr)

학부연구생, 2021.09.01 ~ 현재

- 학내 클라우드 서비스 JCloud(Openstack Xena) 구축 및 운영
    - [인스턴스들을 스냅샷 하는 배시 스크립트](https://github.com/ginami0129/jcloud/tree/main/backupService)
        - OpenStack에 여러 인스턴스를 한번에 스냅샷하는 기능이 존재 하지 않는 문제 해결
        - 트래픽을 사용하지 않은 시간대에 자동으로 실행하도록한다.
    - 학생들이 서로의 인스턴스를 조작할 수 있는 문제 해결
        - Nova 코드 수정을 통해 User_id 기반 정책 적용
            - https://github.com/openstack/nova/pull/100/commits/a921ceb7a9e3d0c059ed709d56082031bc95d8ac
        - 2022 한국컴퓨터종합학술대회 논문투고
            - [오픈스택 기반 교육용 클라우드 컴퓨팅 시스템의 권한 모델에 관한 연구](https://www.dbpia.co.kr/journal/articleDetail?nodeId=NODE11120535)
                

## 💻  Projects

---

### 📋 [BLOG API](https://github.com/ginami0129/blog_nestjs) (2022.05 ~ 진행중)

- 한줄 소개 : 블로그를 구현한 Back-end API 개발
- 사용 기술 :  NestJS, TypeScript, MySQL, Git, Swagger UI, TypeORM
- **개발 부분**

>
포스트 기본 CRUD 구현

>

- **TODO LIST**

>
댓글 , 소셜 로그인, email comfirmation
OAuth 구현
API protection 기능 구현
Swagge UI로 API 문서 자동작성
Passport로 유저 인증
AWS 배포
Docker 개발 환경 구축
Micro Service Architecture

>

---

### 📋 [E-Commerce API](https://github.com/ginami0129/Shopping-mall-api) (2022.03 ~ 2020.04)

- 한줄 소개 : 쇼핑몰 Back-end API 개발
- 사용 기술 : Express.js, Node.js, MongoDB, Git, Swagger UI
- **개발 부분**

>
회원가입, 로그인, 주문 저장 및 조회 API 구현  
상품 목록 조회 시 Pagenation 기능 구현  
API protection 기능 구현  
Swagge UI로 API 문서 작성  
JWT로 유저 인증  
AWS Beanstalk 이용 배포   
AWS Codepipeline 사용 배포 자동화  

>

- **TODO LIST**

>
OAuth 구현
Docker 개발 환경 구축
Passport로 유저 인증
Micro Service Architecture

>

---

### 📋 [호버링 터치](https://github.com/ginami0129/HoveringTouch) 기능 탑재 [키오스크](https://github.com/ginami0129/KioskWithHoveringTouch) (2021.10 ~ 2021.10)

- 손가락의 움직임을 이용한 비 접촉 방식 키오스크
- Back-end API 개발 , 손 동작 인식 및 마우스 조작 기능 구현(google Mediapipe)
- Python, JavaScript, Express.js, React.js, MongoDB, google Mediapipe, PyAutoGUI
- 제 7회 전북권 온라인 아이디어 해커톤 대회 참가 및 대상 수상
- **개발 부분**

>
키오스크 관리자 API 구현(Express.js, MongoDB)  
주문 목록, 주문 상태 보기, 주문 상태 변경 기능 구현  
손가락의 좌표 변화 값 이용 제스처 인식 구현(Google MediaPipe)  
손가락의 움직임과 마우스 움직임 매핑(Python)  

>

- [발표 영상](https://www.youtube.com/watch?v=kkXp_c6Zthc)

---

### 📋 [Joasis](https://github.com/ginami0129/Joasis) (2021.07 ~ 2022.02)

- 학교 공지사항 키워드 알림 및 기숙사 식단 확인 앱  
- React Native, JavaScript, AWS Lambda, Firebase, Serverless, CheerioJS  
- **개발 부분**  

>
학교 공지사항 및 기숙사 식단 데이터 수집 (데이터 크롤링)  
AWS Lambda(Serverless), AWS Codecommit, Codepipeline 이용  CI/CD 구성  
FCM 이용 푸시 Notification 구현  

>

- [발표 영상](https://www.youtube.com/watch?v=4hP23OKuTds)

---

### 📋 [너 측정 문제있어?](https://github.com/osamhack2020/WEB_WebbasedAutomatedMeasurementService_Doyouhaveameasurementproblem) (2020.10 ~ 2020.11)

- 웹 기반 측정 자동화 서비스
- JavaScript, Node.js, Express.js, React.js, linux-gpib
- 2020 군장병 공개SW 온라인 해커톤 참가작
- [**개발 부분**](https://github.com/osamhack2020/WEB_WebbasedAutomatedMeasurementService_Doyouhaveameasurementproblem/commits?author=ginami0129&before=0d463e55ae4459087b7066b62c5cf9e03d86e43f+35)

>
linux-gpib 이용 측정 장비와 연결 이슈 해결 및 메뉴얼 작성  
Enter 누르면 전송 또는 로그인 하게 구현  
채팅 수신 및 발신시 자동으로 밑으로 스크롤  

>

- [시연영상](https://www.youtube.com/watch?v=kgryo3qVIrA)

---

### 📋 한국거래소 주식 정보 크롤링 및 백 테스팅( 2020.03 ~ 2020.04)

- 한국거래소에서 1994~ 2020년 주식 정보(PER-PBR, 순 매수 순위, 공매도, 가격) 수집 및 백 테스팅
- Python, tor, fake-useragent, cron
- **개발 부분**

>
PER-PBR, 거래주체별 순 매수 순위, 공매도, 가격을 한국거래소에서 크롤링  
tor 이용 IP 우회 후 request  
fake-useragent 이용 request 마다 header에 User Agent 변경  
cron 명령어로 특정 시간에 크롤링 프로그램 실행  
특정 기간 거래 주체(외국인, 개인, 기관) 별 백 테스팅 후 수익률 계산 프로그램 작성  

>

## 🎓  Education

---

### 전북대학교

|:------------------|:------------------|
**컴퓨터공학**      | 2017.03 - 2023.02
전체 **3.88 / 4.5** | 전공 **4.02 / 4.5**

## 📖 Certifications
---

|:--------------------------------|:------------------|
[AWS Certified Cloud Practitioner](https://www.credly.com/badges/455cdbe0-f0af-4b27-880a-646a809ec3ae/linked_in_profile]) | **2022년 09월 12일**     

## 🏆 **Awards**

---

|:-------------------|:-------------------------------------------------|:----------------------------|
**2021년 11월 07일** |제 7회 전북권 온라인 아이디어 해커톤 대회 대상    | 전북대학교 총장
**2021년 11월 26일** |2021년 컴퓨터공학부 작품경진대회 금상             | 전북대학교 컴퓨터공학부장
**2022년 03월 15일** |2021년 성적 우수상                                | 전북대학교 총장