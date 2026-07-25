# 🐻‍❄️ Polar bear 빼꼼의 개발 성장 일지

> 하고 싶은 것도, 좋아하는 것도 많은 다재다능 제너럴리스트 PM을 꿈꾸고 있어요.<br>
> 사용자의 흐름을 먼저 생각하고, 직접 만들고 고치고 배포하면서 배운 것을 차곡차곡 기록합니다 🚀

---

## 💫 About Me

- 📊 경영정보학 / 산업공학 전공
- 🧸 사람을 좋아하는 파워 내향형 ISFJ
- 🧭 사용자의 문제와 흐름을 먼저 정리한 뒤 기능으로 옮기는 과정을 좋아해요.
- 🛠️ 서비스 기획, 사용자 경험, 백엔드 개발, 프론트엔드, 배포 자동화까지 전체 흐름을 이해하려고 공부하고 있어요.
- 📧 `kkamang03@gmail.com`
- 🐻‍❄️ **실시간 웹 포트폴리오**: **[doyeon-dev-portfolio.web.app](https://doyeon-dev-portfolio.web.app/)** 

---

## 🚀 Recent Projects

### 🏠 04_Final Project_ZIPT (전세사기 방지 플랫폼)
> 등기부등본 분석, 임대차계약서 검토, HUG 전세보증보험 조건 확인, 동네 인프라 브리핑을 한 흐름으로 연결한 전세사기 방지 플랫폼

- **성능 최적화**: `React.lazy` 지연 로딩을 통한 초기 JS 메인 번들 **73.7% 감축** (1,243KB ➡️ 327KB) 및 LCP 개선
- **리소스 최적화**: 빌드타임 WebP 자동 변환 및 리사이징으로 이미지 파일 용량 **99.6% 극적 감소** (최대 370KB ➡️ 1.5KB)
- **아키텍처 설계**: 백엔드 서버 병목 방지를 위한 클라이언트단 Gemini API 직접 호출 및 5단계 fallback 파이프라인 설계
- **[🔗 상세 구현 기여도 및 트러블슈팅 보러가기](https://github.com/dorigum/Final_ZIPT_Project)**

---

### 🦄 03_Backend Project_CodeMate (개발자 스터디 매칭 API)
> 스터디 및 모각코 모집, 신청, 승인/거절 상태 관리 및 동시성 제어 Spring Boot 백엔드 API

- **동시성 제어**: 마감 직전 동시 신청 상황에서의 데이터 무결성을 위해 **JPA 비관적 락(Pessimistic Lock)** 적용
- **보안성 극대화**: Refresh Token Rotation(RTR), SHA-256 해싱, Redis 블랙리스트 기반 로그아웃 예외 차단
- **테스트 환경**: Testcontainers를 도입하여 실제 MySQL 환경과 100% 일치하는 통합 테스트 CI 파이프라인 구성
- **[🔗 상세 구현 기여도 및 트러블슈팅 보러가기](https://github.com/dorigum/3_CodeMate_Project)**

---

### 🧳 02_Frontend Project_CodeTrip (여행 큐레이션 서비스)
> 공공 여행 데이터, 실시간 날씨 추천, 위시리스트 및 메모 연동형 개인 맞춤형 여행 큐레이션 서비스

- **성능 최적화**: 공공 KTO API 호출 한계(429) 및 응답 지연을 인메모리 캐싱으로 극복, **응답 속도 99.5% 개선** (2s ➡️ 10ms)
- **UX 인터랙션**: 좋아요 및 댓글 액션에 **낙관적 업데이트(Optimistic Update)** 적용으로 네트워크 지연 없는 체감 속도 0ms 구현
- **클라우드 포팅**: 2인 AWS 배포 프로젝트를 공모전 제출을 목적으로 Firebase Auth / Realtime DB / Hosting 환경으로 포팅 완수
- **Service**: [dorigum-codetrip.web.app](https://dorigum-codetrip.web.app/)
- **[🔗 상세 구현 기여도 및 트러블슈팅 보러가기](https://github.com/dorigum/2_CodeTrip_Project)**

---

### ☕ 01_Java Project_Cafe Kiosk (콘솔 기반 관리/주문 키오스크)
> MVC 패턴 및 Layered Architecture 기반 콘솔 카페 키오스크 관리 시스템

- **구조적 유연성**: MVC 패턴을 충실히 적용해 UI와 백엔드 트랜잭션을 분리하여 향후 웹으로의 이식성을 고려한 설계 진행
- **결제 관리**: 회원/비회원 구매액 포인트 적립 및 차감 트랜잭션 안전성 확보 및 VVIP 구매 이력 추적 구현
- **보안 기초**: 민감한 DB 접속 정보를 properties 파일로 분리하고 gitignore를 활용하는 등 초기 보안성 습관 수립
- **[🔗 상세 구현 기여도 및 트러블슈팅 보러가기](https://github.com/dorigum/1_Cafe_kiosk_Project)**

---

## 🌱 2026 Study Log

- **Backend**: Java/Spring Boot 기반 MVC 계층 설계, JPA 연관관계 매핑 및 동시성 락 처리, Spring Security & JWT/OAuth2
- **Frontend**: React/Vite 기반 싱글 페이지 어플리케이션(SPA) 구조 설계, Zustand 전역 상태 및 TanStack Query 서버 상태 관리
- **DevOps**: Docker 컨테이너 오케스트레이션, GitHub Actions CI/CD 파이프라인, AWS(EC2, S3, CloudFront) 배포 프로세스
- **AI & Data**: Spring AI 기반 프롬프트 및 pgvector 연동 RAG 구현, Gemini API 브라우저 연동 아키텍처 실습

---

## 🗂 Remote Repository Highlights

| Repo | 기록한 내용 |
| --- | --- |
| [Final_ZIPT_Project](https://github.com/dorigum/Final_ZIPT_Project) | 전세사기 예방 및 부동산 가이드 AI 분석 서비스 (팀 공용 백업 저장소) |
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
<img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white"> <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"> <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white"> <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"> <img src="https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black"> <img src="https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white"> <img src="https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white"> <img src="https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white">

### 🤝 Collaboration & Tools
<img src="https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=notion&logoColor=white"> <img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white"> <img src="https://img.shields.io/badge/Obsidian-7C3AED?style=for-the-badge&logo=obsidian&logoColor=white">

---

## 📌 My Working Style

- 📝 기능을 만들기 전에 목적과 사용자 흐름을 먼저 정리해요.
- 🧩 작은 단위로 구현하고 바로 확인해요.
- 🐛 에러가 나면 원인을 기록하고, 해결 과정을 다시 설명할 수 있게 정리하려고 해요.
- 📚 작업이 끝나면 코드 실습과 문서화를 함께 가져가며 학습 맥락을 잃지 않으려고 해요.
- 🔗 기획, 개발, 배포를 따로 보지 않고 하나의 서비스 흐름으로 이해하려고 해요.

---

## 🚀 Quick Links & Daily Flow

| 📅 2026 Focus | 🧠 Knowledge Base | 🎶 Working Music |
| :---: | :---: | :---: |
| [![Todo](https://img.shields.io/badge/2026_Focus-Todo_List-blue?style=flat-square&logo=github)](https://github.com/users/dorigum/projects/1) | [![NotebookLM](https://img.shields.io/badge/NotebookLM-Study_Notes-E37400?style=flat-square&logo=google)](https://notebooklm.google.com/notebook/026bc33a-5adb-4dbb-970a-f1116c05c871) | [![Playlist](https://img.shields.io/badge/Playlist-Working_Music-1DB954?style=flat-square&logo=spotify)](https://open.spotify.com/playlist/2wfOsCeCEvEKlDhQ0RYg4p?si=KbqnExpKRXGpynhE3V_SLw&nd=1&dlsi=33fdfb22bac54b5d) |

---

## 🌼 작은 다짐

> 오늘의 커밋이 내일의 저를 조금 더 단단하게 만들어준다고 믿어요.<br>
> 기획과 개발, 배포를 함께 이해하는 PM으로 성장하고 싶어 공부하고 있습니다 ✨

🗓️ _Last Updated: 2026-07-22_
