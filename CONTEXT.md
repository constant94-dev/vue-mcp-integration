# Vue MCP Integration - 프로젝트 컨텍스트

## 📋 프로젝트 개요

Vue.js + TypeScript 기반 MCP 통합 클라이언트로, Spring Boot 백엔드와 연동하여 MCP 시스템의 사용자 인터페이스를 제공합니다. Nuxt.js 프레임워크를 사용하여 SSR/SSG 지원을 계획하고 있습니다.

### 주요 기능
- **대시보드**: MCP 시스템 상태 및 성능 모니터링
- **API 관리**: 공공데이터 API 호출 및 결과 시각화
- **세션 관리**: 사용자 세션 및 설정 관리
- **반응형 UI**: 모바일/데스크톱 반응형 인터페이스
- **MCP 클라이언트**: MCP 서버와의 직접 통신
- **실시간 데이터**: WebSocket을 통한 실시간 업데이트

## ✅ 완료된 작업

### Phase 0: 프로젝트 기반 설정 (100% 완료)
- ✅ **GitHub 저장소 생성**: `vue-mcp-integration` 저장소 생성
- ✅ **로컬 저장소 클론**: 개발 환경 설정 완료
- ✅ **프로젝트 구조 설계**: Vue.js + TypeScript 기반 구조 설계
- ✅ **기술 스택 결정**: Vue.js 3, TypeScript, Nuxt.js (예정)
- ✅ **프로젝트 문서화**: README.md 작성 및 간소화
- ✅ **워크스페이스 통합**: 전역 설정과 연동 완료

### 기술 스택 검토 완료
- ✅ **Vue.js 3**: 최신 Vue.js 프레임워크 선택
- ✅ **TypeScript**: 타입 안전성 확보
- ✅ **Nuxt.js**: SSR/SSG 지원 프레임워크 선택
- ✅ **Pinia**: 상태 관리 라이브러리 선택
- ✅ **Tailwind CSS**: 유틸리티 기반 CSS 프레임워크 선택

## 🚀 앞으로 진행할 작업

### Phase 1: 프로젝트 초기 설정
- [ ] **Nuxt.js 프로젝트 생성**
  - `npx nuxi@latest init .` 명령으로 프로젝트 초기화
  - TypeScript 설정 구성
  - 기본 프로젝트 구조 설정
- [ ] **개발 환경 설정**
  - ESLint 설정 (코드 품질 관리)
  - Prettier 설정 (코드 포맷팅)
  - TypeScript 설정 최적화
- [ ] **의존성 설치**
  - Pinia (상태 관리)
  - Tailwind CSS (스타일링)
  - Axios (HTTP 클라이언트)

### Phase 2: 기본 구현
- [ ] **기본 UI 컴포넌트 생성**
  - 레이아웃 컴포넌트 (Header, Sidebar, Footer)
  - 공통 컴포넌트 (Button, Card, Modal)
  - 폼 컴포넌트 (Input, Select, Form)
- [ ] **Spring Boot 백엔드 연동**
  - API 클라이언트 설정
  - 인터셉터 설정 (인증, 에러 처리)
  - 타입 정의 (API 응답 타입)
- [ ] **MCP 서버 직접 연동**
  - MCP 클라이언트 구현
  - STDIO 통신 설정
  - MCP 도구 호출 인터페이스
- [ ] **대시보드 페이지 구현**
  - 시스템 상태 모니터링
  - 성능 지표 시각화
  - 실시간 데이터 업데이트

### Phase 3: 고급 기능
- [ ] **상태 관리 구현**
  - Pinia 스토어 설정
  - 사용자 세션 관리
  - 애플리케이션 상태 관리
- [ ] **인증 시스템**
  - 로그인/로그아웃 기능
  - JWT 토큰 관리
  - 권한 기반 접근 제어
- [ ] **데이터 시각화**
  - 차트 라이브러리 연동
  - 실시간 데이터 업데이트
  - 반응형 차트 구현

## 📊 현재 상태

### 기술 스택
- **Vue.js**: 3 (예정)
- **TypeScript**: 타입 안전성
- **Nuxt.js**: SSR/SSG 지원 (예정)
- **Pinia**: 상태 관리 (예정)
- **Tailwind CSS**: 스타일링 (예정)

### 프로젝트 구조 (예정)
```
vue-mcp-integration/
├── components/           # Vue 컴포넌트
│   ├── layout/          # 레이아웃 컴포넌트
│   ├── common/          # 공통 컴포넌트
│   └── forms/           # 폼 컴포넌트
├── pages/               # 페이지 (자동 라우팅)
│   ├── index.vue        # 대시보드
│   ├── login.vue        # 로그인
│   └── api/             # API 관리
├── layouts/             # 레이아웃
│   └── default.vue      # 기본 레이아웃
├── composables/         # Composition API
│   ├── useAuth.ts       # 인증 관련
│   └── useApi.ts        # API 관련
├── types/               # TypeScript 타입 정의
│   ├── api.ts           # API 타입
│   └── user.ts          # 사용자 타입
├── api/                 # API 통신
│   ├── client.ts        # API 클라이언트
│   └── endpoints.ts     # API 엔드포인트
├── stores/              # Pinia 상태 관리
│   ├── auth.ts          # 인증 상태
│   └── app.ts           # 애플리케이션 상태
└── assets/              # 정적 자원
    ├── css/             # 스타일시트
    └── images/          # 이미지
```

### 성능 지표
- **목표 로딩 시간**: < 2초 (초기 로딩)
- **목표 응답성**: < 100ms (사용자 인터랙션)
- **목표 호환성**: Chrome, Firefox, Safari, Edge 지원

## ⚙️ 전역 설정 참조

이 프로젝트는 워크스페이스 루트의 전역 설정을 사용합니다:
- **전역 Cursor AI 규칙**: `/Users/ethan/Cursor/.cursor/.cursorrules`
- **전역 MCP 설정**: `/Users/ethan/Cursor/.cursor/mcp.json`
- **전역 프로젝트 개요**: `/Users/ethan/Cursor/cursor-workspace/PROJECTS.md`

## 🛠️ 기술 스택

### 현재 사용 중
- **Git**: 버전 관리
- **Node.js**: 개발 환경 (예정)

### 추가 예정
- **Vue.js 3**: 프론트엔드 프레임워크
- **TypeScript**: 타입 안전성
- **Nuxt.js**: SSR/SSG 지원
- **Pinia**: 상태 관리
- **Tailwind CSS**: 스타일링
- **Axios**: HTTP 클라이언트
- **Chart.js**: 데이터 시각화
- **WebSocket**: 실시간 통신
- **MCP 클라이언트**: MCP 서버 연동

## 📁 프로젝트 구조

### 향후 확장 계획
```
src/
├── components/           # Vue 컴포넌트
│   ├── layout/
│   │   ├── Header.vue
│   │   ├── Sidebar.vue
│   │   └── Footer.vue
│   ├── common/
│   │   ├── Button.vue
│   │   ├── Card.vue
│   │   └── Modal.vue
│   └── forms/
│       ├── Input.vue
│       └── Select.vue
├── pages/               # 페이지
│   ├── index.vue        # 대시보드
│   ├── login.vue        # 로그인
│   └── api/
│       ├── index.vue    # API 목록
│       └── [id].vue     # API 상세
├── layouts/
│   └── default.vue      # 기본 레이아웃
├── composables/         # Composition API
│   ├── useAuth.ts       # 인증 관련
│   ├── useApi.ts        # API 관련
│   └── useChart.ts      # 차트 관련
├── types/               # TypeScript 타입
│   ├── api.ts           # API 타입
│   ├── user.ts          # 사용자 타입
│   └── chart.ts         # 차트 타입
├── api/                 # API 통신
│   ├── client.ts        # API 클라이언트
│   ├── endpoints.ts     # API 엔드포인트
│   └── interceptors.ts  # 인터셉터
├── stores/              # Pinia 스토어
│   ├── auth.ts          # 인증 상태
│   ├── app.ts           # 애플리케이션 상태
│   └── api.ts           # API 상태
└── assets/              # 정적 자원
    ├── css/
    │   └── main.css     # 메인 스타일
    └── images/
        └── logo.png     # 로고
```

## 🔄 개발 과정

### 현재 워크플로우
1. **프로젝트 초기화**: Nuxt.js 프로젝트 생성
2. **환경 설정**: TypeScript, ESLint, Prettier 설정
3. **컴포넌트 개발**: 기본 UI 컴포넌트 구현
4. **페이지 개발**: 각 페이지별 기능 구현
5. **API 연동**: 백엔드 API와 통신 구현

### 새로운 기능 추가 방법
1. **컴포넌트 생성**: `components/NewComponent.vue`
2. **페이지 생성**: `pages/new-page.vue`
3. **타입 정의**: `types/newType.ts`
4. **API 연동**: `api/newEndpoint.ts`
5. **상태 관리**: `stores/newStore.ts`

## 🔗 관련 프로젝트

- **[spring-boot-mcp-integration](https://github.com/constant94-dev/spring-boot-mcp-integration)**: Spring Boot 백엔드 서버
- **[public-data-mcp-server](https://github.com/constant94-dev/public-data-mcp-server)**: 공공데이터 MCP 서버

## 📝 업데이트 히스토리

### 2025-08-17
- ✅ **GitHub 저장소 생성**: `vue-mcp-integration` 저장소 생성
- ✅ **로컬 저장소 클론**: 개발 환경 설정 완료
- ✅ **프로젝트 구조 설계**: Vue.js + TypeScript 기반 구조 설계
- ✅ **기술 스택 결정**: Nuxt.js, Pinia, Tailwind CSS 선택
- ✅ **프로젝트 문서화**: README.md 작성 및 간소화
- ✅ **워크스페이스 통합**: 전역 설정과 연동 완료

---

**마지막 업데이트**: 2025-08-17  
**작성자**: Ethan  
**상태**: 프로젝트 기반 설정 완료 ✅ (Nuxt.js 프로젝트 생성 준비됨)
