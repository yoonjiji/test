# Team Project - **Noldabam**

> **놀다밤**은 낮에는 문화생활, 밤에는 휴식 — 하루를 가득 채우는 특별한 경험이란 의미에서 이름을 지었습니다.

> **놀다밤**은 다양한 세대와 라이프스타일을 아우르는 문화 소비 흐름을 반영해, 사용자에게 숙박과 공연을 한 번에 예약할 수 있는 통합 플랫폼을 직접 **기획**하고 **개발**하였습니다.

> **다양한 외부 API**를 통합하고 이를 실서비스 수준으로 가공·활용하여 사용자 편의를 고려한 맞춤형 서비스로 가공했습니다.

🔗 [배포 링크 바로가기](http://noldabam.s3-website.ap-northeast-2.amazonaws.com/)

---

## 📎 목차 바로가기

- [🏁 프로젝트 목표](#-프로젝트-목표)
- [👥 팀원 구성](#-팀원-구성)
- [⚙️ 개발 환경 및 스택](#️-개발-환경-및-스택)
- [📌 주요 기능 요약](#-주요-기능-요약)
- [🔍 다이어그램 / 폴더 구조도 / ERD](#-다이어그램--폴더-구조도--erd)
- [💻 화면 구성](#-화면-구성)

---

## 🏁 **프로젝트 목표**

1. 다양한 외부 API(날씨, 숙박, 공연, 지도) 통합 및 데이터 가공 경험
2. MySQL과 Firebase를 병행한 하이브리드 백엔드 아키텍처 설계
3. 사용자 맞춤형 숙박·공연/테마 예약 서비스 구현
4. 클라이언트 ↔ 서버 ↔ DB 간의 전체 연동 흐름 설계 및 구현
5. React 기반 SPA 구조를 활용한 반응형 UI 개발

---

## 👥 **팀원 구성**

| 이름   | 담당 기능                                                                                            |
| ------ | ---------------------------------------------------------------------------------------------------- |
| 정민규 | 전체 UI 디자인 / 홈 / 마이페이지(회원설정) / 숙박, 공연 페이지 / 리뷰(상세페이지) / AI챗봇 / DB 관리 |
| 강현우 | 공연 좌석 선택 / 예약 / 결제                                                                         |
| 오광석 | 숙박,공연 페이지/ 등급, 쿠폰 / 관리자 페이지 / 마이페이지(리뷰) / DB 관리                            |
| 윤지혜 | 로그인 / 회원가입 / 아이디, 비밀번호 찾기 / 마이페이지                                               |

---

## ⚙️ **개발 환경 및 기술 스택**

### 🎨 Frontend

<p>
  <img src="https://img.shields.io/badge/React-61DAFB?style=flat&logo=React&logoColor=white"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=JavaScript&logoColor=black"/>
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=HTML5&logoColor=white"/>
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=CSS3&logoColor=white"/>
  <img src="https://img.shields.io/badge/Tailwind%20CSS-white?logo=tailwindcss"/>
</p>

---

### 🛠️ Backend

<p>
  <img src="https://img.shields.io/badge/Node.js-339933?style=flat&logo=Node.js&logoColor=white"/>
  <img src="https://img.shields.io/badge/Express-000000?style=flat&logo=Express&logoColor=white"/>
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=MySQL&logoColor=white"/>
  <img src="https://img.shields.io/badge/MySQLWorkbench-00758F?style=flat&logo=mysql&logoColor=white"/>
  <img src="https://img.shields.io/badge/Firebase--Admin-FFCA28?style=flat&logo=firebase&logoColor=black"/>
</p>

---

### 🤝 Collaboration

<p>
  <img src="https://img.shields.io/badge/Git-F05032?style=flat&logo=Git&logoColor=white"/>
  <img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=GitHub&logoColor=white"/>
  <img src="https://img.shields.io/badge/Notion-000000?style=flat&logo=Notion&logoColor=white"/>
  <img src="https://img.shields.io/badge/VSCode-007ACC?style=flat&logo=VisualStudioCode&logoColor=white"/>
</p>

---

### 🧩 Libraries & Tools

<p>
<img src="https://img.shields.io/badge/Axios-5A29E4?style=flat&logo=Axios&logoColor=white"/>
  <img src="https://img.shields.io/badge/JWT-000000?style=flat&logo=JSONWebTokens&logoColor=white"/>
  <img src="https://img.shields.io/badge/bcrypt-121212?style=flat&logoColor=white"/>
  <img src="https://img.shields.io/badge/Swiper-6332F6?style=flat&logo=Swiper&logoColor=white"/>
  <img src="https://img.shields.io/badge/OpenAI-412991?style=flat&logo=OpenAI&logoColor=white"/>
  <img src="https://img.shields.io/badge/dotenv-ECD53F?style=flat&logo=dotenv&logoColor=black"/>
  <img src="https://img.shields.io/badge/CORS-003545?style=flat&logoColor=white"/>
  <img src="https://img.shields.io/badge/React_Hook_Form-EC5990?style=flat&logo=ReactHookForm&logoColor=white"/>
  <img src="https://img.shields.io/badge/Multer-34D058?style=flat&logoColor=white"/>
</p>

---

## 📌 **주요 기능 요약**

### 🔐 **회원 관련**

- **로그인/로그아웃**:
  - JWT 토큰 기반 인증
  - 아이디 저장 기능
  - 소셜 로그인 (Naver, Google, Kakao)
- **회원가입**:
  - 단계별 회원가입 프로세스
  - 아이디 중복 확인
  - 비밀번호 유효성 검사
  - 이메일 인증
- **아이디/비밀번호 찾기**:
  - 이메일 기반 아이디 찾기
  - 휴대폰 인증 기반 비밀번호 재설정
- **마이페이지**:
  - 프로필 관리 (이름, 연락처, 이메일 수정)
  - 회원 등급 및 포인트 조회
  - 예약 내역 관리
  - 리뷰/평점 관리
  - 회원 탈퇴

### 🏨 **숙박 & 테마/공연 예약 페이지**

- **메인 페이지**:
  - 숙소, 테마/공연 검색
  - 지역/날짜/인원 기반 필터링
  - 실시간 날씨 정보 제공
- **상세 페이지**:
  - 숙소/테마/공연 상세 정보
  - 리뷰 및 평점 조회
  - 예약 가능 날짜 확인
- **예약 시스템**:
  - 숙소: 객실 선택 및 예약
  - 테마/공연: 좌석 선택 및 예매
  - 카카오페이 결제 연동
- **리뷰 시스템**:
  - 평점 및 리뷰 관리

### 👨‍💼 **관리자 기능**

- **회원 관리**: 회원 목록 조회, 회원 등급별 쿠폰 발급
- **주문 관리**: 숙박, 테마/공연 주문 리스트 조회
- **리뷰 관리**: 숙박, 테마/공연 리뷰 리스트 조회 및 삭제
- **쿠폰 관리**: 쿠폰 발급 리스트 조회 및 삭제

---

## 🔍 **프로젝트 개발 환경**

### 🖼 **코딩 컨벤션**

![코딩컨벤션](https://github.com/user-attachments/assets/52bd8064-c43d-423a-9e4d-c131a6c99514)

### 🗂️ **개발 폴더 구조도**

```csharp
noldabam/                           # 프로젝트 루트 디렉토리
├── .git/                         # Git 버전 관리 디렉토리
├── client/                       # 프론트엔드 클라이언트 코드
│   ├── src/                      # 소스 코드 메인 디렉토리
│   │   ├── services/             # API 통신 및 외부 서비스 연동
│   │   ├── page/                 # 페이지 컴포넌트들
│   │   ├── hooks/                # 커스텀 React 훅
│   │   ├── context/              # React Context 관련 파일들
│   │   ├── components/           # 재사용 가능한 UI 컴포넌트들
│   │   ├── utils/                # 유틸리티 함수들
│   │   ├── lib/                  # 라이브러리 관련 코드
│   │   ├── features/             # 주요 기능별 모듈
│   │   ├── app/                  # 앱의 핵심 로직
│   │   ├── index.js              # 앱의 진입점
│   │   ├── App.js                # 메인 앱 컴포넌트
│   │   ├── filtersData.js        # 필터링 관련 데이터
│   │   ├── accommodationDetailData.js  # 숙박 상세 데이터
│   │   └── themeDetailData.js    # 테마/공연 상세 데이터
│   ├── public/                   # 정적 파일들
│   ├── tailwind.config.js        # Tailwind CSS 설정
│   ├── insert_members.py         # 회원 데이터 삽입 스크립트
│   ├── final_customers.json      # 고객 데이터
│   ├── README.md                 # 프로젝트 문서
│   ├── .gitignore                # Git 제외 파일 목록
│   └── .env                      # api 인증 키 파일
├── server/                       # 백엔드 서버 코드
│   ├── upload_files/             # 업로드된 파일 저장소
│   ├── router/                   # API 라우터
│   ├── repository/               # 데이터베이스 접근 계층
│   ├── controller/               # 비즈니스 로직 처리
│   ├── firebase/                 # Firebase 관련 설정
│   ├── middleWare/               # 미들웨어 함수들
│   ├── server.js                 # 서버 진입점
│   ├── hashPassword.js           # 비밀번호 해싱 유틸리티
│   ├── .gitignore                # Git 제외 파일 목록
│   └── .env                      # api 인증 키 파일
└──  sql/                         # 데이터베이스 관련 파일들
```

### 💾 **ERD**
#### MySQL
![erd](https://github.com/user-attachments/assets/16878393-e140-4cd0-856b-7da96d01a28e)
- MySQL은 멤버, 주문 등 구조화된 핵심 데이터를 저장하여 안정성과 관계형 데이터 관리를 담당

#### FireBase
![firebase](https://github.com/user-attachments/assets/5bf3392d-8f5e-47dd-8ab7-45fdf61d6b64)
- Firebase는 리뷰, 쿠폰처럼 읽기·쓰기 빈도가 높고 실시간 반영이 필요한 데이터를 저장하여 빠른 응답성과 유연성을 확보

### 🚩 **배포 환경**
![배포](https://github.com/user-attachments/assets/c4c821df-5c42-4f96-b4a4-d9141f39f238)

---

## 💻 **화면 구성**

### 1️⃣ 로그인 / 회원가입

![loginSignup](https://github.com/user-attachments/assets/8046cb62-e85d-4cfb-a063-132cdcb03679)

### 2️⃣ 마이페이지 / 회원설정 / 회원탈퇴

#### 마이페이지
![mypage](https://github.com/user-attachments/assets/9ec5928f-3e97-467f-a59c-577750627118)

#### 회원설정 / 회원탈퇴
![userSetting](https://github.com/user-attachments/assets/9ef13eec-cc32-4974-b886-a5a0b8a3fcf1)

### 3️⃣ 메인페이지

![main](https://github.com/user-attachments/assets/00b511ce-fa6d-4ce9-ac55-b87d0ee925be)

### 4️⃣ 숙소 검색 페이지

![search](https://github.com/user-attachments/assets/31dc58f0-d1b1-4e10-b0e4-8fa5353413d0)

### 5️⃣ 결제페이지

![order](https://github.com/user-attachments/assets/c7fce3b6-f6b9-4c79-8006-71a5504a1dfb)

### 6️⃣ 예약 상세페이지

![detail](https://github.com/user-attachments/assets/553e1cbf-bbd5-4855-b26a-c109a4f71098) ㅇ

#### 좌석 예약 페이지

![seat](https://github.com/user-attachments/assets/2c80642c-7373-463c-9fd4-d1c41d857f5d)

### 7️⃣ 리뷰 페이지

![review](https://github.com/user-attachments/assets/1af0bc09-0cc6-4832-b9d7-c8bf5a2dc820)

### 8️⃣ 관리자 페이지

![admin](https://github.com/user-attachments/assets/fd041ee2-d5aa-4250-8e58-a5b6da3298cc)

---
