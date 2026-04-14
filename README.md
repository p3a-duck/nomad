# Yu Blog

Astro와 Markdown을 기반으로 구성한 개인 기술 블로그 프로젝트입니다.  
구현 기록, 설계 메모, 실험 결과를 정적 사이트 형태로 정리하는 것을 목표로 합니다.

## 실행 방법

```sh
npm install
npm run dev
```

- 개발 서버 기본 주소: `http://localhost:4321`
- 프로덕션 빌드 확인: `npm run build`

## GitHub Pages 배포

이 저장소는 GitHub Pages용 정적 Astro 블로그로 구성되어 있습니다.

1. GitHub 저장소의 `Settings > Pages`에서 `GitHub Actions`를 선택합니다.
2. `main` 브랜치에 푸시하면 `.github/workflows/deploy.yml`이 자동으로 빌드와 배포를 수행합니다.
3. 배포 전 [astro.config.mjs](./astro.config.mjs)의 `site` 값을 실제 Pages 주소로 바꾸는 것이 좋습니다.

예시:

```js
site: 'https://<github-username>.github.io/<repo-name>'
```

## 글 작성 방법

새 글은 `src/content/posts` 아래에 Markdown 파일로 추가합니다.

예시:

```md
---
title: "새 글 제목"
description: "글 요약"
pubDate: 2026-04-14
tags:
  - astro
  - note
---

본문 내용을 Markdown으로 작성합니다.
```

## 디렉터리 구조

```text
src/
├── components/      # Header, Footer, PostCard 등 UI 조각
├── content/
│   └── posts/       # Markdown 포스트
├── layouts/         # 공통 문서 레이아웃 및 SEO 메타데이터
└── pages/           # 홈, 블로그 목록, 상세 페이지
```

## 현재 포함된 기능

- 홈 페이지
- 블로그 목록 페이지
- 포스트 상세 페이지
- 공통 헤더/푸터
- 기본 SEO 메타데이터(title, description, og tags)
- Markdown 기반 샘플 포스트 2개
- GitHub Pages 정적 배포
