# Web Tech Stack Handbook 2026

> 프런트엔드에서 배포·운영까지, 1인 웹 빌더를 위한 풀스택 기술 핸드북

프런트엔드, 백엔드, 데이터베이스, 배포와 제품 운영까지 웹 서비스를 구축하는 데 필요한 기술과 서비스를 정리합니다.

신규 프로젝트의 채택 추세뿐 아니라 **개발 속도, 운영 부담, 비용, 확장성**을 함께 고려합니다.

## 목록 정렬 원칙

같은 역할을 하는 기술은 다음 순서로 배치합니다. 다운로드 수나 누적 사용자 수만으로 판단하지 않고, 
**신규 프로젝트에서의 채택 추세와 권장도**를 우선합니다.

1. 혼자 빠르게 구축하고 운영하기 좋은 기술
2. 신규 프로젝트에서 널리 선택되는 기술
3. 생태계와 유지보수가 안정적인 대안
4. 특정 규모나 요구사항에 적합한 기술
5. 운영 부담이 크거나 Experimental 또는 Legacy인 기술

역할이 서로 다른 기술은 직접 비교하지 않으며, 각 목록은 정기적으로 최신 상태를 검토합니다.

## Contents

- [Frontend](#frontend)
- [Content and documentation](#content-and-documentation)
- [Styling and UI](#styling-and-ui)
- [Data and APIs](#data-and-apis)
- [Backend and server](#backend-and-server)
- [Background jobs and workflows](#background-jobs-and-workflows)
- [Email and notifications](#email-and-notifications)
- [Cache and application infrastructure](#cache-and-application-infrastructure)
- [Search](#search)
- [State management](#state-management)
- [Authentication](#authentication)
- [Development tools](#development-tools)
- [Testing](#testing)
- [Deployment and hosting](#deployment-and-hosting)
- [Operations](#operations)
- [Quality, security, and observability](#quality-security-and-observability)
- [Product integrations](#product-integrations)
- [Data visualization](#data-visualization)
- [Cross-platform development](#cross-platform-development)
- [Developer services](#developer-services)
- [AI development](#ai-development)
- [Git and releases](#git-and-releases)

## Frontend

### Core languages and standards

- [HTML](https://html.spec.whatwg.org/): 웹 문서 구조를 정의하는 표준 마크업 언어
- [CSS](https://www.w3.org/Style/CSS/): 웹 문서의 표현과 레이아웃을 정의하는 스타일 언어
- [JavaScript](https://developer.mozilla.org/docs/Web/JavaScript): 브라우저와 서버에서 실행되는 웹의 표준 프로그래밍 언어
- [TypeScript](https://www.typescriptlang.org/): JavaScript에 정적 타입을 추가하는 언어로, 현대적인 프런트엔드 프로젝트의 사실상 기본 선택
- [Web APIs](https://developer.mozilla.org/docs/Web/API): 브라우저가 제공하는 DOM, Fetch, Storage, Workers 등의 표준 API

### UI frameworks and libraries

- [React](https://react.dev/): 컴포넌트 기반 UI 라이브러리
- [Vue](https://vuejs.org/): 점진적으로 도입할 수 있는 UI 프레임워크
- [Angular](https://angular.dev/): 라우팅, 폼, 의존성 주입 등을 포함한 통합 웹 프레임워크
  - [RxJS](https://rxjs.dev/): 비동기 이벤트 스트림을 위한 리액티브 프로그래밍 라이브러리
  - [ReactiveX](https://reactivex.io/): 리액티브 프로그래밍 API와 언어별 구현을 소개하는 프로젝트
  - [Learn RxJS](https://www.learnrxjs.io/): RxJS 연산자와 패턴을 설명하는 학습 자료
- [Svelte](https://svelte.dev/): 컴파일러 기반 UI 프레임워크
- [jQuery](https://jquery.com/): DOM 조작과 레거시 웹 애플리케이션 유지보수에 사용되는 라이브러리

### Full-stack and meta-frameworks

- [Next.js](https://nextjs.org/): React 기반 풀스택 웹 프레임워크
- [React Router](https://reactrouter.com/): React 라우팅 및 풀스택 웹 프레임워크
- [Nuxt](https://nuxt.com/): Vue 기반 풀스택 웹 프레임워크
- [SvelteKit](https://svelte.dev/docs/kit): Svelte 기반 풀스택 웹 프레임워크
- [Astro](https://astro.build/): 콘텐츠 중심 웹사이트에 적합한 멀티 프레임워크 웹 프레임워크

### Static site and documentation generators

참고: [Jamstack Generators](https://jamstack.org/generators/)

- [Docusaurus](https://docusaurus.io/): React와 MDX 기반 문서 사이트 생성기
- [Hugo](https://gohugo.io/): 대규모 정적 사이트에 적합한 Go 기반 사이트 생성기
- [Gatsby](https://www.gatsbyjs.com/): React와 GraphQL 기반의 성숙한 정적 사이트 프레임워크

## Content and documentation

### Headless CMS

참고: [Jamstack Headless CMS](https://jamstack.org/headless-cms/)

- [Strapi](https://strapi.io/): Node.js 기반 오픈소스 Headless CMS
- [Sanity](https://www.sanity.io/): 커스텀 스키마와 실시간 협업에 강한 SaaS CMS
- [Payload](https://payloadcms.com/): TypeScript 및 Next.js 친화적인 코드 중심 CMS
- [Contentful](https://www.contentful.com/): 엔터프라이즈 환경에서 널리 사용되는 SaaS CMS
- [Ghost](https://ghost.org/): 블로그, 출판 및 뉴스레터에 특화된 CMS

### Markdown and MDX

- [MDX](https://mdxjs.com/): Markdown 안에서 JSX 컴포넌트를 사용할 수 있는 포맷
- [MDXEditor](https://mdxeditor.dev/): React 기반 WYSIWYG MDX 편집기

### Rich-text editors

- [Tiptap](https://tiptap.dev/): ProseMirror 기반 Headless 리치 텍스트 편집기
- [Lexical](https://lexical.dev/): Meta가 개발한 확장 가능한 리치 텍스트 편집기 엔진

### Syntax highlighting

- [Shiki](https://shiki.style/): VS Code 문법과 테마를 사용하는 구문 강조 엔진
- [Prism](https://prismjs.com/): 브라우저에서 사용하기 쉬운 경량 구문 강조 라이브러리

### Diagrams and code images

- [Mermaid](https://mermaid.js.org/): 텍스트로 다이어그램과 시퀀스 차트를 작성하는 도구
- [Carbon](https://carbon.now.sh/): 소스 코드를 이미지로 만드는 도구

### Documentation hosting

- [Read the Docs](https://about.readthedocs.com/): 문서 빌드 및 호스팅 플랫폼

### Feeds

- [W3C Feed Validation Service](https://validator.w3.org/feed/): RSS와 Atom 피드 유효성 검사 도구
- [Feeder](https://feeder.co/): RSS 피드 리더 및 알림 서비스
- [FeedBurner](https://feedburner.google.com/): 핵심 피드 관리 기능만 유지되는 레거시 서비스

## Styling and UI

### CSS frameworks

- [Tailwind CSS](https://tailwindcss.com/): CSS-first 설정을 사용하는 Utility-first CSS 프레임워크
- [Bootstrap](https://getbootstrap.com/): 완성형 컴포넌트를 제공하는 CSS 프레임워크

### CSS preprocessors

- [Sass](https://sass-lang.com/): CSS 전처리기

### CSS-in-JS and build-time styling

- [styled-components](https://styled-components.com/): React용 런타임 CSS-in-JS 라이브러리
- [Emotion](https://emotion.sh/): 프레임워크에 유연하게 적용할 수 있는 런타임 CSS-in-JS 라이브러리
- [vanilla-extract](https://vanilla-extract.style/): TypeScript 기반 Zero-runtime 스타일링 도구
- [Panda CSS](https://panda-css.com/): 빌드 시점에 스타일을 생성하는 타입 안전 CSS-in-JS 도구

### Headless components

- [Radix UI](https://www.radix-ui.com/): 접근성을 고려한 React Headless UI 컴포넌트
- [Headless UI](https://headlessui.com/): Tailwind Labs의 React 및 Vue용 Headless UI 컴포넌트
- [Base UI](https://base-ui.com/): MUI 팀이 만드는 React Headless UI 컴포넌트

### Styled component libraries

- [shadcn/ui](https://ui.shadcn.com/): Tailwind CSS와 Radix UI 또는 Base UI를 사용하는 코드 소유형 컴포넌트 모음
- [Material UI](https://mui.com/): Material Design 기반 React 컴포넌트 라이브러리
- [Ant Design](https://ant.design/): 관리 화면과 엔터프라이즈 제품에 강한 React UI 라이브러리
- [daisyUI](https://daisyui.com/): Tailwind CSS 플러그인 방식의 컴포넌트 라이브러리
- [Angular Material](https://material.angular.dev/): Angular용 Material Design 컴포넌트
- [PrimeNG](https://primeng.org/): Angular용 UI 컴포넌트 모음
- [spartan/ui](https://www.spartan.ng/): Angular와 Tailwind CSS 기반 UI 컴포넌트

### Admin application frameworks

- [React-admin](https://marmelab.com/react-admin/): 데이터 중심 관리자 애플리케이션용 React 프레임워크
- [Refine](https://refine.dev/): 관리자 화면과 내부 도구를 위한 Headless React 프레임워크

### Admin templates

- [shadcn/ui Templates](https://www.shadcn.io/template): shadcn/ui 기반 애플리케이션 템플릿 모음
- [Shadcn Admin](https://www.shadcn.io/template/satnaing-shadcn-admin): shadcn/ui 기반 관리자 대시보드 템플릿
- [Metronic](https://keenthemes.com/metronic): 상용 관리자 화면 템플릿
- [TailAdmin](https://tailadmin.com/): Tailwind CSS 기반 대시보드 템플릿

### Icons

- [Lucide](https://lucide.dev/): 일관된 디자인의 오픈소스 SVG 아이콘 모음
- [Font Awesome](https://fontawesome.com/): 광범위한 무료·상용 아이콘 라이브러리
- [Bootstrap Icons](https://icons.getbootstrap.com/): Bootstrap 팀이 제공하는 오픈소스 SVG 아이콘 모음

### Fonts

- [Google Fonts](https://fonts.google.com/): 웹 폰트 검색 및 제공 서비스
- [Inter](https://rsms.me/inter/): 화면과 사용자 인터페이스에 최적화된 오픈소스 글꼴

### Animation

#### UI and component animation

- [Motion](https://motion.dev/): React 및 JavaScript용 UI 애니메이션 라이브러리
- [AutoAnimate](https://auto-animate.formkit.com/): 레이아웃 변경을 자동으로 애니메이션하는 도구

#### Timeline and scroll animation

- [GSAP](https://gsap.com/): 복잡한 타임라인과 스크롤 애니메이션 라이브러리

#### Vector animation

- [Lottie](https://airbnb.io/lottie/): JSON 기반 벡터 애니메이션 포맷과 렌더러
- [LottieFiles](https://lottiefiles.com/): Lottie 애니메이션 에셋 검색, 제작 및 관리 플랫폼
- [dotLottie](https://dotlottie.io/): Lottie 에셋을 묶고 압축하는 `.lottie` 포맷
- [`@lottiefiles/dotlottie-react`](https://www.npmjs.com/package/@lottiefiles/dotlottie-react): React용 최신 dotLottie 플레이어

#### Number and text animation

- [CountUp.js](https://inorganik.github.io/CountUp.js/): 숫자 카운팅 애니메이션 라이브러리

### Gestures

- [use-gesture](https://use-gesture.netlify.app/): React용 터치, 드래그, 핀치 및 스크롤 제스처 훅
- [AlloyFinger](https://github.com/AlloyTeam/AlloyFinger): 프레임워크에 종속되지 않는 경량 멀티터치 제스처 라이브러리
- [Hammer.js](https://hammerjs.github.io/): 유지보수 중심의 기존 터치 제스처 라이브러리

### Data tables

- [TanStack Table](https://tanstack.com/table/latest): UI를 직접 구성하는 Headless 테이블 라이브러리
- [AG Grid](https://www.ag-grid.com/): 대용량 데이터와 엔터프라이즈 기능을 지원하는 그리드
- [MUI X Data Grid](https://mui.com/x/react-data-grid/): MUI 생태계의 데이터 그리드
- [DataTables](https://datatables.net/): TypeScript 기반의 독립 실행형 테이블 라이브러리 (v2 이하: jQuery 중심 구조)

### Hotkeys

- [react-hotkeys-hook](https://react-hotkeys-hook.vercel.app/): React용 선언적 단축키 훅
- [hotkeys-js](https://wangchujiang.com/hotkeys-js/): 의존성 없는 단축키 라이브러리
- [Mousetrap](https://craig.is/killing/mice): 성숙한 경량 단축키 라이브러리
- [TanStack Hotkeys](https://tanstack.com/hotkeys/latest): 타입 안전한 명령 및 단축키 시스템. 현재 alpha

## Data and APIs

### HTTP clients

- [Fetch API](https://developer.mozilla.org/docs/Web/API/Fetch_API): 브라우저와 최신 JavaScript 런타임의 표준 HTTP API
- [Axios](https://axios-http.com/): 브라우저와 Node.js에서 사용하는 Promise 기반 HTTP 클라이언트
- [Ky](https://github.com/sindresorhus/ky): Fetch 기반 경량 HTTP 클라이언트

### Type-safe APIs

- [tRPC](https://trpc.io/): TypeScript 기반 End-to-End 타입 안전 API 프레임워크

### OpenAPI code generation

- [Orval](https://orval.dev/): OpenAPI 스키마에서 TypeScript 클라이언트와 타입을 생성하는 도구
- [openapi-typescript](https://openapi-ts.dev/): OpenAPI 스키마에서 TypeScript 타입을 생성하는 도구

### GraphQL

- [GraphQL](https://graphql.org/): API를 위한 쿼리 언어와 실행 규격
- [Apollo Client](https://www.apollographql.com/docs/react): GraphQL 쿼리, 캐시 및 상태 관리 라이브러리
- [urql](https://nearform.com/open-source/urql/): 확장 가능한 경량 GraphQL 클라이언트

### Real-time communication

- [Socket.IO](https://socket.io/): 실시간 양방향 이벤트 통신 라이브러리
- [WebSocket](https://developer.mozilla.org/docs/Web/API/WebSockets_API): 클라이언트와 서버 간 양방향 실시간 통신 표준
- [Server-Sent Events](https://developer.mozilla.org/docs/Web/API/Server-sent_events): 서버에서 클라이언트로 이벤트를 전송하는 단방향 통신 표준

### API mocking

- [MSW](https://mswjs.io/): 네트워크 수준 API 모킹 라이브러리

### Forms

- [React Hook Form](https://react-hook-form.com/): React용 고성능 폼 상태 관리 라이브러리
- [TanStack Form](https://tanstack.com/form/latest): 타입 안전한 멀티 프레임워크 폼 라이브러리

### Schema validation

- [Zod](https://zod.dev/): TypeScript-first 스키마 검증 라이브러리
- [Valibot](https://valibot.dev/): 모듈식 스키마 검증 라이브러리

### Backend as a Service

- [Supabase](https://supabase.com/): PostgreSQL 기반 오픈소스 BaaS
- [Firebase](https://firebase.google.com/): 인증, NoSQL 데이터베이스 및 호스팅을 제공하는 BaaS

### ORM and query builders

- [Prisma](https://www.prisma.io/): Node.js와 TypeScript용 타입 안전 ORM
- [Drizzle ORM](https://orm.drizzle.team/): SQL과 가까운 TypeScript ORM
- [Kysely](https://kysely.dev/): 타입 안전한 SQL 쿼리 빌더

### Managed databases

- [Supabase Database](https://supabase.com/database): 인증과 Storage를 함께 사용할 수 있는 관리형 PostgreSQL
- [Neon](https://neon.com/): Serverless PostgreSQL 플랫폼
- [Turso](https://turso.tech/): libSQL 기반 Edge database 플랫폼
- [PlanetScale](https://planetscale.com/): MySQL과 PostgreSQL을 지원하는 관리형 데이터베이스 플랫폼
- [Cloudflare D1](https://developers.cloudflare.com/d1/): Cloudflare Workers와 통합되는 관리형 Serverless SQL database

### Object storage

- [Vercel Blob](https://vercel.com/docs/storage/vercel-blob): Vercel 애플리케이션용 객체 스토리지
- [Cloudflare R2](https://developers.cloudflare.com/r2/): S3 API와 호환되며 Egress fee가 없는 객체 스토리지
- [Supabase Storage](https://supabase.com/storage): Supabase Auth와 Row Level Security를 연동할 수 있는 객체 스토리지
- [Amazon S3](https://aws.amazon.com/s3/): 범용 객체 스토리지 서비스

## Backend and server

프런트엔드와 별도 서버를 처음부터 분리하기보다, 제품 요구사항이 생길 때 분리합니다. 일반적인 CRUD와 인증은 Full-stack framework 안에서 시작하고 Python 생태계, 독립적인 확장 또는 복잡한 도메인이 필요할 때 전용 API 서버를 둡니다.

### Full-stack backends

- [Next.js Route Handlers](https://nextjs.org/docs/app/getting-started/route-handlers): App Router 안에서 HTTP API를 구현하는 기본 방식
- [Next.js Server Functions and Actions](https://nextjs.org/docs/app/getting-started/updating-data): 폼 제출과 데이터 변경을 서버에서 처리하는 방식

### TypeScript API frameworks

- [Hono](https://hono.dev/): Web Standards 기반의 경량 멀티 런타임 웹 프레임워크
- [Fastify](https://fastify.dev/): 낮은 오버헤드와 플러그인 구조를 갖춘 Node.js 웹 프레임워크
- [NestJS](https://nestjs.com/): 모듈과 의존성 주입을 제공하는 대규모 Node.js 애플리케이션 프레임워크
- [Express](https://expressjs.com/): 생태계가 넓은 전통적인 Node.js 웹 프레임워크

### Python API frameworks

- [FastAPI](https://fastapi.tiangolo.com/): 타입 힌트와 OpenAPI를 활용하는 Python API 프레임워크
- [Django](https://www.djangoproject.com/): ORM, 관리자 화면과 인증을 포함하는 Python 웹 프레임워크
- [Flask](https://flask.palletsprojects.com/): 작은 서비스와 기존 프로젝트에 적합한 경량 Python 웹 프레임워크

### API design and reliability

- [REST](https://developer.mozilla.org/docs/Glossary/REST): 범용 HTTP API 설계 방식
- [Webhooks](https://www.svix.com/resources/webhooks/): 외부 서비스의 이벤트를 HTTP로 수신하는 통합 방식
- [Idempotency](https://docs.stripe.com/api/idempotent_requests): 재시도에도 중복 처리를 막는 요청 설계 원칙
- [OpenAPI](https://www.openapis.org/): HTTP API를 문서화하고 도구와 연결하는 표준 명세

## Background jobs and workflows

메일 발송, Webhook 재시도, 정기 동기화와 AI 처리처럼 요청 안에서 끝내기 어려운 작업에 사용합니다. 1인 운영에서는 직접 Queue worker를 관리하기 전에 관리형 서비스를 우선 검토합니다.

### Managed jobs and durable workflows

- [Inngest](https://www.inngest.com/): 이벤트 기반 Background job과 단계별 재시도를 제공하는 관리형 플랫폼
- [Trigger.dev](https://trigger.dev/): TypeScript 기반 장시간 작업과 Scheduled task 실행 플랫폼
- [Upstash Workflow](https://upstash.com/docs/workflow/getstarted): Serverless 환경용 Durable workflow SDK

### Queues and message delivery

- [Upstash QStash](https://upstash.com/docs/qstash/overall/getstarted): HTTP 기반 메시지 전달, 예약과 자동 재시도 서비스
- [Cloudflare Queues](https://developers.cloudflare.com/queues/): Cloudflare Workers와 통합되는 관리형 Message queue
- [BullMQ](https://docs.bullmq.io/): Redis 기반 Node.js Queue. Worker와 Redis 운영이 필요한 경우에 적합

### Scheduled jobs

- [Vercel Cron Jobs](https://vercel.com/docs/cron-jobs): Vercel Function을 정해진 일정에 호출하는 기능
- [Cloudflare Cron Triggers](https://developers.cloudflare.com/workers/configuration/cron-triggers/): Workers용 Scheduled event
- [GitHub Actions](https://docs.github.com/actions/using-workflows/events-that-trigger-workflows#schedule): 저장소 작업과 배치 스크립트를 위한 Scheduled workflow

## Email and notifications

### Transactional email

- [Resend](https://resend.com/): 개발자 중심의 Transactional email API
- [Postmark](https://postmarkapp.com/): Transactional email 전송과 전달 상태 추적 서비스
- [Amazon SES](https://aws.amazon.com/ses/): 대량 발송에 적합한 AWS 이메일 전송 서비스

### Email templates

- [React Email](https://react.email/): React 컴포넌트로 이메일 템플릿을 작성하는 도구

### Marketing email

- [Buttondown](https://buttondown.com/): 개인과 소규모 팀에 적합한 Newsletter 서비스
- [Mailchimp](https://mailchimp.com/): Audience 관리와 Marketing automation 플랫폼

### Push notifications

- [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging): 웹과 모바일 앱용 Cross-platform push messaging
- [OneSignal](https://onesignal.com/): Push, In-app message와 이메일을 제공하는 Customer messaging 플랫폼

## Cache and application infrastructure

### Managed cache and key-value storage

- [Upstash Redis](https://upstash.com/docs/redis/overall/getstarted): Serverless와 Edge 환경에 적합한 관리형 Redis 호환 서비스
- [Upstash for Redis on Vercel](https://vercel.com/marketplace/upstash): Vercel Marketplace에서 연결하는 관리형 Redis 호환 서비스
- [Cloudflare Workers KV](https://developers.cloudflare.com/kv/): 읽기 중심의 전역 분산 Key-value storage
- [Redis](https://redis.io/): Cache, session과 Queue에 사용하는 In-memory data store. 직접 운영할 때 관리 부담을 고려

### Common uses

- Cache: 느리거나 비용이 큰 조회 결과를 짧게 보관
- Rate limiting: 사용자, IP 또는 API key 단위로 요청량 제한
- Session storage: 여러 서버 인스턴스가 공유하는 로그인 상태 저장
- Distributed locks: 여러 작업이 같은 자원을 동시에 변경하지 않도록 조정

## Search

데이터가 많지 않거나 검색 요구가 단순하면 PostgreSQL에서 시작하고, 오타 허용·Faceting·관련도 조정이 중요해질 때 전용 검색 엔진을 도입합니다.

- [PostgreSQL Full Text Search](https://www.postgresql.org/docs/current/textsearch.html): 별도 검색 인프라 없이 시작하는 전문 검색
- [Meilisearch](https://www.meilisearch.com/docs): 빠른 도입과 오타 허용에 초점을 둔 오픈소스 검색 엔진
- [Typesense](https://typesense.org/docs/): 즉시 검색과 Faceting을 제공하는 오픈소스 검색 엔진
- [Algolia](https://www.algolia.com/doc/): 관리형 Search-as-a-Service
- [OpenSearch](https://opensearch.org/docs/latest/): 대규모 검색과 로그 분석을 위한 분산 검색 엔진
- [pgvector](https://github.com/pgvector/pgvector): PostgreSQL에 Vector similarity search를 추가하는 확장

## State management

### Server state

- [TanStack Query](https://tanstack.com/query/latest): 비동기 데이터 조회, 캐시 및 동기화 라이브러리
- [SWR](https://swr.vercel.app/): Vercel이 개발한 React용 데이터 페칭 및 캐싱 라이브러리

### Client state

- [Zustand](https://zustand.docs.pmnd.rs/): 간결한 React 전역 상태 관리 라이브러리
- [Redux Toolkit](https://redux-toolkit.js.org/): Redux 애플리케이션의 공식 권장 작성 방식
- [Jotai](https://jotai.org/): 원자 단위 React 상태 관리 라이브러리
- [Pinia](https://pinia.vuejs.org/): Vue의 공식 상태 관리 라이브러리
- [NgRx](https://ngrx.io/): RxJS와 Redux 패턴을 사용하는 Angular 상태 관리 프레임워크
- [NGXS](https://www.ngxs.io/): Angular용 상태 관리 프레임워크
- [Recoil](https://github.com/facebookexperimental/Recoil): 저장소가 아카이브된 React 상태 관리 라이브러리. 기존 프로젝트 참고용
- [Vuex](https://vuex.vuejs.org/): Vue 2와 기존 Vue 프로젝트 참고용 상태 관리 라이브러리

## Authentication

### Application-owned authentication

- [Better Auth](https://better-auth.com/): TypeScript 기반 인증·인가 프레임워크. 신규 프로젝트 우선 검토
- [Auth.js](https://authjs.dev/): Better Auth 팀이 유지보수하는 기존 JavaScript 인증 라이브러리
- [SimpleWebAuthn](https://simplewebauthn.dev/): WebAuthn과 Passkey 구현용 라이브러리
- [Lucia](https://lucia-auth.com/): deprecated된 인증 라이브러리. 기존 프로젝트 참고용

### Managed authentication

- [Clerk](https://clerk.com/): React와 Next.js에 친화적인 관리형 인증 플랫폼
- [Auth0](https://auth0.com/): 엔터프라이즈 기능을 제공하는 관리형 인증 플랫폼
- [Kinde](https://kinde.com/): 빠른 통합에 초점을 둔 인증 플랫폼

### BaaS-integrated authentication

- [Supabase Auth](https://supabase.com/auth): Supabase 데이터베이스 및 RLS와 통합되는 인증 서비스
- [Firebase Authentication](https://firebase.google.com/products/auth): Firebase 생태계와 통합되는 관리형 인증 서비스

### Passkey-first services

- [Corbado](https://www.corbado.com/): Passkey 도입과 전환에 특화된 인증 플랫폼
- [Hanko](https://www.hanko.io/): Passkey-first 인증을 제공하는 오픈소스 플랫폼

### Token handling

- [jose](https://github.com/panva/jose): JWT/JWS/JWE의 서명, 검증 및 암호화를 지원하는 라이브러리
- [jwt-decode](https://github.com/auth0/jwt-decode): JWT 내용을 디코딩하는 클라이언트 유틸리티. 서명이나 유효성을 검증하지 않음

## Development tools

### Code quality

- [ESLint](https://eslint.org/): Flat Config를 기본으로 사용하는 JavaScript 및 TypeScript 정적 분석 도구
- [Prettier](https://prettier.io/): 일관된 코드 스타일을 위한 포맷터
- [Biome](https://biomejs.dev/): Rust 기반 Linter 및 Formatter
- [Oxlint](https://oxc.rs/docs/guide/usage/linter.html): Oxc 프로젝트의 고성능 JavaScript 및 TypeScript Linter

### JavaScript runtimes

- [Node.js](https://nodejs.org/): 서버와 개발 도구에서 널리 사용하는 JavaScript 런타임
- [Bun](https://bun.com/): 런타임, 패키지 매니저, 번들러 및 테스트 도구를 포함한 JavaScript 툴킷

### Package managers

- [pnpm](https://pnpm.io/): 저장 공간 효율성과 워크스페이스 기능에 강한 JavaScript 패키지 관리자
- [npm](https://www.npmjs.com/): Node.js에 기본 포함되는 JavaScript 패키지 관리자
- [Yarn](https://yarnpkg.com/): Plug'n'Play과 워크스페이스 기능을 제공하는 패키지 관리자

### Python project tools

- [uv](https://docs.astral.sh/uv/): Python version, 가상 환경, 의존성과 Lockfile을 함께 관리하는 빠른 프로젝트 도구
- [Ruff](https://docs.astral.sh/ruff/): Python Linter와 Formatter
- [Pyright](https://microsoft.github.io/pyright/): Python 정적 타입 검사기
- [Poetry](https://python-poetry.org/): Python 의존성과 패키징 관리 도구

### Build tools

- [Vite](https://vite.dev/): Rolldown과 Oxc 기반 프런트엔드 빌드 도구 (v7 이하: esbuild + Rollup 조합 사용)
- [Turbopack](https://nextjs.org/docs/app/api-reference/turbopack): Next.js에 통합된 Rust 기반 번들러
- [Rspack](https://rspack.rs/): Webpack 생태계와 호환되는 Rust 기반 번들러
- [Webpack](https://webpack.js.org/): 광범위한 생태계와 설정 유연성을 갖춘 성숙한 번들러
- [Rolldown](https://rolldown.rs/): Rollup 호환성을 지향하는 Rust 기반 번들러
- [esbuild](https://esbuild.github.io/): Go 기반의 고성능 JavaScript 번들러와 변환기
- [Rollup](https://rollupjs.org/): 라이브러리 패키징과 ES module 최적화에 강한 번들러

### Monorepo tools

- [Turborepo](https://turborepo.com/): JavaScript와 TypeScript 모노레포 빌드 시스템
- [Nx](https://nx.dev/): 다중 언어와 프레임워크를 지원하는 모노레포 도구
- [pnpm workspaces](https://pnpm.io/workspaces): pnpm 내장 워크스페이스 기능

### Release automation

- [Changesets](https://github.com/changesets/changesets): 모노레포 버전 및 변경 기록 관리 도구
- [release-please](https://github.com/googleapis/release-please): Conventional Commits 기반 릴리스 PR 자동화 도구

### Component development

- [Storybook](https://storybook.js.org/): UI 컴포넌트 독립 개발, 테스트 및 문서화 도구
- [Bit](https://bit.dev/): 컴포넌트 단위 개발과 공유를 위한 플랫폼

## Testing

### Unit and integration testing

- [Vitest](https://vitest.dev/): Vite 생태계와 통합되는 테스트 프레임워크
- [Jest](https://jestjs.io/): JavaScript와 TypeScript 테스트 프레임워크
- [pytest](https://docs.pytest.org/): Python 테스트 프레임워크

### Component testing

- [Testing Library](https://testing-library.com/): 사용자 관점의 UI 테스트 도구

### End-to-end testing

- [Playwright](https://playwright.dev/): 크로스 브라우저 E2E 및 웹 자동화 도구
- [Cypress](https://www.cypress.io/): 대화형 개발 경험을 제공하는 E2E 테스트 도구

### API and load testing

- [Bruno](https://www.usebruno.com/): API collection을 저장소에서 관리할 수 있는 오픈소스 API client
- [Postman](https://www.postman.com/): API 설계, 테스트와 협업 플랫폼
- [k6](https://grafana.com/docs/k6/latest/): 코드 기반 Load testing 도구

## Deployment and hosting

### CI/CD automation

- [GitHub Actions](https://github.com/features/actions): GitHub 통합 CI/CD 자동화
- [Jenkins](https://www.jenkins.io/): 자체 구축형 CI/CD 자동화 서버
- [Travis CI](https://www.travis-ci.com/): 클라우드 CI/CD 서비스

### Containers

- [Docker](https://www.docker.com/): 컨테이너 기반 애플리케이션 패키징 및 실행

### Serverless deployment

- [SST](https://sst.dev/): AWS 기반 풀스택 및 Serverless 애플리케이션 개발 도구
- [Serverless Framework](https://www.serverless.com/): Serverless 애플리케이션 배포 프레임워크

### Frontend and full-stack platforms

- [Vercel](https://vercel.com/): Next.js 및 프런트엔드 애플리케이션에 최적화된 플랫폼
- [Cloudflare Workers Static Assets](https://developers.cloudflare.com/workers/static-assets/): Cloudflare의 신규 정적·SPA·풀스택 프로젝트 권장 배포 방식
- [Netlify](https://www.netlify.com/): 정적 사이트와 풀스택 웹 애플리케이션 플랫폼
- [Firebase App Hosting](https://firebase.google.com/products/app-hosting): 풀스택 웹 애플리케이션 호스팅
- [AWS Amplify](https://aws.amazon.com/amplify/): AWS 기반 풀스택 웹 개발 및 호스팅
- [Firebase Hosting](https://firebase.google.com/products/hosting): 정적 사이트와 SPA 호스팅
- [Cloudflare Pages](https://pages.cloudflare.com/): 기존 Pages 프로젝트를 위한 정적 및 웹 애플리케이션 호스팅

### Application and container platforms

- [Render](https://render.com/): 백엔드, 데이터베이스 및 풀스택 애플리케이션 플랫폼
- [Fly.io](https://fly.io/): 컨테이너 기반 글로벌 애플리케이션 플랫폼
- [Google Cloud Run](https://cloud.google.com/run): 컨테이너 기반 Serverless 실행 환경

### Cloud infrastructure

- [Amazon S3](https://aws.amazon.com/s3/): 정적 파일과 빌드 결과물을 저장하는 객체 스토리지
- [Amazon CloudFront](https://aws.amazon.com/cloudfront/): 정적·동적 콘텐츠를 전송하는 글로벌 CDN

### Domain registrars

#### International

- [Cloudflare Registrar](https://www.cloudflare.com/products/registrar/): 원가 기반 가격 정책과 Cloudflare DNS 통합을 제공하는 등록기관
- [Porkbun](https://porkbun.com/products/domains): 투명한 가격과 무료 WHOIS 개인정보 보호를 제공하는 등록기관
- [Namecheap](https://www.namecheap.com/domains/): 도메인과 관련 웹 서비스를 함께 제공하는 등록기관

#### South Korea

- [가비아](https://www.gabia.com/): 국내 결제와 증빙이 편리한 도메인 등록기관
- [호스팅케이알](https://www.hosting.kr/domain/search): 국내 도메인 등록 및 호스팅 서비스

### DNS

- [Cloudflare DNS](https://www.cloudflare.com/dns/): CDN과 보안 기능을 함께 제공하는 글로벌 DNS 서비스
- [Amazon Route 53](https://aws.amazon.com/route53/): AWS의 고가용성 DNS 및 트래픽 라우팅 서비스

### Development DNS

- [DuckDNS](https://www.duckdns.org/): 개발과 개인 프로젝트용 무료 Dynamic DNS
- [sslip.io](https://sslip.io/): IP 주소가 포함된 호스트명을 자동으로 해석하는 개발용 DNS
- [nip.io](https://nip.io/): 로컬 및 테스트 환경용 와일드카드 DNS

### DNS diagnostics

- [DNSChecker](https://dnschecker.org/): 전 세계 DNS 레코드 전파 상태 확인 도구
- [ICANN Lookup](https://lookup.icann.org/): 도메인 등록 정보 조회 도구
- [who.is](https://who.is/): 도메인 등록기관, 만료일 및 공개 WHOIS 정보 조회 도구

## Operations

1인 운영에서는 도구의 기능 수보다 장애를 빨리 발견하고 적은 단계로 복구할 수 있는지가 중요합니다. 배포 전에 아래 항목의 소유 위치와 복구 절차를 정합니다.

### Secrets and configuration

- Hosting platform environment variables: 작은 프로젝트에서 가장 단순한 기본 선택
- [Doppler](https://www.doppler.com/): 여러 환경과 서비스의 Secret을 중앙에서 관리하는 플랫폼
- [1Password Secrets Automation](https://developer.1password.com/docs/secrets-automation/): 1Password vault의 Secret을 CI와 애플리케이션에 연결하는 도구
- 원칙: Secret을 저장소와 클라이언트 번들에 넣지 않고, 개발·Preview·Production 값을 분리하며 교체 절차를 기록

### Uptime and status

- [Better Stack Uptime](https://betterstack.com/uptime): Uptime monitoring, On-call과 Status page 서비스
- [UptimeRobot](https://uptimerobot.com/): 간단한 HTTP, Keyword와 Port monitoring 서비스
- [Checkly](https://www.checklyhq.com/): Playwright 기반 Synthetic monitoring과 API check 플랫폼

### Backups and recovery

- Managed database의 자동 Backup과 Point-in-time recovery 제공 여부를 먼저 확인
- [pg_dump](https://www.postgresql.org/docs/current/app-pgdump.html): PostgreSQL의 논리 Backup 도구
- Database뿐 아니라 Object storage, DNS, 환경 변수와 외부 서비스 설정의 복구 방법도 기록
- Backup 생성 여부가 아니라 별도 환경에서 실제 Restore가 되는지 정기적으로 확인

### Feature flags

- [PostHog Feature Flags](https://posthog.com/docs/feature-flags): Product analytics와 함께 사용하는 Feature flag
- [Flags SDK](https://flags-sdk.dev/): Next.js와 여러 Provider를 연결하는 Feature flag 표준화 도구
- [Unleash](https://docs.getunleash.io/): 자체 호스팅이 가능한 오픈소스 Feature management 플랫폼

### Cost controls

- Hosting, database, email, storage와 AI provider에 Budget alert를 설정
- 사용량 기반 서비스는 Rate limit, 월별 상한과 이상 사용량 알림을 함께 구성
- Preview deployment와 사용하지 않는 데이터베이스·스토리지·로그의 정리 주기를 결정

## Quality, security, and observability

### Performance

#### Web Vitals and performance audits

- [web.dev Performance](https://web.dev/performance/): Core Web Vitals와 웹 성능 가이드
- [PageSpeed Insights](https://pagespeed.web.dev/): 실제 및 실험실 성능 진단
- [Lighthouse](https://developer.chrome.com/docs/lighthouse): 성능, 접근성, SEO 및 모범 사례 감사 도구
- [WebPageTest](https://www.webpagetest.org/): 다양한 환경의 상세 웹 성능 분석

#### Bundle size and optimization

- [Bundlephobia](https://bundlephobia.com/): npm 패키지 번들 크기 확인 도구
- [`@next/bundle-analyzer`](https://www.npmjs.com/package/@next/bundle-analyzer): Next.js 애플리케이션의 번들 구성 시각화
- [webpack-bundle-analyzer](https://www.npmjs.com/package/webpack-bundle-analyzer): Webpack 번들 구성과 크기 시각화

### Accessibility

- [WCAG](https://www.w3.org/WAI/standards-guidelines/wcag/): 웹 접근성 국제 지침
- [axe-core](https://github.com/dequelabs/axe-core): 자동화된 접근성 검사 엔진
- [Storybook Accessibility](https://storybook.js.org/docs/writing-tests/accessibility-testing): 컴포넌트 접근성 테스트
- [eslint-plugin-jsx-a11y](https://github.com/jsx-eslint/eslint-plugin-jsx-a11y): JSX 접근성 규칙 검사

### Security

#### Guides and browser security

- [OWASP Web Security Testing Guide](https://owasp.org/www-project-web-security-testing-guide/): 웹 보안 테스트 지침
- [Content Security Policy](https://developer.mozilla.org/docs/Web/HTTP/CSP): 스크립트와 리소스 실행 출처를 제한하는 브라우저 보안 정책
- [Trusted Types](https://developer.mozilla.org/docs/Web/API/Trusted_Types_API): DOM XSS 위험을 줄이는 브라우저 API
- [DOMPurify](https://github.com/cure53/DOMPurify): 신뢰할 수 없는 HTML을 정화하는 라이브러리

#### Server and integration security

- Authentication과 authorization을 구분하고, 모든 데이터 변경 작업에서 서버가 권한을 다시 확인
- Cookie 기반 인증은 `Secure`, `HttpOnly`, `SameSite`와 [CSRF](https://owasp.org/www-community/attacks/csrf) 방어를 함께 구성
- [CORS](https://developer.mozilla.org/docs/Web/HTTP/CORS)는 필요한 Origin, Method와 Header만 허용
- 결제·인증·메일 등 외부 Webhook은 서명을 검증하고, Idempotency key로 중복 처리를 방지
- 공개 API와 비용이 발생하는 작업에는 Rate limit과 입력 크기 제한을 적용

#### Dependencies and supply chain

- [Dependabot](https://docs.github.com/code-security/dependabot): 의존성 보안 업데이트와 취약점 알림
- [`npm audit`](https://docs.npmjs.com/cli/commands/npm-audit): npm 의존성의 알려진 취약점 검사
- CI에서는 Lockfile을 고정하고 최소 권한의 짧은 수명 Credential을 사용

### Observability

- [Sentry](https://sentry.io/): 오류 추적과 애플리케이션 성능 모니터링
- [OpenTelemetry](https://opentelemetry.io/): 벤더 중립적인 로그, 메트릭 및 트레이스 표준
- [Web Vitals](https://github.com/GoogleChrome/web-vitals): 실제 사용자 환경의 Core Web Vitals 측정 라이브러리
- 운영 원칙: 요청 ID와 배포 버전을 로그·오류에 포함하고, 사용자 정보와 Secret은 기록하지 않으며 보관 기간을 설정

### Browser compatibility

- [web.dev Baseline](https://web.dev/baseline): 브라우저 간 웹 기능 지원 상태 기준
- [Browserslist](https://browsersl.ist/): 지원 브라우저 범위를 도구 간 공유하는 설정
- [Can I Use](https://caniuse.com/): 웹 플랫폼 기능별 브라우저 지원 현황

## Product integrations

### SEO & GEO

#### Guides and standards

- [sitemaps.org](https://www.sitemaps.org/): sitemap.xml 프로토콜 규격
- [JSON-LD](https://www.w3.org/TR/json-ld11/): 검색엔진과 AI 도구가 콘텐츠의 구조와 의미를 이해하도록 돕는 연결 데이터 형식
- [`robots.txt`](https://www.rfc-editor.org/rfc/rfc9309): 검색 및 AI 크롤러의 접근 정책을 설정하는 표준
- [Google Search Central](https://developers.google.com/search): Google의 공식 검색 최적화 문서
- [The Beginner's Guide to SEO](https://moz.com/beginners-guide-to-seo): Moz의 종합 SEO 입문 가이드
- [llms.txt](https://llmstxt.org/): AI 에이전트가 사이트 정보를 읽기 쉽게 제공하기 위한 확산 중인 제안 규격

#### Frameworks and libraries

- Next.js [Metadata API](https://nextjs.org/docs/app/getting-started/metadata-and-og-images): App Router의 기본 메타데이터 및 Open Graph 관리 방식
- [next-seo](https://github.com/garmeeh/next-seo): 기존 Next.js 프로젝트에서 메타데이터와 Open Graph 설정을 관리하는 보조 라이브러리
- [next-sitemap](https://github.com/iamvishnusankar/next-sitemap): Next.js용 sitemap.xml 및 robots.txt 생성 도구
- [schema-dts](https://github.com/google/schema-dts): Schema.org JSON-LD용 TypeScript 타입

#### Search engine consoles

- [Google Search Console](https://search.google.com/search-console/): Google 검색 색인과 검색 성과 관리 도구
- [네이버 서치어드바이저](https://searchadvisor.naver.com/): 네이버 검색 색인과 사이트 진단 도구
- [Bing Webmaster Tools](https://www.bing.com/webmasters/about): Bing 검색 색인 및 성과 관리 도구

#### AI crawler monitoring

- [Cloudflare AI Crawl Control](https://developers.cloudflare.com/ai-crawl-control/): AI 크롤러 접근 현황을 분석하고 크롤러별 정책을 관리하는 서비스 (이전 명칭: AI Audit)

#### Debuggers

- [SEO Site Checkup](https://seositecheckup.com/): 웹사이트의 기술적 SEO 진단 서비스
- [Google Rich Results Test](https://search.google.com/test/rich-results): 구조화 데이터와 리치 결과 유효성 검사 도구
- [OpenGraph.xyz](https://www.opengraph.xyz/): Open Graph 메타데이터 미리보기 도구
- [Meta Sharing Debugger](https://developers.facebook.com/tools/debug/): Meta 서비스의 공유 정보 검사 및 캐시 갱신 도구
- [카카오 URL 디버거](https://developers.kakao.com/tool/debugger/sharing): 카카오톡 공유 메타데이터 검사 및 캐시 갱신 도구

### Analytics

#### Web analytics

- [Google Analytics](https://analytics.google.com/): 웹과 앱의 트래픽 및 전환 분석 서비스
  - [GA Dev Tools](https://ga-dev-tools.google/ga4/): Google Analytics 데모와 디버깅 유틸리티
- [Plausible](https://plausible.io/): 개인정보 보호 중심의 경량 웹 분석 서비스
- [Statcounter](https://statcounter.com/): 실시간 방문자와 트래픽 통계 서비스

#### Product analytics

- [Amplitude](https://amplitude.com/): 코호트, 퍼널 및 사용자 행동 분석 플랫폼
- [Mixpanel](https://mixpanel.com/): 이벤트 기반 제품 분석 플랫폼
- [PostHog](https://posthog.com/): 분석, 세션 재생 및 기능 플래그를 제공하는 오픈소스 플랫폼

#### Heatmaps and session replay

- [Microsoft Clarity](https://clarity.microsoft.com/): 무료 세션 재생과 히트맵 서비스
- [Hotjar](https://www.hotjar.com/): 세션 재생, 히트맵 및 사용자 피드백 도구

#### Tag management

- [Google Tag Manager](https://tagmanager.google.com/): 마케팅 및 분석 태그 관리 도구

#### Attribution and marketing pixels

- [Airbridge](https://www.airbridge.io/): 웹과 앱의 마케팅 기여도 측정 플랫폼
- [Meta Pixel](https://www.facebook.com/business/tools/meta-pixel): Meta 광고 전환 측정 및 리타게팅 도구
- [카카오 픽셀 & SDK](https://business.kakao.com/info/pixelsdk/): 카카오 광고 전환 및 사용자 행동 측정 도구

#### Consent and privacy

- [Google Consent Mode](https://developers.google.com/tag-platform/security/guides/consent): 사용자의 동의 상태를 Google tag 동작에 반영하는 방식
- [Klaro](https://klaro.org/): 자체 호스팅이 가능한 오픈소스 Consent manager
- [Cookiebot](https://www.cookiebot.com/): Cookie scan과 Consent banner를 제공하는 관리형 플랫폼
- 원칙: 서비스 지역과 수집 정보에 맞는 개인정보 처리방침을 작성하고, 동의 전에는 불필요한 분석·광고 Script를 실행하지 않음

### Payments and monetization

#### Global payments

- [Stripe](https://stripe.com/): 개발자 친화적인 글로벌 결제 및 구독 플랫폼
  - [Link](https://link.com/): Stripe가 제공하는 원클릭 결제 서비스
- [PayPal](https://www.paypal.com/): 글로벌 온라인 결제 및 간편결제 서비스

#### Korean payments

- [Toss Payments](https://www.tosspayments.com/): 국내 결제 API와 결제 UI를 제공하는 PG 서비스
- [PortOne](https://developers.portone.io/): 여러 PG사와 간편결제를 단일 API로 연결하는 결제 오케스트레이션 서비스
- [KG이니시스](https://www.inicis.com/): 국내 전자결제 서비스
- [NHN KCP](https://www.kcp.co.kr/): 국내 온·오프라인 전자결제 서비스

#### Subscriptions and Merchant of Record

- [Paddle](https://www.paddle.com/): SaaS 결제, 구독, 세금 처리를 제공하는 Merchant of Record
- [Lemon Squeezy](https://www.lemonsqueezy.com/): 디지털 제품과 SaaS용 결제 및 Merchant of Record
- [RevenueCat](https://www.revenuecat.com/): 모바일 앱과 웹 구독 관리 플랫폼

#### Sponsorship

- [GitHub Sponsors](https://github.com/sponsors): 오픈소스 개발자 후원 플랫폼
- [Patreon](https://www.patreon.com/): 정기 멤버십과 창작자 후원 플랫폼
- [Buy Me a Coffee](https://buymeacoffee.com/): 창작자용 일회성·정기 후원 서비스
- [Ko-fi](https://ko-fi.com/): 후원, 멤버십 및 디지털 상품 판매 서비스

### Advertising

#### Web ad networks

- [Google AdSense](https://adsense.google.com/): 웹사이트용 Google 광고 수익화 플랫폼
- [kakaoAdFit](https://adfit.kakao.com/): 카카오의 국내 웹·앱 광고 플랫폼
- [Taboola](https://www.taboola.com/): 콘텐츠 추천 기반 네이티브 광고 플랫폼
- [Outbrain](https://www.outbrain.com/): 콘텐츠 추천 기반 네이티브 광고 플랫폼

#### In-app ad networks

- [Google AdMob](https://admob.google.com/): 모바일 앱용 Google 광고 플랫폼
- [AppLovin MAX](https://www.applovin.com/max/): 모바일 광고 미디에이션 플랫폼
- [Unity LevelPlay](https://unity.com/products/levelplay): 모바일 앱과 게임용 광고 미디에이션 플랫폼

#### Affiliate and commerce ads

- [쿠팡 파트너스](https://partners.coupang.com/): 상품 링크를 통한 국내 제휴 마케팅 프로그램
- [Amazon Associates](https://affiliate-program.amazon.com/): Amazon 상품을 위한 글로벌 제휴 마케팅 프로그램

#### Ad infrastructure

- [Google Publisher Tag](https://developers.google.com/publisher-tag): Google Ad Manager 광고를 웹에 표시하고 제어하는 라이브러리
- [Prebid.js](https://prebid.org/product-suite/prebidjs/): 브라우저 기반 Header Bidding 오픈소스 라이브러리

### Maps and location

#### Commercial map platforms

- [Google Maps Platform](https://developers.google.com/maps): 글로벌 지도, 장소 검색 및 경로 API
- [Kakao Maps](https://apis.map.kakao.com/): 국내 장소 검색과 지도 API
- [Naver Maps](https://www.ncloud.com/product/applicationService/maps): 국내 지도, 장소 및 경로 API

#### Vector and open-source maps

- [Mapbox](https://www.mapbox.com/): 커스텀 벡터 지도와 위치 서비스 플랫폼
- [Leaflet](https://leafletjs.com/): 오픈 지도 타일과 함께 사용하는 경량 2D 지도 라이브러리

#### Geospatial visualization

- [deck.gl](https://deck.gl/): WebGL 기반 대규모 지리 데이터 시각화 프레임워크

## Data visualization

### Charts

- [Chart.js](https://www.chartjs.org/): 사용하기 쉬운 Canvas 기반 차트 라이브러리
- [Recharts](https://recharts.org/): React용 컴포넌트 기반 차트 라이브러리
- [Apache ECharts](https://echarts.apache.org/): 다양한 차트와 대규모 데이터 렌더링을 지원하는 라이브러리
- [D3](https://d3js.org/): 데이터 기반의 커스텀 시각화를 만드는 로우레벨 라이브러리
- [Plotly](https://plotly.com/javascript/): 과학·통계 및 3D 시각화에 강한 인터랙티브 차트 라이브러리
- [AG Charts](https://www.ag-grid.com/charts/): 엔터프라이즈 애플리케이션용 차트 라이브러리

### Graphics

- [Three.js](https://threejs.org/): 웹 3D 그래픽을 위한 WebGL 라이브러리
- [PixiJS](https://pixijs.com/): 고성능 2D WebGL 렌더링 엔진

## Cross-platform development

- [React Native](https://reactnative.dev/): React 기반 네이티브 애플리케이션 프레임워크
- [Flutter](https://flutter.dev/): Dart 기반 멀티플랫폼 UI 프레임워크
- [Ionic](https://ionicframework.com/): 웹 기술과 WebView를 활용하는 크로스플랫폼 앱 프레임워크

## Developer services

- [CodePen](https://codepen.io/): 프런트엔드 예제 작성과 공유를 위한 브라우저 기반 편집기
- [JSFiddle](https://jsfiddle.net/): HTML, CSS 및 JavaScript를 실행하고 공유하는 온라인 편집기
- [Transform](https://transform.tools/): 개발 데이터 및 코드 형식 변환 도구
- [Bitly](https://bitly.com/): 단축 URL 서비스
- [Lorem Picsum](https://picsum.photos/): 플레이스홀더 이미지 서비스

## AI development

- [AI SDK](https://ai-sdk.dev/): AI 애플리케이션과 에이전트 개발용 TypeScript 툴킷
- [LM Studio](https://lmstudio.ai/): 로컬 AI 모델 실행 도구
- [Hugging Face](https://huggingface.co/): AI 모델, 데이터셋 및 애플리케이션 커뮤니티
- [OpenRouter](https://openrouter.ai/): 여러 AI 모델을 통합해 제공하는 API 플랫폼

## Git and releases

### Version control

- [Git](https://git-scm.com/): 분산 버전 관리 시스템
- [Git Cheat Sheet](https://git-scm.com/cheat-sheet): 자주 사용하는 Git 명령 요약

### Branching workflows

- [GitHub Flow](https://docs.github.com/get-started/using-github/github-flow): 짧은 브랜치와 Pull Request 중심의 개발 흐름
- [Trunk Based Development](https://trunkbaseddevelopment.com/): 작은 변경을 자주 통합하는 메인 브랜치 중심 개발 방식
- [Git-flow](https://nvie.com/posts/a-successful-git-branching-model/): 장기 브랜치를 사용하는 전통적 모델. 기존 프로젝트 참고용

### Versioning and commit conventions

- [Semantic Versioning](https://semver.org/): 공개 API 변경에 따른 버전 규칙
- [Conventional Commits](https://www.conventionalcommits.org/): 커밋 메시지 규약

### README badges

- [Shields.io](https://shields.io/): 저장소와 프로젝트 상태를 표시하는 배지 생성 서비스
- [Badgen](https://badgen.net/): 빠르고 간결한 SVG 배지 생성 서비스
