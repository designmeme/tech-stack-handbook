# Web Tech Stack Handbook 2026

**English** | [한국어](README.ko.md)

> A practical 2026 web development tech stack guide for solo builders—from frontend and backend to deployment, analytics, and operations.

This handbook organizes modern tools and services for building web products across frontend development, full-stack architecture, databases, deployment, and product operations.

Recommendations consider not only adoption in new projects, but also **development speed, operational overhead, cost, and scalability**.

## How this handbook is organized

Tools that serve the same purpose are generally ordered by the following criteria. Download counts and cumulative user numbers are not the sole considerations;
**adoption trends and suitability for new projects** take priority.

1. Suitability for solo builders who need to ship and operate quickly
2. Adoption and momentum in new projects
3. Ecosystem maturity and maintenance stability
4. Fit for specialized requirements or larger organizations
5. Operationally heavy, experimental, or legacy status

Tools with different roles are not ranked directly against one another. Each list is reviewed regularly as the ecosystem changes.

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

- [HTML](https://html.spec.whatwg.org/): The standard markup language for web documents
- [CSS](https://www.w3.org/Style/CSS/): The standard styling and layout language for the web
- [JavaScript](https://developer.mozilla.org/docs/Web/JavaScript): The standard programming language of browsers and web servers
- [TypeScript](https://www.typescriptlang.org/): JavaScript with static types and the default choice for many modern web projects
- [Web APIs](https://developer.mozilla.org/docs/Web/API): Standard browser APIs including DOM, Fetch, Storage, and Workers

### UI frameworks and libraries

- [React](https://react.dev/): Component-based UI library
- [Vue](https://vuejs.org/): Progressive UI framework
- [Angular](https://angular.dev/): Integrated framework with routing, forms, and dependency injection
  - [RxJS](https://rxjs.dev/): Reactive programming library for asynchronous event streams
  - [ReactiveX](https://reactivex.io/): Repository Programming API and project introduction of language implementation
  - [Learn RxJS](https://www.learnrxjs.io/): Learning materials describing RxJS operators and patterns
- [Svelte](https://svelte.dev/): Compiler-based UI framework
- [jQuery](https://jquery.com/): DOM library primarily relevant to legacy applications

### Full-stack and meta-frameworks

- [Next.js](https://nextjs.org/): Full-stack React framework
- [React Router](https://reactrouter.com/): React routing and full-stack web framework
- [Nuxt](https://nuxt.com/): Full-stack Vue framework
- [SvelteKit](https://svelte.dev/docs/kit): Full-stack Svelte framework
- [Astro](https://astro.build/): Multi-framework platform well suited to content-focused sites

### Static site and documentation generators

Reference: [Jamstack Generators](https://jamstack.org/generators/)

- [Docusaurus](https://docusaurus.io/): React and MDX documentation generator
- [Hugo](https://gohugo.io/): Fast Go-based static site generator
- [Gatsby](https://www.gatsbyjs.com/): Mature React and GraphQL static-site framework

## Content and documentation

### Headless CMS

Reference: [Jamstack Headless CMS](https://jamstack.org/headless-cms/)

- [Strapi](https://strapi.io/): Open-source Node.js headless CMS
- [Sanity](https://www.sanity.io/): SaaS CMS with custom schemas and real-time collaboration
- [Payload](https://payloadcms.com/): Code-first TypeScript CMS with strong Next.js integration
- [Contentful](https://www.contentful.com/): Enterprise-oriented SaaS CMS
- [Ghost](https://ghost.org/): Publishing, blogging, and newsletter platform

### Markdown and MDX

- [MDX](https://mdxjs.com/): Markdown with embedded JSX components
- [MDXEditor](https://mdxeditor.dev/): React-based WYSIWYG MDX Editor

### Rich-text editors

- [Tiptap](https://tiptap.dev/): Headless rich-text editor built on ProseMirror
- [Lexical](https://lexical.dev/): Extensible rich-text editor framework from Meta

### Syntax highlighting

- [Shiki](https://shiki.style/): Syntax highlighter using VS Code grammars and themes
- [Prism](https://prismjs.com/): Lightweight syntax-highlighting library for browsers

### Diagrams and code images

- [Mermaid](https://mermaid.js.org/): Text-based diagrams and sequence charts
- [Carbon](https://carbon.now.sh/): Create a source code image

### Documentation hosting

- [Read the Docs](https://about.readthedocs.com/): Documentation build and hosting platform

### Feeds

- [W3C Feed Validation Service](https://validator.w3.org/feed/): RSS and Atom feed validator
- [Feeder](https://feeder.co/): RSS feed reader and notification service
- [FeedBurner](https://feedburner.google.com/): Rescheduling service only for core feed management functions

## Styling and UI

### CSS frameworks

- [Tailwind CSS](https://tailwindcss.com/): Utility-first CSS framework with CSS-first configuration
- [Bootstrap](https://getbootstrap.com/): CSS framework with ready-made components

### CSS preprocessors

- [Sass](https://sass-lang.com/): CSS preprocessor

### CSS-in-JS and build-time styling

- [styled-components](https://styled-components.com/): Runtime CSS-in-JS for React
- [Emotion](https://emotion.sh/): Flexible runtime CSS-in-JS library
- [vanilla-extract](https://vanilla-extract.style/): TypeScript-based zero-runtime styling
- [Panda CSS](https://panda-css.com/): Type-safe CSS-in-JS with build-time extraction

### Headless components

- [Radix UI](https://www.radix-ui.com/): Accessible headless React components
- [Headless UI](https://headlessui.com/): Headless React and Vue components from Tailwind Labs
- [Base UI](https://base-ui.com/): Headless React components from the MUI team

### Styled component libraries

- [shadcn/ui](https://ui.shadcn.com/): Source-owned components built with Tailwind CSS and Radix UI or Base UI
- [Material UI](https://mui.com/): Material Design React component library
- [Ant Design](https://ant.design/): React UI system popular for admin and enterprise products
- [daisyUI](https://daisyui.com/): Component library implemented as a Tailwind CSS plugin
- [Angular Material](https://material.angular.dev/): Material Design Components for Angular
- [PrimeNG](https://primeng.org/): Angular UI component collection
- [spartan/ui](https://www.spartan.ng/): Angular and Tailwind CSS based UI component

### Admin application frameworks

- [React-admin](https://marmelab.com/react-admin/): React framework for data-driven admin applications
- [Refine](https://refine.dev/): Headless React framework for admin screen and internal tools

### Admin templates

- [shadcn/ui Templates](https://www.shadcn.io/template): shadcn/ui-based application template collection
- [Shadcn Admin](https://www.shadcn.io/template/satnaing-shadcn-admin): shadcn/ui based manager dashboard template
- [Metronic](https://keenthemes.com/metronic): Commercial admin interface template
- [TailAdmin](https://tailadmin.com/): Tailwind CSS Based Dashboard Template

### Icons

- [Lucide](https://lucide.dev/): Consistent open-source SVG icon set
- [Font Awesome](https://fontawesome.com/): Free and easy-to-use icon library
- [Bootstrap Icons](https://icons.getbootstrap.com/): Open source SVG icon collection with Bootstrap team

### Fonts

- [Google Fonts](https://fonts.google.com/): Web font discovery and delivery service
- [Inter](https://rsms.me/inter/): Open source font optimized for screen and user interface

### Animation

#### UI and component animation

- [Motion](https://motion.dev/): UI animation library for React and JavaScript
- [AutoAnimate](https://auto-animate.formkit.com/): A tool to automatically create layout changes

#### Timeline and scroll animation

- [GSAP](https://gsap.com/): Timeline and scroll animation platform

#### Vector animation

- [Lottie](https://airbnb.io/lottie/): JSON-based vector animation format and renderer
- [LottieFiles](https://lottiefiles.com/): Lottie animation asset search, production and management platform
- [dotLottie](https://dotlottie.io/): Stringing and compressing Lottie assets`.lottie` Scots Gaelic
- [`@lottiefiles/dotlottie-react`](https://www.npmjs.com/package/@lottiefiles/dotlottie-react): latest dotLottie player for React

#### Number and text animation

- [CountUp.js](https://inorganik.github.io/CountUp.js/): Number-counting animation library

### Gestures

- [use-gesture](https://use-gesture.netlify.app/): Touch, drag, pinch and scroll gesture hook for React
- [AlloyFinger](https://github.com/AlloyTeam/AlloyFinger): Lightweight multitouch gesture library that does not depend on the framework
- [Hammer.js](https://hammerjs.github.io/): Established touch-gesture library primarily maintained for existing projects

### Data tables

- [TanStack Table](https://tanstack.com/table/latest): Headless data-table library
- [AG Grid](https://www.ag-grid.com/): Data grid for large datasets and enterprise requirements
- [MUI X Data Grid](https://mui.com/x/react-data-grid/): Data Grid in MUI Ecosystem
- [DataTables](https://datatables.net/): TypeScript-based standalone table library (v2 and below: jQuery center structure)

### Hotkeys

- [react-hotkeys-hook](https://react-hotkeys-hook.vercel.app/): Declarative keyboard shortcuts for React
- [hotkeys-js](https://wangchujiang.com/hotkeys-js/): Dependency-free keyboard shortcut library
- [Mousetrap](https://craig.is/killing/mice): Mature lightweight keyboard shortcut library
- [TanStack Hotkeys](https://tanstack.com/hotkeys/latest): Type safe command and shortcut system. Current alpha

## Data and APIs

### HTTP clients

- [Fetch API](https://developer.mozilla.org/docs/Web/API/Fetch_API): Standard HTTP API in browsers and modern JavaScript runtimes
- [Axios](https://axios-http.com/): Promise-based HTTP client for browsers and Node.js
- [Ky](https://github.com/sindresorhus/ky): Lightweight client built on Fetch

### Type-safe APIs

- [tRPC](https://trpc.io/): End-to-end type-safe APIs for TypeScript

### OpenAPI code generation

- [Orval](https://orval.dev/): Generates TypeScript clients and types from OpenAPI
- [openapi-typescript](https://openapi-ts.dev/): Generates TypeScript types from OpenAPI

### GraphQL

- [GraphQL](https://graphql.org/): Query language and execution specification for APIs
- [Apollo Client](https://www.apollographql.com/docs/react): GraphQL query, cache and status management library
- [urql](https://nearform.com/open-source/urql/): Expandable Lightweight GraphQL Client

### Real-time communication

- [Socket.IO](https://socket.io/): Event-based bidirectional realtime communication
- [WebSocket](https://developer.mozilla.org/docs/Web/API/WebSockets_API): Standard bidirectional realtime protocol
- [Server-Sent Events](https://developer.mozilla.org/docs/Web/API/Server-sent_events): Server-to-client event stream

### API mocking

- [MSW](https://mswjs.io/): Network-level API mocking

### Forms

- [React Hook Form](https://react-hook-form.com/): Performant React form state management
- [TanStack Form](https://tanstack.com/form/latest): Type-safe, multi-framework forms

### Schema validation

- [Zod](https://zod.dev/): TypeScript-first schema validation
- [Valibot](https://valibot.dev/): Modular schema validation

### Backend as a Service

- [Supabase](https://supabase.com/): Open-source PostgreSQL-based backend platform
- [Firebase](https://firebase.google.com/): Managed authentication, NoSQL database, and hosting platform

### ORM and query builders

- [Prisma](https://www.prisma.io/): Type-safe ORM for Node.js and TypeScript
- [Drizzle ORM](https://orm.drizzle.team/): SQL-oriented TypeScript ORM
- [Kysely](https://kysely.dev/): Type-safe SQL query builder

### Managed databases

- [Supabase Database](https://supabase.com/database): Manageable PostgreSQL with authentication and storage
- [Neon](https://neon.com/): Serverless PostgreSQL platform
- [Turso](https://turso.tech/): Edge database platform based on libSQL
- [PlanetScale](https://planetscale.com/): Managed MySQL and PostgreSQL platform
- [Cloudflare D1](https://developers.cloudflare.com/d1/): Serverless SQL database integrated with Cloudflare Workers

### Object storage

- [Vercel Blob](https://vercel.com/docs/storage/vercel-blob): Object storage for Vercel applications
- [Cloudflare R2](https://developers.cloudflare.com/r2/): S3-compatible object storage without egress fees
- [Supabase Storage](https://supabase.com/storage): Object Storage that can integrate Supabase Auth and Row Level Security
- [Amazon S3](https://aws.amazon.com/s3/): General-purpose object storage

## Backend and server

Do not separate the frontend and server from the outset; split them when product requirements justify it. Start ordinary CRUD and authentication inside a full-stack framework, then add a dedicated API server when the Python ecosystem, independent scaling, or complex domains require one.

### Full-stack backends

- [Next.js Route Handlers](https://nextjs.org/docs/app/getting-started/route-handlers): HTTP endpoints in the App Router
- [Next.js Server Functions and Actions](https://nextjs.org/docs/app/getting-started/updating-data): Server-side mutations and form handling

### TypeScript API frameworks

- [Hono](https://hono.dev/): Lightweight, Web Standards-based framework for multiple runtimes
- [Fastify](https://fastify.dev/): Low-overhead Node.js web framework with a plugin architecture
- [NestJS](https://nestjs.com/): Structured Node.js framework for larger applications
- [Express](https://expressjs.com/): Mature Node.js web framework with a broad ecosystem

### Python API frameworks

- [FastAPI](https://fastapi.tiangolo.com/): Python API framework built around type hints and OpenAPI
- [Django](https://www.djangoproject.com/): Batteries-included Python web framework
- [Flask](https://flask.palletsprojects.com/): Lightweight Python web framework

### API design and reliability

- [REST](https://developer.mozilla.org/docs/Glossary/REST): Universal HTTP API Design
- [Webhooks](https://www.svix.com/resources/webhooks/): An integrated way to receive events of external services to HTTP
- [Idempotency](https://docs.stripe.com/api/idempotent_requests): The design principles of request to prevent duplicate processing even when revised
- [OpenAPI](https://www.openapis.org/): Standard specification to document HTTP API and connect with tools

## Background jobs and workflows

Use these tools for work that cannot reliably finish within a request, such as email delivery, webhook retries, scheduled synchronization, and AI processing. Solo operators should evaluate managed services before running queue workers themselves.

### Managed jobs and durable workflows

- [Inngest](https://www.inngest.com/): Event-driven background jobs with step-level retries
- [Trigger.dev](https://trigger.dev/): Long-running TypeScript jobs and scheduled tasks
- [Upstash Workflow](https://upstash.com/docs/workflow/getstarted): Durable workflows for serverless applications

### Queues and message delivery

- [Upstash QStash](https://upstash.com/docs/qstash/overall/getstarted): HTTP message delivery, scheduling, and retries
- [Cloudflare Queues](https://developers.cloudflare.com/queues/): Managed queues integrated with Workers
- [BullMQ](https://docs.bullmq.io/): Redis-based Node.js queue for self-managed workers

### Scheduled jobs

- [Vercel Cron Jobs](https://vercel.com/docs/cron-jobs): Scheduled Vercel Function invocation
- [Cloudflare Cron Triggers](https://developers.cloudflare.com/workers/configuration/cron-triggers/): Scheduled Workers events
- [GitHub Actions](https://docs.github.com/actions/using-workflows/events-that-trigger-workflows#schedule): Scheduled workflow for repository operations and batch scripts

## Email and notifications

### Transactional email

- [Resend](https://resend.com/): Developer-focused transactional email API
- [Postmark](https://postmarkapp.com/): Transactional email delivery and tracking
- [Amazon SES](https://aws.amazon.com/ses/): AWS email delivery service for larger volumes

### Email templates

- [React Email](https://react.email/): Email templates built with React components

### Marketing email

- [Buttondown](https://buttondown.com/): Newsletter service for individuals and small teams
- [Mailchimp](https://mailchimp.com/): Audience management and marketing automation

### Push notifications

- [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging): Cross-platform push messaging
- [OneSignal](https://onesignal.com/): Push, in-app, and email messaging platform

## Cache and application infrastructure

### Managed cache and key-value storage

- [Upstash Redis](https://upstash.com/docs/redis/overall/getstarted): Managed Redis-compatible service for serverless and edge apps
- [Upstash for Redis on Vercel](https://vercel.com/marketplace/upstash): Managed Redis compatible services that connect to Vercel Marketplace
- [Cloudflare Workers KV](https://developers.cloudflare.com/kv/): Globally distributed, read-oriented key-value storage
- [Redis](https://redis.io/): In-memory data store for caching, sessions, and queues

### Common uses

- Cache: Store slow or less expensive results
- Rate limiting: Limiting requests in user, IP or API key units
- Session storage: Save login status that multiple server instances share
- Distributed locks: Fixed that multiple operations do not change resources at the same time

## Search

If the data is not large or simple to search, it starts at PostgreSQL, and introduces a dedicated search engine when the Otta allowed·Faceting·related adjustment is important.

- [PostgreSQL Full Text Search](https://www.postgresql.org/docs/current/textsearch.html)
- [Meilisearch](https://www.meilisearch.com/docs)
- [Typesense](https://typesense.org/docs/)
- [Algolia](https://www.algolia.com/doc/)
- [OpenSearch](https://opensearch.org/docs/latest/)
- [pgvector](https://github.com/pgvector/pgvector)

## State management

### Server state

- [TanStack Query](https://tanstack.com/query/latest): Async server-state fetching, caching, and synchronization
- [SWR](https://swr.vercel.app/): React data fetching and caching from Vercel

### Client state

- [Zustand](https://zustand.docs.pmnd.rs/): Minimal React client-state management
- [Redux Toolkit](https://redux-toolkit.js.org/): Official recommended approach to Redux applications
- [Jotai](https://jotai.org/): Atomic React state management
- [Pinia](https://pinia.vuejs.org/): Official state library for Vue
- [NgRx](https://ngrx.io/): Angular state management using RxJS and Redux patterns
- [NGXS](https://www.ngxs.io/): Angular Status Management Framework
- [Recoil](https://github.com/facebookexperimental/Recoil): React Status Management Library archived. Jeonju National University
- [Vuex](https://vuex.vuejs.org/): Vue 2 and existing Vue project reference status management library

## Authentication

### Application-owned authentication

- [Better Auth](https://better-auth.com/): TypeScript authentication and authorization framework
- [Auth.js](https://authjs.dev/): Established JavaScript authentication library maintained by the Better Auth team
- [SimpleWebAuthn](https://simplewebauthn.dev/): WebAuthn and passkey implementation toolkit
- [Lucia](https://lucia-auth.com/): deprecated authentication library. Jeonju National University

### Managed authentication

- [Clerk](https://clerk.com/): Managed authentication with strong React and Next.js support
- [Auth0](https://auth0.com/): Managed authentication with enterprise capabilities
- [Kinde](https://kinde.com/): Fast integration focused authentication platform

### BaaS-integrated authentication

- [Supabase Auth](https://supabase.com/auth): Authentication integrated with Supabase and RLS
- [Firebase Authentication](https://firebase.google.com/products/auth): Authentication integrated with Firebase

### Passkey-first services

- [Corbado](https://www.corbado.com/): Certificated Platform for Passkey Introduction and Conversion
- [Hanko](https://www.hanko.io/): Open source platform with Passkey-first authentication

### Token handling

- [jose](https://github.com/panva/jose): JWT, JWS, and JWE signing, verification, and encryption
- [jwt-decode](https://github.com/auth0/jwt-decode): Client utility to decode JWT content. Not validation of signature or validity

## Development tools

### Code quality

- [ESLint](https://eslint.org/): JavaScript and TypeScript static analysis with Flat Config
- [Prettier](https://prettier.io/): Opinionated code formatter
- [Biome](https://biomejs.dev/): Rust-based linter and formatter
- [Oxlint](https://oxc.rs/docs/guide/usage/linter.html): High-performance JavaScript and TypeScript linter

### JavaScript runtimes

- [Node.js](https://nodejs.org/): Mainstream JavaScript runtime for servers and tooling
- [Bun](https://bun.com/): Runtime, package manager, bundler, and test toolkit

### Package managers

- [pnpm](https://pnpm.io/): Storage-efficient package manager with strong workspace support
- [npm](https://www.npmjs.com/): JavaScript Package Manager, included in Node.js
- [Yarn](https://yarnpkg.com/): Package Manager with Plug'n'Play and Workspace features

### Python project tools

- [uv](https://docs.astral.sh/uv/): Fast Python version, environment, dependency, and lockfile manager
- [Ruff](https://docs.astral.sh/ruff/): Python linter and formatter
- [Pyright](https://microsoft.github.io/pyright/): Python static type checker
- [Poetry](https://python-poetry.org/): Python dependencies and packaging management tools

### Build tools

- [Vite](https://vite.dev/): Frontend build tool based on Rolldown and Oxc (v7 and earlier used esbuild and Rollup)
- [Turbopack](https://nextjs.org/docs/app/api-reference/turbopack): Rust-based bundler integrated with Next.js
- [Rspack](https://rspack.rs/): Rust-based bundler compatible with the Webpack ecosystem
- [Webpack](https://webpack.js.org/): Mature bundler with a broad ecosystem
- [Rolldown](https://rolldown.rs/): Rust-based bundler with Rollup compatibility
- [esbuild](https://esbuild.github.io/): Go-based high performance JavaScript bundler and converter
- [Rollup](https://rollupjs.org/): Strong Burner for Library Packaging and ES Module Optimization

### Monorepo tools

- [Turborepo](https://turborepo.com/): Build system for JavaScript and TypeScript monorepos
- [Nx](https://nx.dev/): Multi-language monorepo platform
- [pnpm workspaces](https://pnpm.io/workspaces): pnpm built-in workspace function

### Release automation

- [Changesets](https://github.com/changesets/changesets): Versioning and changelog management for monorepos
- [release-please](https://github.com/googleapis/release-please): Conventional Commits-based Release PR Automation Tools

### Component development

- [Storybook](https://storybook.js.org/): Isolated UI component development, testing, and documentation
- [Bit](https://bit.dev/): Platform for development and sharing of components

## Testing

### Unit and integration testing

- [Vitest](https://vitest.dev/): Test framework integrated with the Vite ecosystem
- [Jest](https://jestjs.io/): JavaScript and TypeScript test framework
- [pytest](https://docs.pytest.org/): Python test framework

### Component testing

- [Testing Library](https://testing-library.com/): User-focused UI testing utilities

### End-to-end testing

- [Playwright](https://playwright.dev/): Cross-browser end-to-end testing and automation
- [Cypress](https://www.cypress.io/): End-to-end testing with an interactive developer experience

### API and load testing

- [Bruno](https://www.usebruno.com/): Open-source, repository-friendly API client
- [Postman](https://www.postman.com/): API design, testing, and collaboration platform
- [k6](https://grafana.com/docs/k6/latest/): Code-driven load testing

## Deployment and hosting

### CI/CD automation

- [GitHub Actions](https://github.com/features/actions): GitHub-integrated CI/CD
- [Jenkins](https://www.jenkins.io/): Built-in CI/CD automation server
- [Travis CI](https://www.travis-ci.com/): Cloud CI/CD Service

### Containers

- [Docker](https://www.docker.com/): Container packaging and execution
- [Kubernetes](https://kubernetes.io/): Open-source orchestration platform for automating the deployment, scaling, and operation of containerized applications

### Serverless deployment

- [SST](https://sst.dev/): AWS-based Full Stack and Serverless Application Development Tools
- [Serverless Framework](https://www.serverless.com/): Serverless Application Distribution Framework

### Frontend and full-stack platforms

- [Vercel](https://vercel.com/): Platform optimized for Next.js and frontend applications
- [Cloudflare Workers Static Assets](https://developers.cloudflare.com/workers/static-assets/): Cloudflare's recommended path for new static, SPA, and full-stack apps
- [Netlify](https://www.netlify.com/): Static and full-stack web application platform
- [Firebase App Hosting](https://firebase.google.com/products/app-hosting): Full-stack web application hosting
- [AWS Amplify](https://aws.amazon.com/amplify/): AWS-based poolside web development and hosting
- [Firebase Hosting](https://firebase.google.com/products/hosting): static site and SPA hosting
- [Cloudflare Pages](https://pages.cloudflare.com/): static and web application hosting for existing Pages projects

### Application and container platforms

- [Render](https://render.com/): Backend, database, and full-stack application platform
- [Fly.io](https://fly.io/): Globally distributed container platform
- [Google Cloud Run](https://cloud.google.com/run): Serverless container runtime

### Cloud infrastructure

- [Amazon S3](https://aws.amazon.com/s3/): General-purpose object storage
- [Amazon CloudFront](https://aws.amazon.com/cloudfront/): Global CDN to transfer static and dynamic content

### Domain registrars

#### International

- [Cloudflare Registrar](https://www.cloudflare.com/products/registrar/): Registrar of Registration, providing cost-based pricing and Cloudflare DNS integration
- [Porkbun](https://porkbun.com/products/domains): A registered organization that provides protection of WHOIS personal information with transparent prices and free
- [Namecheap](https://www.namecheap.com/domains/): A registered organization that provides web services related to domain

#### South Korea

- [Gabia](https://www.gabia.com/): Domain registration system convenient for domestic payment and proofing
- [Hosting.kr](https://www.hosting.kr/domain/search): Local domain registration and hosting services

### DNS

- [Cloudflare DNS](https://www.cloudflare.com/dns/): Global DNS with integrated CDN and security features
- [Amazon Route 53](https://aws.amazon.com/route53/): Highly available DNS and traffic routing on AWS

### Development DNS

- [DuckDNS](https://www.duckdns.org/): Free Dynamic DNS for development and personal projects
- [sslip.io](https://sslip.io/): DNS for development that automatically interprets hostname with IP address
- [nip.io](https://nip.io/): Wildcard DNS for Local and Test Environment

### DNS diagnostics

- [DNSChecker](https://dnschecker.org/): Domain Name Search Engine Optimization
- [ICANN Lookup](https://lookup.icann.org/): Search Engine Optimization
- [who.is](https://who.is/): Domain Registrar, Expiration Dates and Public WHOIS Information View Tool

## Operations

In one operation, it is important that you can quickly discover obstacles than the number of tools and recover them in less steps. Before deploying, set the possession location and recovery procedure of the items below.

### Secrets and configuration

- Hosting platform environment variables: the simplest basic choice of small projects
- [Doppler](https://www.doppler.com/): A platform that manages multiple environments and services secrets centrally
- [1Password Secrets Automation](https://developer.1password.com/docs/secrets-automation/): 1Password vault’s Secret to CI and Applications
- Principle: Unpack Secret to the repository and client bundles, separate development·Preview·Production value and record the replacement procedure

### Uptime and status

- [Better Stack Uptime](https://betterstack.com/uptime): Uptime Monitoring, On-call and Status page service
- [UptimeRobot](https://uptimerobot.com/): Simple HTTP, Keyword and Port Monitoring Services
- [Checkly](https://www.checklyhq.com/): Playwright-based Synthetic Monitoring and API check platform

### Backups and recovery

- Managed database for automatic backup and Point-in-time recovery
- [pg_dump](https://www.postgresql.org/docs/current/app-pgdump.html): PostgreSQL logic backup tool
- Database as well as Object storage, DNS, environment variables and external service settings also record
- If you don’t want to create backups, check regularly to be a real Restore in a separate environment.

### Feature flags

- [PostHog Feature Flags](https://posthog.com/docs/feature-flags): Product analytics
- [Flags SDK](https://flags-sdk.dev/): Feature flag standardization tool to connect multiple Providers with Next.js
- [Unleash](https://docs.getunleash.io/): Open source feature management platform for self-hosting

### Cost controls

- Hosting, database, email, storage and set up a budget alert for AI providers
- Use-based services consist of rate limit, monthly and more usage alerts
- Preview Deployment and unused database·Story and log cleanup cycles

## Quality, security, and observability

### Performance

#### Web Vitals and performance audits

- [web.dev Performance](https://web.dev/performance/): Core Web Vitals and Web Performance Guides
- [PageSpeed Insights](https://pagespeed.web.dev/): Realistic and laboratory performance diagnosis
- [Lighthouse](https://developer.chrome.com/docs/lighthouse): Performance, Accessibility, SEO and Best Practice Audit Tool
- [WebPageTest](https://www.webpagetest.org/): Analysis of detailed web performance in various environments

#### Bundle size and optimization

- [Bundlephobia](https://bundlephobia.com/): npm Package Bundle Size Check Tool
- [`@next/bundle-analyzer`](https://www.npmjs.com/package/@next/bundle-analyzer): Visualization of bundle configuration of the Next.js application
- [webpack-bundle-analyzer](https://www.npmjs.com/package/webpack-bundle-analyzer): Webpack Bundle Configuration and Size Visualization

### Accessibility

- [WCAG](https://www.w3.org/WAI/standards-guidelines/wcag/): Web Accessibility International Guidelines
- [axe-core](https://github.com/dequelabs/axe-core): Automated Accessibility Inspection Engine
- [Storybook Accessibility](https://storybook.js.org/docs/writing-tests/accessibility-testing): Scots Gaelic
- [eslint-plugin-jsx-a11y](https://github.com/jsx-eslint/eslint-plugin-jsx-a11y): JSX Accessibility Rules Inspection

### Security

#### Guides and browser security

- Follow the [OWASP Web Security Testing Guide](https://owasp.org/www-project-web-security-testing-guide/)
- [Content Security Policy](https://developer.mozilla.org/docs/Web/HTTP/CSP): A browser security policy that limits scripts and resource execution sources
- [Trusted Types](https://developer.mozilla.org/docs/Web/API/Trusted_Types_API): DOM XSS Browser API Reducing Risks
- [DOMPurify](https://github.com/cure53/DOMPurify): A library that cleans unreliable HTML

#### Server and integration security

- Distinguish authentication from authorization, and have the server verify permissions again for every data-changing operation
- For cookie-based authentication, configure `Secure`, `HttpOnly`, and `SameSite` together with [CSRF](https://owasp.org/www-community/attacks/csrf) protection
- [CORS](https://developer.mozilla.org/docs/Web/HTTP/CORS): Allow only the required origins, methods, and headers
- Verify signatures on external webhooks for payments, authentication, and email, and use idempotency keys to prevent duplicate processing
- Apply rate limits and input-size limits to public APIs and operations that incur costs

#### Dependencies and supply chain

- [Dependabot](https://docs.github.com/code-security/dependabot): Responsible security updates and vulnerability notifications
- [`npm audit`](https://docs.npmjs.com/cli/commands/npm-audit): npm Known Vulnerability Test
- CI uses Lockfile and short-life Credential for minimum authority

### Observability

- [Sentry](https://sentry.io/): Error tracking and application performance monitoring
- [Vercel Observability](https://vercel.com/docs/observability): Vercel-native insights for requests, functions, errors, and usage
- [Grafana](https://grafana.com/): Dashboards and alerting across metrics, logs, traces, and profiles
- [OpenTelemetry](https://opentelemetry.io/): Vendor-neutral logs, metrics, and traces
- [Web Vitals](https://github.com/GoogleChrome/web-vitals): Real-user Core Web Vitals measurement
- Operation principle: Contains request ID and distribution version to log·Withdraw, User information and Secret does not record and set the storage period

### Browser compatibility

- [web.dev Baseline](https://web.dev/baseline): Web function support status standard between browsers
- [Browserslist](https://browsersl.ist/): Configuring support browser range between tools
- [Can I Use](https://caniuse.com/): Web Platform features browser support status

## Product integrations

### SEO & GEO

#### Guides and standards

- [sitemaps.org](https://www.sitemaps.org/): sitemap.xml protocol specification
- [JSON-LD](https://www.w3.org/TR/json-ld11/): Search engines and AI tools to help understand the structure and meaning of content
- [`robots.txt`](https://www.rfc-editor.org/rfc/rfc9309): Standards for searching and setting access policies of AI crawlers
- [Google Search Central](https://developers.google.com/search): Google’s Official Search Optimization Document
- [The Beginner's Guide to SEO](https://moz.com/beginners-guide-to-seo): Mozart's comprehensive SEO guide
- [llms.txt](https://llmstxt.org/): AI agent is a proposition standard that spreads to read site information easily.

#### Frameworks and libraries

- Next.js [Metadata API](https://nextjs.org/docs/app/getting-started/metadata-and-og-images): Basic metadata and Open Graph management of App Router
- [next-seo](https://github.com/garmeeh/next-seo): Auxiliary library that manages metadata and Open Graph settings in the existing Next.js project
- [next-sitemap](https://github.com/iamvishnusankar/next-sitemap): Sitemap.xml and robots.txt creation tools for Next.js
- [schema-dts](https://github.com/google/schema-dts): TypeScript for Schema.org JSON-LD

#### Search engine consoles

- [Google Search Console](https://search.google.com/search-console/): Google Search Index and Search Performance Management Tools
- [Naver Search Advisor](https://searchadvisor.naver.com/): Naver search indexing and site diagnostics tool
- [Bing Webmaster Tools](https://www.bing.com/webmasters/about): Bing Search Index and Performance Management Tools

#### AI crawler monitoring

- [Cloudflare AI Crawl Control](https://developers.cloudflare.com/ai-crawl-control/): A service that analyzes AI crawler access status and manages crawler policy (formerly name: AI Audit)

#### Debuggers

- [SEO Site Checkup](https://seositecheckup.com/): Technical SEO diagnostic services of website
- [Google Rich Results Test](https://search.google.com/test/rich-results): Structural Data and Rich Results Validation Tool
- [OpenGraph.xyz](https://www.opengraph.xyz/): Open Graph metadata preview tool
- [Meta Sharing Debugger](https://developers.facebook.com/tools/debug/): Share information check and cache update tool for Meta service
- [Kakao URL Debugger](https://developers.kakao.com/tool/debugger/sharing): KakaoTalk Share Metadata Scan and Cash Update Tool

### Analytics

#### Web analytics

- [Google Analytics](https://analytics.google.com/): Traffic and Conversion Analysis Services for Web and App
  - [GA Dev Tools](https://ga-dev-tools.google/ga4/): Google Analytics Demo and Debugging Utilities
- [Plausible](https://plausible.io/): Lightweight, privacy-focused web analytics service
- [Statcounter](https://statcounter.com/): Live visitors and traffic statistics services

#### Product analytics

- [Amplitude](https://amplitude.com/): Cohort, Foundation and user behavior analysis platform
- [Mixpanel](https://mixpanel.com/): Event-based product analytics platform
- [PostHog](https://posthog.com/): Open source platform that provides analysis, session playback and function flags

#### Heatmaps and session replay

- [Microsoft Clarity](https://clarity.microsoft.com/): Free session playback and hit map service
- [Hotjar](https://www.hotjar.com/): Session playback, hitmap and user feedback tools

#### Tag management

- Tag management: [Google Tag Manager](https://tagmanager.google.com/)

#### Attribution and marketing pixels

- [Airbridge](https://www.airbridge.io/): Web and App Marketing Contribution Measurement Platform
- [Meta Pixel](https://www.facebook.com/business/tools/meta-pixel): Meta advertising conversion measurement and retargeting tools
- [Kakao Pixel & SDK](https://business.kakao.com/info/pixelsdk/): Kakao advertising conversion and user behavior measurement tools

#### Consent and privacy

- [Google Consent Mode](https://developers.google.com/tag-platform/security/guides/consent): How to reflect the user’s consent status to Google tag operation
- [Klaro](https://klaro.org/): Open Source Consent manager that can self-host
- [Cookiebot](https://www.cookiebot.com/): Cookie Scan and Consent banner
- Principle: Write a privacy policy appropriate to the service regions and collected data, and do not run unnecessary analytics or advertising scripts before consent

### Payments and monetization

#### Global payments

- [Stripe](https://stripe.com/): Automated TrackingAnalyticsNotificationsTrack ButtonApps & Plugins
  - [Link](https://link.com/): One-click payment service provided by Stripe
- [PayPal](https://www.paypal.com/): Global online payment and digital wallet service

#### Korean payments

- [Toss Payments](https://www.tosspayments.com/): PG service providing domestic payment API and payment UI
- [PortOne](https://developers.portone.io/): Payments with multiple PGs to connect with a single API
- [KG Inicis](https://www.inicis.com/): LOGIN JOIN
- [NHN KCP](https://www.kcp.co.kr/): Korean online and offline electronic payment service

#### Subscriptions and Merchant of Record

- [Paddle](https://www.paddle.com/): Merchant of Record providing SaaS payment, subscription, tax processing
- [Lemon Squeezy](https://www.lemonsqueezy.com/): Payment for digital products and SaaS and Merchant of Record
- [RevenueCat](https://www.revenuecat.com/): Mobile App and Web Subscription Management Platform

#### Sponsorship

- [GitHub Sponsors](https://github.com/sponsors): Open Source Developer Sponsorship Platform
- [Patreon](https://www.patreon.com/): Recurring membership and creator sponsorship platform
- [Buy Me a Coffee](https://buymeacoffee.com/): One-time and recurring support service for creators
- [Ko-fi](https://ko-fi.com/): Support, membership and digital products sales service

### Advertising

#### Web ad networks

- [Google AdSense](https://adsense.google.com/): Google Ad Revenue Platform for Websites
- [kakaoAdFit](https://adfit.kakao.com/): Kakao’s domestic web and app advertising platform
- [Taboola](https://www.taboola.com/): Content-recommendation-based native advertising platform
- [Outbrain](https://www.outbrain.com/): Content-recommendation-based native advertising platform

#### In-app ad networks

- [Google AdMob](https://admob.google.com/): Google Ad Platform for Mobile App
- [AppLovin MAX](https://www.applovin.com/max/): Mobile Advertisement Platform
- [Unity LevelPlay](https://unity.com/products/levelplay): Mobile Apps and Games Advertising Beauty Platform

#### Affiliate and commerce ads

- [Coupang Partners](https://partners.coupang.com/): Korean affiliate marketing program based on product links
- [Amazon Associates](https://affiliate-program.amazon.com/): Global Affiliate Marketing Program for Amazon Products

#### Ad infrastructure

- [Google Publisher Tag](https://developers.google.com/publisher-tag): Google Ad Manager Ads to display and control the web
- [Prebid.js](https://prebid.org/product-suite/prebidjs/): Browser-based Header Bidding Open Source Library

### Maps and location

#### Commercial map platforms

- [Google Maps Platform](https://developers.google.com/maps): Global maps, place search, and routing APIs
- [Kakao Maps](https://apis.map.kakao.com/): Place search and map APIs for South Korea
- [Naver Maps](https://www.ncloud.com/product/applicationService/maps): Maps, places, and routing APIs for South Korea

#### Vector and open-source maps

- [Mapbox](https://www.mapbox.com/): Custom vector maps and location services platform
- [Leaflet](https://leafletjs.com/): Lightweight 2D map library commonly used with open map tiles
- [OpenLayers](https://openlayers.org/): Open-source map library supporting vector tiles and a wide range of geospatial data formats

#### Geospatial visualization

- [deck.gl](https://deck.gl/): WebGL-based framework for large-scale geospatial visualization

## Data visualization

### Charts

- [Chart.js](https://www.chartjs.org/): Easy to use Canvas-based Chart Library
- [Recharts](https://recharts.org/): React component-based chart library
- [Apache ECharts](https://echarts.apache.org/): A library that supports various charts and large data renderings
- [D3](https://d3js.org/): Low level library for data-based custom visualization
- [Plotly](https://plotly.com/javascript/): A strong interactive chart library of science and science and 3D visualization
- [AG Charts](https://www.ag-grid.com/charts/): © 2020 Sennheiser electronic GmbH & Co. KG   Germany

### Graphics

- [Three.js](https://threejs.org/): WebGL Library for Web 3D Graphics
- [PixiJS](https://pixijs.com/): High Performance 2D WebGL Rendering Engine

## Cross-platform development

- [React Native](https://reactnative.dev/): Native application framework based on React
- [Flutter](https://flutter.dev/): Dart-based multi-platform UI framework
- [Ionic](https://ionicframework.com/): Cross-platform application framework built on web technologies and WebView

## Developer services

- [CodePen](https://codepen.io/): A browser-based editor for creating front-end examples and sharing
- [JSFiddle](https://jsfiddle.net/): Online editor to run and share HTML, CSS and JavaScript
- [Transform](https://transform.tools/) for developer data and code conversion
- [Bitly](https://bitly.com/) for short URLs
- [Lorem Picsum](https://picsum.photos/) for placeholder images

## AI development

- [AI SDK](https://ai-sdk.dev/): TypeScript toolkit for AI applications and agents
- [LM Studio](https://lmstudio.ai/): Local AI model runtime
- [Hugging Face](https://huggingface.co/): Community for models, datasets, and AI applications
- [OpenRouter](https://openrouter.ai/): Unified API platform for multiple AI models

## Git and releases

### Version control

- [Git](https://git-scm.com/): Decentralized Version Management System
- [Git Cheat Sheet](https://git-scm.com/cheat-sheet): Summary of Git commands often used

### Branching workflows

- [GitHub Flow](https://docs.github.com/get-started/using-github/github-flow) for short-lived branches and pull requests
- [Trunk Based Development](https://trunkbaseddevelopment.com/) for frequent integration into the main branch
- [Git-flow](https://nvie.com/posts/a-successful-git-branching-model/): Traditional model using long-term brand. Jeonju National University

### Versioning and commit conventions

- [Semantic Versioning](https://semver.org/): Version rules based on public API changes
- [Conventional Commits](https://www.conventionalcommits.org/): Automated TrackingAnalysis

### README badges

- [Shields.io](https://shields.io/): Create a badge for displaying repositories and project status
- [Badgen](https://badgen.net/): Fast and concise SVG badge creation service
- [Markdown Badges](https://github.com/Ileriayo/markdown-badges): Curated collection of Markdown badges for developer profiles and projects

## Created by

This handbook is created and maintained by [Dokkaebi Club](https://dokkaebiclub.dev/?utm_source=github&utm_medium=referral&utm_campaign=tech-stack-handbook).

## License

Copyright © 2026 Lee Jihye. This work is licensed under the [Creative Commons Attribution 4.0 International License](LICENSE).
