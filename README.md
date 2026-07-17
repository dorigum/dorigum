# 🐻‍❄️ Polar bear 빼꼼의 개발 성장 일지

> 하고 싶은 것도, 좋아하는 것도 많은 다재다능 제너럴리스트 PM을 꿈꾸고 있어요.<br>
> 사용자의 흐름을 먼저 생각하고, 직접 만들고 고치고 배포하면서 배운 것을 차곡차곡 기록합니다 🚀

---

## 💫 About Me

- 📊 경영정보학 / 산업공학 전공
- 🧸 사람을 좋아하는 파워 내향형 ISFJ
- 🧭 사용자의 문제와 흐름을 먼저 정리한 뒤 기능으로 옮기는 과정을 좋아해요.
- 🛠️ 서비스 기획, 사용자 경험, 백엔드 개발, 프론트엔드, 배포 자동화까지 전체 흐름을 이해하려고 공부하고 있어요.
- 📝 작은 실습도 기록으로 남기고, 에러와 해결 과정도 다시 설명할 수 있게 정리하려고 해요.
- 📧 `kkamang03@gmail.com`

---

## 🚀 Recent Projects

### 🏠 04_Final Project_ZIPT

> 등기부등본 분석, 임대차계약서 검토, HUG 전세보증보험 조건 확인, 동네 인프라 브리핑을 한 흐름으로 연결한 전세사기 방지 플랫폼이에요.

- **Service**: https://zipt.store/
- **Frontend Repo**: https://github.com/1-ZIPT/front_zipt
- **Backend Repo**: https://github.com/1-ZIPT/back_zipt
- **Frontend**: React 19, Vite, React Router, TanStack Query, Zustand, SCSS, Kakao Maps, Gemini API
- **Backend**: Java 21, Spring Boot 3.5, Spring Security, JPA, MySQL, Redis, PostgreSQL + pgvector, Spring AI
- **Infra**: AWS EC2, S3, CloudFront, Route53, Docker, GitHub Actions, Prometheus, Grafana, CloudWatch

#### ✨ 제가 집중한 작업

- 전월세 계약 전후의 사용자 흐름을 기준으로 홈, 분석, 계약서, 지도, 마이페이지 화면 구조를 정리했어요.
- 등기부등본/계약서 분석 이력과 상세 리포트를 React Query 기반으로 관리했어요.
- Zustand 기반 인증 상태, silent refresh, OAuth redirect 흐름을 정리했어요.
- Kakao 지도 기반 동네 인프라 탐색과 AI 브리핑 화면을 구현했어요.
- 프론트엔드 README, API 흐름, 성능 개선 포인트, 트러블슈팅을 문서화했어요.

#### 🧠 이번 작업을 통해 배운 것

- 사용자는 기능보다 “지금 내가 어디에 있고 다음에 뭘 해야 하는지”를 먼저 느낀다는 것
- 백엔드 분석 결과를 화면에 보여줄 때는 성공/실패/진행중 상태를 모두 자연스럽게 설계해야 한다는 것
- 배포된 서비스는 코드뿐 아니라 환경 변수, API 경로, 인증 흐름, 캐시까지 같이 봐야 한다는 것

---

### 🦄 03_Backend Project_CodeMate

> 개발자를 위한 스터디와 모각코 모집, 신청, 승인/거절, 정원 관리를 다루는 Spring Boot 백엔드 API 프로젝트예요.

- **Repo**: https://github.com/dorigum/3_CodeMate_Project
- **Stack**: Java 17, Spring Boot, Spring Security, Spring Data JPA, MySQL, Flyway, Docker, GitHub Actions, Testcontainers
- **Deploy**: GitHub Actions → Docker Hub → AWS EC2 → Docker Compose → ALB / ACM HTTPS

#### ✨ 제가 집중한 작업

- 스터디 참여 신청과 방장 승인/거절 상태 흐름을 설계했어요.
- 비관적 락을 적용해 정원 마감 직전 동시 요청이 들어와도 데이터 정합성이 깨지지 않도록 구성했어요.
- Refresh Token Rotation, SHA-256 저장, JWT blacklist 기반으로 인증 흐름을 고도화했어요.
- 키워드, 카테고리, 모집 상태, 지역, 기술 스택 등 여러 조건을 조합한 검색과 페이징을 구현했어요.
- Testcontainers 기반 MySQL 통합 테스트와 CI 파이프라인을 구성했어요.

#### 🧠 이번 작업을 통해 배운 것

- 단순 CRUD처럼 보여도 “신청 → 승인 → 정원 변경 → 모집 상태 변경”처럼 상태가 얽히면 비즈니스 규칙이 훨씬 중요해진다는 것
- 인증은 로그인 성공보다 토큰 만료, 재발급, 로그아웃, 비밀번호 변경 이후의 흐름까지 같이 봐야 한다는 것
- 테스트 환경이 실제 DB와 가까울수록 배포 전 불안이 줄어든다는 것

---

### 🧳 02_Frontend Project_CodeTrip

> 2인 팀 프로젝트로 시작해 AWS 기반으로 배포했던 여행 큐레이션 서비스를,<br>
> 이후 공모전 제출을 위해 개인적으로 Firebase 기반 구조로 전환하며 다시 정리한 프로젝트예요.

공공 여행 데이터, 날씨, 위시리스트, 폴더, 메모, 체크리스트, 커뮤니티 기능을 결합한 여행 큐레이션 서비스입니다.

- **Main Repo**: https://github.com/dorigum/2_CodeTrip_Project
- **Firebase Log Repo**: https://github.com/dorigum/CodeTrip-firebase-log
- **Service**: https://newagent-9c2a8.web.app/
- **Original Deploy**: AWS 기반 2인 팀 프로젝트 배포 경험
- **Personal Refactor**: 공모전 제출 목적의 Firebase Authentication / Realtime Database / Hosting 전환
- **Stack**: React, Vite, Zustand, Tailwind CSS, Express, MySQL, AWS, Firebase Authentication, Realtime Database, Firebase Hosting

#### ✨ 제가 집중한 작업

- 2인 팀 프로젝트로 AWS 배포까지 진행한 뒤, 공모전 제출 목적에 맞춰 Firebase 기반 배포 구조로 개인 전환했어요.
- Firebase Authentication 기반 로그인/회원가입과 Hosting 배포 흐름을 정리했어요.
- Realtime Database 기반 위시리스트, 폴더, 메모, 체크리스트 데이터 구조를 다시 설계했어요.
- 여행지 상세, Kakao Map, 최근 본 여행지, 커뮤니티 게시글/댓글 UX를 개선했어요.
- 날씨와 관심 지역을 활용한 여행지 추천 흐름을 보완했어요.
- Firebase 전환 문서, 수정 로그, 상세 내역서를 작성했어요.

#### 🧠 이번 작업을 통해 배운 것

- “팀 프로젝트로 만든 서비스”를 목적에 맞게 개인 제출용 구조로 다시 정리하는 과정도 중요한 개발 경험이라는 것
- “로컬에서 되는 코드”, “AWS에서 배포되는 코드”, “Firebase로 빠르게 제출 가능한 코드”는 각각 설계 관점이 다르다는 것
- Firebase는 빠르게 배포하기 좋지만, 데이터 구조와 보안 규칙을 처음부터 잘 생각해야 한다는 것
- 기능 구현만큼이나 사용자가 자연스럽게 이동하고 저장하고 다시 확인하는 흐름이 중요하다는 것

---

### ☕ 01_Java Project_Cafe Kiosk

> KOSTA 1차 미니 프로젝트로 진행한 Java 기반 카페 주문/관리 키오스크 프로젝트예요. Java 기본기와 데이터베이스 모델링을 함께 연습했습니다.

- **Repo**: https://github.com/dorigum/1_Cafe_kiosk_Project
- **Stack**: Java, MySQL, JDBC, ERD 설계
- **ERD**: dbdiagram / ERDCloud 기반 테이블 구조 설계

#### ✨ 제가 집중한 작업

- 메뉴 조회, 주문, 결제 흐름을 콘솔 기반 키오스크 기능으로 구현했어요.
- 역할별 클래스를 분리하며 객체지향 설계를 연습했어요.
- `cafe_kiosk` 데이터베이스 기준으로 테이블 구조와 관계를 설계했어요.
- DB 접속 정보는 `dbinfo.properties`로 분리하고 `.gitignore`로 관리하는 습관을 정리했어요.

#### 🧠 이번 작업을 통해 배운 것

- 작은 콘솔 프로젝트라도 메뉴, 주문, 결제처럼 흐름을 나누면 구조 설계가 필요하다는 것
- DB 모델링을 먼저 해두면 기능 구현 방향이 훨씬 선명해진다는 것
- 접속 정보처럼 민감한 값은 처음부터 코드와 분리하는 습관이 중요하다는 것

---

## 🌱 2026 Study Log

### Backend

- Java 기본 문법, 객체지향, 예외 처리, 컬렉션, 파일 처리
- JDBC와 SQL 기반 데이터 접근 흐름
- Servlet / JSP / MVC 구조 이해
- Spring MVC 기반 CRUD, Ajax, 게시판 기능 구현
- Spring Boot 프로젝트 구조, Controller-Service-Repository 계층 설계
- JPA, 연관관계 매핑, 트랜잭션, QueryDSL 실습
- Spring Security, JWT, OAuth2, 권한 처리, Swagger API 문서화

### Frontend & Product

- HTML, CSS, JavaScript 기본기
- React, Vite, React Router 기반 프론트엔드 구조 이해
- Context, Redux, Zustand 상태 관리 실습
- TanStack Query 기반 서버 상태 관리 실습
- 사용자 흐름을 고려한 화면 이동, 이력 관리, 리포트 UI, 마이페이지 구성

### DevOps & Infra

- Git / GitHub 커밋, 브랜치, 원격 저장소 관리
- Docker 이미지, Dockerfile, Docker Compose 실습
- GitHub Actions 기반 CI/CD workflow 작성
- AWS EC2, RDS, S3, CloudFront, Route53, ALB, ACM HTTPS 배포 흐름 학습
- Prometheus, Grafana, CloudWatch 기반 모니터링 학습
- Terraform 기반 IaC 기본 실습

### Data & AI

- Python, NumPy, Pandas 기초 실습
- Spring AI, AWS Bedrock Claude, Gemini API, OCR, RAG, pgvector 활용 경험

---

## 🗂 Remote Repository Highlights

| Repo | 기록한 내용 |
| --- | --- |
| [306-DevOps-Edu](https://github.com/dorigum/306-DevOps-Edu) | KOSTA DevOps 306기 Java/Spring/DevOps 학습 기록 |
| [3_CodeMate_Project](https://github.com/dorigum/3_CodeMate_Project) | Spring Security 기반 개발자 스터디 서비스 백엔드 |
| [2_CodeTrip_Project](https://github.com/dorigum/2_CodeTrip_Project) | React 기반 여행지 소개 및 추천 서비스 |
| [CodeTrip-firebase-log](https://github.com/dorigum/CodeTrip-firebase-log) | CodeTrip Firebase 배포 전환 작업 로그 |
| [1_Cafe_kiosk_Project](https://github.com/dorigum/1_Cafe_kiosk_Project) | Java 기반 카페 키오스크와 DB 모델링 미니 프로젝트 |
| [cicd03_back_security](https://github.com/dorigum/cicd03_back_security) | Spring Security 백엔드 CI/CD 실습 |
| [cicd04_front_react](https://github.com/dorigum/cicd04_front_react) | React 프론트엔드 CI/CD 실습 |
| [cicd02_boot](https://github.com/dorigum/cicd02_boot) | Spring Boot 배포 파이프라인 실습 |

---

## 🛠 Tech Stack

### 💻 Backend & Server

<img src="https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=java&logoColor=white"> <img src="https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white"> <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white"> <img src="https://img.shields.io/badge/Spring%20Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white"> <img src="https://img.shields.io/badge/JPA-59666C?style=for-the-badge"> <img src="https://img.shields.io/badge/REST%20API-02569B?style=for-the-badge"> <img src="https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white"> <img src="https://img.shields.io/badge/OAuth2-4285F4?style=for-the-badge&logo=google&logoColor=white"> <img src="https://img.shields.io/badge/Flyway-CC0200?style=for-the-badge&logo=flyway&logoColor=white"> <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white">

### 💾 Database & Cloud

<img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white"> <img src="https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white"> <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white"> <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white"> <img src="https://img.shields.io/badge/pgvector-4169E1?style=for-the-badge&logo=postgresql&logoColor=white"> <img src="https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black"> <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white"> <img src="https://img.shields.io/badge/AWS%20EC2-FF9900?style=for-the-badge&logo=amazonec2&logoColor=white"> <img src="https://img.shields.io/badge/AWS%20S3-569A31?style=for-the-badge&logo=amazons3&logoColor=white"> <img src="https://img.shields.io/badge/CloudFront-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white"> <img src="https://img.shields.io/badge/Route%2053-8C4FFF?style=for-the-badge&logo=amazonroute53&logoColor=white">

### 🎨 Frontend

<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"> <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black"> <img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white"> <img src="https://img.shields.io/badge/React%20Router-CA4245?style=for-the-badge&logo=reactrouter&logoColor=white"> <img src="https://img.shields.io/badge/Zustand-443E38?style=for-the-badge&logo=react&logoColor=white"> <img src="https://img.shields.io/badge/TanStack%20Query-FF4154?style=for-the-badge&logo=reactquery&logoColor=white"> <img src="https://img.shields.io/badge/Axios-5A29E4?style=for-the-badge&logo=axios&logoColor=white"> <img src="https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white"> <img src="https://img.shields.io/badge/SCSS-CC6699?style=for-the-badge&logo=sass&logoColor=white">

### 🧪 Test & Quality

<img src="https://img.shields.io/badge/JUnit5-25A162?style=for-the-badge&logo=junit5&logoColor=white"> <img src="https://img.shields.io/badge/Testcontainers-2496ED?style=for-the-badge&logo=docker&logoColor=white">

### 🤖 AI & Data

<img src="https://img.shields.io/badge/Spring%20AI-6DB33F?style=for-the-badge&logo=spring&logoColor=white"> <img src="https://img.shields.io/badge/AWS%20Bedrock-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white"> <img src="https://img.shields.io/badge/OCR-555555?style=for-the-badge"> <img src="https://img.shields.io/badge/RAG-111827?style=for-the-badge">

### 🧰 DevOps & Tools

<img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white"> <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"> <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white"> <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"> <img src="https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black"> <img src="https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white"> <img src="https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white">

### 🤝 Collaboration & Docs

<img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white"> <img src="https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=notion&logoColor=white">

- Discord로 팀원들과 진행 상황, 이슈, 회의 내용을 빠르게 공유했어요.
- Notion에 기획 문서, 회의록, API 흐름, 작업 체크리스트를 정리했어요.
- 구현 전에는 사용자 흐름을 먼저 정리하고, 구현 후에는 작업 로그와 회고를 남기려고 해요.

---

## 📌 My Working Style

- 📝 기능을 만들기 전에 목적과 사용자 흐름을 먼저 정리해요.
- 🧩 작은 단위로 구현하고 바로 확인해요.
- 🐛 에러가 나면 원인을 기록하고, 해결 과정을 다시 설명할 수 있게 정리하려고 해요.
- 📚 작업이 끝나면 코드 실습과 문서화를 함께 가져가며 학습 맥락을 잃지 않으려고 해요.
- 🤝 Discord와 Notion을 활용해 팀원들과 같은 맥락을 보고 작업하려고 해요.
- 🔗 기획, 개발, 배포를 따로 보지 않고 하나의 서비스 흐름으로 이해하려고 해요.
- 🌱 완벽하진 않아도 매일 조금씩 나아지는 개발자가 되고 싶어요.

---

## 🚀 Quick Links & Daily Flow

| 📅 2026 Focus | 🧠 Knowledge Base | 🎶 Working Music |
| :---: | :---: | :---: |
| [![Todo](https://img.shields.io/badge/2026_Focus-Todo_List-blue?style=flat-square&logo=github)](https://github.com/users/dorigum/projects/1) | [![NotebookLM](https://img.shields.io/badge/NotebookLM-Study_Notes-E37400?style=flat-square&logo=google)](https://notebooklm.google.com/notebook/026bc33a-5adb-4dbb-970a-f1116c05c871) | [![Playlist](https://img.shields.io/badge/Playlist-Working_Music-1DB954?style=flat-square&logo=spotify)](https://open.spotify.com/playlist/2wfOsCeCEvEKlDhQ0RYg4p?si=KbqnExpKRXGpynhE3V_SLw&nd=1&dlsi=33fdfb22bac54b5d) |

---

## 🌼 작은 다짐

> 오늘의 커밋이 내일의 저를 조금 더 단단하게 만들어준다고 믿어요.<br>
> 기획과 개발, 배포를 함께 이해하는 PM으로 성장하고 싶어 공부하고 있습니다 ✨

🗓️ _Last Updated: 2026-07-17_
