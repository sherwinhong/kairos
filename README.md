# Kairos ⏱️

> 광고 없는 무료 뽀모도로 타이머 — Web, iOS, watchOS, iPad 멀티플랫폼 동기화

## 기술 스택

- **Frontend:** React + Vite
- **Backend:** Spring Boot (Java)
- **Database:** PostgreSQL
- **인증:** Spring Security + JWT

## 주요 기능

- 집중 / 짧은 휴식 / 긴 휴식 모드 전환
- 원형 링 타이머 UI
- 세션 완료 시 태그 선택 (분야별 기록)
- 태그 추가 / 삭제
- 통계 페이지 (분야별 막대그래프 + 세션 히스토리)
- 4세션 완료 시 긴 휴식 자동 전환

## 로컬 실행

```bash
# 패키지 설치
npm install

# 개발 서버 실행
npm run dev
```

## 환경변수 설정

프로젝트 루트에 `.env` 파일 생성 후 아래 내용 추가:

```
VITE_API_URL=http://localhost:8080
```

## 프로젝트 구조

```
src/
  app/          # 앱 진입점, 전역 설정
  features/     # 기능별 모듈 (auth, sessions, tags, timer)
  shared/       # 공통 컴포넌트, 유틸, 타입
```
