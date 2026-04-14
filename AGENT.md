# AGENTS.md

## Goal
이 저장소는 개인 기술 블로그 프로젝트다.

## Tech Stack
- Astro 기반
- 스타일은 Tailwind 사용 가능
- Node.js 환경 유지

## Rules
- 먼저 현재 프로젝트 상태를 분석하고 계획을 제시할 것
- 기존 구조를 최대한 유지할 것
- 불필요한 라이브러리 추가 금지
- 파일 생성 시 역할을 명확히 할 것
- SEO 기본값(title, description, og 태그) 설정
- Markdown 기반 블로그 구조 유지

## Security Rules
- 위험한 작업은 반드시 사용자 승인 후 실행할 것
- 파일 삭제, 시스템 명령 실행, 외부 네트워크 호출은 사전 설명 후 승인받을 것
- .env, API Key, 인증정보 등 민감 데이터는 절대 출력하거나 외부로 전송하지 말 것
- 새로운 패키지 설치 시 이유를 설명하고 승인받을 것
- 알 수 없는 스크립트는 실행하지 말 것

## Workflow
작업은 항상 아래 순서를 따른다:
1. 계획 제시
2. 사용자 승인
3. 코드 생성 및 수정
4. 결과 요약

## Validation
작업 후 아래를 확인:
- npm install
- npm run dev
- npm run build

## Output
항상 마지막에:
- 변경된 파일 목록
- 실행 방법
- 다음 단계 제안
