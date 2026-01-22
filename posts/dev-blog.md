---
title: Blog 만들기 (feat. Next + Obsidian)
description: useEffect가 언제 실행되는지 렌더링 흐름 기준으로 정리합니다.
date: 2025-01-10
category: react
tags:
  - react
  - hooks
  - lifecycle
draft: false
---

### 콘텐츠 시스템 구축

- [x] Frontmatter 구조 정의

```
---
title: useEffect 실행 시점 완벽 정리
description: useEffect가 언제 실행되는지 렌더링 흐름 기준으로 정리합니다.
date: 2025-01-10
category: react
tags:
  - react
  - hooks
  - lifecycle
draft: false
---

```

Obsidian에서 template을 지정해서 파일 생성시 자동으로 만들어지게 했다.

- [x]  `content/posts` 디렉토리 생성

**blog 구조**
blog-contents : obsidian을 CMS로 사용
blog : Next로 개발

obsidian으로 글작성 -> blog-contents push -> blog 배포

지금까지는 블로그 컨텐츠를 Obsidian을 이용해 CMS 방식으로 사용하는걸 했음.
이제 만들어진 repository의 posts들을 next에서 조회 해야한다.
~~조회하기 위해서는 github api를 이용했다. ~~
~~api로 호출하려고 했는데 git submodule방식으로 하기로...~~

아니 그냥 CMS방식으로 분리하고 싶어서 github API 이용하는걸루





- [ ] MDX 도입

- [ ] Post 타입 정의
- [ ] `getAllPosts`, `getPostBySlug` 구현
- [ ] draft 글 처리


## 핵심 페이지 구현

### 📄 필수 페이지

- [ ]  홈 (소개 + 최신 글)
- [ ]  글 목록
- [ ]  글 상세 (SSG)
- [ ]  404
### 🔧 렌더링

- [ ]  `generateStaticParams`
- [ ]  metadata 적용
- [ ] ISR 옵션 설정