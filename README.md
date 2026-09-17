# Web Tech Stack Handbook 2026

**English** | [한국어](README.ko.md)

> A practical 2026 web development tech stack guide for solo builders—from frontend and backend to deployment, analytics, and operations.

This handbook organizes modern tools and services for building web products across frontend development, full-stack architecture, databases, deployment, and product operations.

Recommendations consider not only adoption in new projects, but also **development speed, operational overhead, cost, and scalability**.

## How this handbook is organized

Tools that serve the same purpose are generally ordered by:

1. Suitability for solo builders who need to ship and operate quickly
2. Adoption and momentum in new projects
3. Ecosystem maturity and maintenance stability
4. Fit for specialized requirements or larger organizations
5. Operationally heavy, experimental, or legacy status

Tools with different roles are not ranked directly against one another. The catalog is reviewed regularly as the ecosystem changes.

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
- [Svelte](https://svelte.dev/): Compiler-based UI framework
- [jQuery](https://jquery.com/): DOM library primarily relevant to legacy applications

### Full-stack and meta-frameworks

- [Next.js](https://nextjs.org/): Full-stack React framework
- [React Router](https://reactrouter.com/): React routing and full-stack web framework
- [Nuxt](https://nuxt.com/): Full-stack Vue framework
- [SvelteKit](https://svelte.dev/docs/kit): Full-stack Svelte framework
- [Astro](https://astro.build/): Multi-framework platform well suited to content-focused sites

### Static sites and documentation

- [Docusaurus](https://docusaurus.io/): React and MDX documentation generator
- [Hugo](https://gohugo.io/): Fast Go-based static site generator
- [Gatsby](https://www.gatsbyjs.com/): Mature React and GraphQL static-site framework

## Content and documentation

### CMS and authoring

- [Strapi](https://strapi.io/): Open-source Node.js headless CMS
- [Sanity](https://www.sanity.io/): SaaS CMS with custom schemas and real-time collaboration
- [Payload](https://payloadcms.com/): Code-first TypeScript CMS with strong Next.js integration
- [Contentful](https://www.contentful.com/): Enterprise-oriented SaaS CMS
- [Ghost](https://ghost.org/): Publishing, blogging, and newsletter platform
- [MDX](https://mdxjs.com/): Markdown with embedded JSX components
- [Tiptap](https://tiptap.dev/): Headless rich-text editor built on ProseMirror
- [Lexical](https://lexical.dev/): Extensible rich-text editor framework from Meta

### Documentation utilities

- [Shiki](https://shiki.style/): Syntax highlighter using VS Code grammars and themes
- [Mermaid](https://mermaid.js.org/): Text-based diagrams and sequence charts
- [Read the Docs](https://about.readthedocs.com/): Documentation build and hosting platform
- [W3C Feed Validation Service](https://validator.w3.org/feed/): RSS and Atom feed validator

## Styling and UI

### Styling

- [Tailwind CSS](https://tailwindcss.com/): Utility-first CSS framework with CSS-first configuration
- [Bootstrap](https://getbootstrap.com/): CSS framework with ready-made components
- [Sass](https://sass-lang.com/): CSS preprocessor
- [styled-components](https://styled-components.com/): Runtime CSS-in-JS for React
- [Emotion](https://emotion.sh/): Flexible runtime CSS-in-JS library
- [vanilla-extract](https://vanilla-extract.style/): TypeScript-based zero-runtime styling
- [Panda CSS](https://panda-css.com/): Type-safe CSS-in-JS with build-time extraction

### Components

- [Radix UI](https://www.radix-ui.com/): Accessible headless React components
- [Headless UI](https://headlessui.com/): Headless React and Vue components from Tailwind Labs
- [Base UI](https://base-ui.com/): Headless React components from the MUI team
- [shadcn/ui](https://ui.shadcn.com/): Source-owned components built with Tailwind CSS and Radix UI or Base UI
- [Material UI](https://mui.com/): Material Design React component library
- [Ant Design](https://ant.design/): React UI system popular for admin and enterprise products
- [daisyUI](https://daisyui.com/): Component library implemented as a Tailwind CSS plugin

### Interaction and presentation

- [Lucide](https://lucide.dev/): Consistent open-source SVG icon set
- [Google Fonts](https://fonts.google.com/): Web font discovery and delivery service
- [Motion](https://motion.dev/): UI animation library for React and JavaScript
- [GSAP](https://gsap.com/): Timeline and scroll animation platform
- [Lottie](https://airbnb.io/lottie/): JSON-based vector animation format and renderer
- [TanStack Table](https://tanstack.com/table/latest): Headless data-table library
- [AG Grid](https://www.ag-grid.com/): Data grid for large datasets and enterprise requirements
- [react-hotkeys-hook](https://react-hotkeys-hook.vercel.app/): Declarative keyboard shortcuts for React

## Data and APIs

### Clients and contracts

- [Fetch API](https://developer.mozilla.org/docs/Web/API/Fetch_API): Standard HTTP API in browsers and modern JavaScript runtimes
- [Axios](https://axios-http.com/): Promise-based HTTP client for browsers and Node.js
- [Ky](https://github.com/sindresorhus/ky): Lightweight client built on Fetch
- [tRPC](https://trpc.io/): End-to-end type-safe APIs for TypeScript
- [Orval](https://orval.dev/): Generates TypeScript clients and types from OpenAPI
- [openapi-typescript](https://openapi-ts.dev/): Generates TypeScript types from OpenAPI
- [GraphQL](https://graphql.org/): Query language and execution specification for APIs

### Realtime, forms, and validation

- [Socket.IO](https://socket.io/): Event-based bidirectional realtime communication
- [WebSocket](https://developer.mozilla.org/docs/Web/API/WebSockets_API): Standard bidirectional realtime protocol
- [Server-Sent Events](https://developer.mozilla.org/docs/Web/API/Server-sent_events): Server-to-client event stream
- [MSW](https://mswjs.io/): Network-level API mocking
- [React Hook Form](https://react-hook-form.com/): Performant React form state management
- [TanStack Form](https://tanstack.com/form/latest): Type-safe, multi-framework forms
- [Zod](https://zod.dev/): TypeScript-first schema validation
- [Valibot](https://valibot.dev/): Modular schema validation

### Data platforms

- [Supabase](https://supabase.com/): Open-source PostgreSQL-based backend platform
- [Firebase](https://firebase.google.com/): Managed authentication, NoSQL database, and hosting platform
- [Prisma](https://www.prisma.io/): Type-safe ORM for Node.js and TypeScript
- [Drizzle ORM](https://orm.drizzle.team/): SQL-oriented TypeScript ORM
- [Kysely](https://kysely.dev/): Type-safe SQL query builder
- [Neon](https://neon.com/): Serverless PostgreSQL platform
- [Turso](https://turso.tech/): Edge database platform based on libSQL
- [PlanetScale](https://planetscale.com/): Managed MySQL and PostgreSQL platform
- [Cloudflare D1](https://developers.cloudflare.com/d1/): Serverless SQL database integrated with Cloudflare Workers
- [Vercel Blob](https://vercel.com/docs/storage/vercel-blob): Object storage for Vercel applications
- [Cloudflare R2](https://developers.cloudflare.com/r2/): S3-compatible object storage without egress fees
- [Amazon S3](https://aws.amazon.com/s3/): General-purpose object storage

## Backend and server

Start ordinary CRUD and authentication inside a full-stack framework. Add a dedicated API server when Python libraries, independent scaling, or complex domain boundaries justify the extra operational cost.

- [Next.js Route Handlers](https://nextjs.org/docs/app/getting-started/route-handlers): HTTP endpoints in the App Router
- [Next.js Server Functions and Actions](https://nextjs.org/docs/app/getting-started/updating-data): Server-side mutations and form handling
- [Hono](https://hono.dev/): Lightweight, Web Standards-based framework for multiple runtimes
- [Fastify](https://fastify.dev/): Low-overhead Node.js web framework with a plugin architecture
- [NestJS](https://nestjs.com/): Structured Node.js framework for larger applications
- [Express](https://expressjs.com/): Mature Node.js web framework with a broad ecosystem
- [FastAPI](https://fastapi.tiangolo.com/): Python API framework built around type hints and OpenAPI
- [Django](https://www.djangoproject.com/): Batteries-included Python web framework
- [Flask](https://flask.palletsprojects.com/): Lightweight Python web framework

Design APIs with [REST](https://developer.mozilla.org/docs/Glossary/REST), [OpenAPI](https://www.openapis.org/), signed webhooks, and idempotent operations where retries are possible.

## Background jobs and workflows

Prefer managed execution before operating your own queue workers.

- [Inngest](https://www.inngest.com/): Event-driven background jobs with step-level retries
- [Trigger.dev](https://trigger.dev/): Long-running TypeScript jobs and scheduled tasks
- [Upstash Workflow](https://upstash.com/docs/workflow/getstarted): Durable workflows for serverless applications
- [Upstash QStash](https://upstash.com/docs/qstash/overall/getstarted): HTTP message delivery, scheduling, and retries
- [Cloudflare Queues](https://developers.cloudflare.com/queues/): Managed queues integrated with Workers
- [BullMQ](https://docs.bullmq.io/): Redis-based Node.js queue for self-managed workers
- [Vercel Cron Jobs](https://vercel.com/docs/cron-jobs): Scheduled Vercel Function invocation
- [Cloudflare Cron Triggers](https://developers.cloudflare.com/workers/configuration/cron-triggers/): Scheduled Workers events

## Email and notifications

- [Resend](https://resend.com/): Developer-focused transactional email API
- [Postmark](https://postmarkapp.com/): Transactional email delivery and tracking
- [Amazon SES](https://aws.amazon.com/ses/): AWS email delivery service for larger volumes
- [React Email](https://react.email/): Email templates built with React components
- [Buttondown](https://buttondown.com/): Newsletter service for individuals and small teams
- [Mailchimp](https://mailchimp.com/): Audience management and marketing automation
- [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging): Cross-platform push messaging
- [OneSignal](https://onesignal.com/): Push, in-app, and email messaging platform

## Cache and application infrastructure

- [Upstash Redis](https://upstash.com/docs/redis/overall/getstarted): Managed Redis-compatible service for serverless and edge apps
- [Cloudflare Workers KV](https://developers.cloudflare.com/kv/): Globally distributed, read-oriented key-value storage
- [Redis](https://redis.io/): In-memory data store for caching, sessions, and queues

Common uses include caching expensive reads, rate limiting, shared session storage, and distributed locks.

## Search

Start with PostgreSQL when requirements are simple. Add a dedicated search engine when typo tolerance, faceting, or relevance tuning becomes important.

- [PostgreSQL Full Text Search](https://www.postgresql.org/docs/current/textsearch.html)
- [Meilisearch](https://www.meilisearch.com/docs)
- [Typesense](https://typesense.org/docs/)
- [Algolia](https://www.algolia.com/doc/)
- [OpenSearch](https://opensearch.org/docs/latest/)
- [pgvector](https://github.com/pgvector/pgvector)

## State management

- [TanStack Query](https://tanstack.com/query/latest): Async server-state fetching, caching, and synchronization
- [SWR](https://swr.vercel.app/): React data fetching and caching from Vercel
- [Zustand](https://zustand.docs.pmnd.rs/): Minimal React client-state management
- [Redux Toolkit](https://redux-toolkit.js.org/): Official recommended approach to Redux applications
- [Jotai](https://jotai.org/): Atomic React state management
- [Pinia](https://pinia.vuejs.org/): Official state library for Vue
- [NgRx](https://ngrx.io/): Angular state management using RxJS and Redux patterns

## Authentication

- [Better Auth](https://better-auth.com/): TypeScript authentication and authorization framework
- [Auth.js](https://authjs.dev/): Established JavaScript authentication library maintained by the Better Auth team
- [SimpleWebAuthn](https://simplewebauthn.dev/): WebAuthn and passkey implementation toolkit
- [Clerk](https://clerk.com/): Managed authentication with strong React and Next.js support
- [Auth0](https://auth0.com/): Managed authentication with enterprise capabilities
- [Supabase Auth](https://supabase.com/auth): Authentication integrated with Supabase and RLS
- [Firebase Authentication](https://firebase.google.com/products/auth): Authentication integrated with Firebase
- [jose](https://github.com/panva/jose): JWT, JWS, and JWE signing, verification, and encryption

## Development tools

- [ESLint](https://eslint.org/): JavaScript and TypeScript static analysis with Flat Config
- [Prettier](https://prettier.io/): Opinionated code formatter
- [Biome](https://biomejs.dev/): Rust-based linter and formatter
- [Oxlint](https://oxc.rs/docs/guide/usage/linter.html): High-performance JavaScript and TypeScript linter
- [Node.js](https://nodejs.org/): Mainstream JavaScript runtime for servers and tooling
- [Bun](https://bun.com/): Runtime, package manager, bundler, and test toolkit
- [pnpm](https://pnpm.io/): Storage-efficient package manager with strong workspace support
- [uv](https://docs.astral.sh/uv/): Fast Python version, environment, dependency, and lockfile manager
- [Ruff](https://docs.astral.sh/ruff/): Python linter and formatter
- [Pyright](https://microsoft.github.io/pyright/): Python static type checker

### Build and monorepo tools

- [Vite](https://vite.dev/): Frontend build tool based on Rolldown and Oxc (v7 and earlier used esbuild and Rollup)
- [Turbopack](https://nextjs.org/docs/app/api-reference/turbopack): Rust-based bundler integrated with Next.js
- [Rspack](https://rspack.rs/): Rust-based bundler compatible with the Webpack ecosystem
- [Webpack](https://webpack.js.org/): Mature bundler with a broad ecosystem
- [Turborepo](https://turborepo.com/): Build system for JavaScript and TypeScript monorepos
- [Nx](https://nx.dev/): Multi-language monorepo platform
- [Changesets](https://github.com/changesets/changesets): Versioning and changelog management for monorepos
- [Storybook](https://storybook.js.org/): Isolated UI component development, testing, and documentation

## Testing

- [Vitest](https://vitest.dev/): Test framework integrated with the Vite ecosystem
- [Jest](https://jestjs.io/): JavaScript and TypeScript test framework
- [pytest](https://docs.pytest.org/): Python test framework
- [Testing Library](https://testing-library.com/): User-focused UI testing utilities
- [Playwright](https://playwright.dev/): Cross-browser end-to-end testing and automation
- [Cypress](https://www.cypress.io/): End-to-end testing with an interactive developer experience
- [Bruno](https://www.usebruno.com/): Open-source, repository-friendly API client
- [Postman](https://www.postman.com/): API design, testing, and collaboration platform
- [k6](https://grafana.com/docs/k6/latest/): Code-driven load testing

## Deployment and hosting

- [GitHub Actions](https://github.com/features/actions): GitHub-integrated CI/CD
- [Docker](https://www.docker.com/): Container packaging and execution
- [Vercel](https://vercel.com/): Platform optimized for Next.js and frontend applications
- [Cloudflare Workers Static Assets](https://developers.cloudflare.com/workers/static-assets/): Cloudflare's recommended path for new static, SPA, and full-stack apps
- [Netlify](https://www.netlify.com/): Static and full-stack web application platform
- [Firebase App Hosting](https://firebase.google.com/products/app-hosting): Full-stack web application hosting
- [Render](https://render.com/): Backend, database, and full-stack application platform
- [Fly.io](https://fly.io/): Globally distributed container platform
- [Google Cloud Run](https://cloud.google.com/run): Serverless container runtime
- [Cloudflare DNS](https://www.cloudflare.com/dns/): Global DNS with integrated CDN and security features
- [Amazon Route 53](https://aws.amazon.com/route53/): Highly available DNS and traffic routing on AWS

## Operations

For a solo operator, fast detection and simple recovery matter more than the number of available features.

- Keep secrets out of repositories and client bundles; separate development, preview, and production values
- Use hosting-platform environment variables first, then consider [Doppler](https://www.doppler.com/) or [1Password Secrets Automation](https://developer.1password.com/docs/secrets-automation/)
- Monitor availability with [Better Stack Uptime](https://betterstack.com/uptime), [UptimeRobot](https://uptimerobot.com/), or [Checkly](https://www.checklyhq.com/)
- Verify managed-database backups and point-in-time recovery; test restores instead of only checking that backups exist
- Use [PostHog Feature Flags](https://posthog.com/docs/feature-flags), [Flags SDK](https://flags-sdk.dev/), or [Unleash](https://docs.getunleash.io/) when staged rollouts become necessary
- Configure budget alerts and usage limits for hosting, databases, email, storage, and AI providers

## Quality, security, and observability

### Performance and accessibility

- [web.dev Performance](https://web.dev/performance/), [PageSpeed Insights](https://pagespeed.web.dev/), [Lighthouse](https://developer.chrome.com/docs/lighthouse), and [WebPageTest](https://www.webpagetest.org/)
- [Bundlephobia](https://bundlephobia.com/) and [`@next/bundle-analyzer`](https://www.npmjs.com/package/@next/bundle-analyzer)
- [WCAG](https://www.w3.org/WAI/standards-guidelines/wcag/), [axe-core](https://github.com/dequelabs/axe-core), and [Storybook Accessibility](https://storybook.js.org/docs/writing-tests/accessibility-testing)

### Security

- Follow the [OWASP Web Security Testing Guide](https://owasp.org/www-project-web-security-testing-guide/)
- Apply [Content Security Policy](https://developer.mozilla.org/docs/Web/HTTP/CSP), [Trusted Types](https://developer.mozilla.org/docs/Web/API/Trusted_Types_API), and [DOMPurify](https://github.com/cure53/DOMPurify) where appropriate
- Recheck authorization for every server-side mutation; do not treat authentication as authorization
- Configure secure cookies and CSRF protection; restrict CORS to required origins, methods, and headers
- Verify webhook signatures, use idempotency keys, and rate-limit public or cost-generating endpoints
- Use [Dependabot](https://docs.github.com/code-security/dependabot) and [`npm audit`](https://docs.npmjs.com/cli/commands/npm-audit) for dependency risk

### Observability and compatibility

- [Sentry](https://sentry.io/): Error tracking and application performance monitoring
- [Vercel Observability](https://vercel.com/docs/observability): Vercel-native insights for requests, functions, errors, and usage
- [Grafana](https://grafana.com/): Dashboards and alerting across metrics, logs, traces, and profiles
- [OpenTelemetry](https://opentelemetry.io/): Vendor-neutral logs, metrics, and traces
- [Web Vitals](https://github.com/GoogleChrome/web-vitals): Real-user Core Web Vitals measurement
- [web.dev Baseline](https://web.dev/baseline), [Browserslist](https://browsersl.ist/), and [Can I Use](https://caniuse.com/) for browser compatibility

## Product integrations

### SEO and GEO

- Standards and guidance: [sitemaps.org](https://www.sitemaps.org/), [JSON-LD](https://www.w3.org/TR/json-ld11/), [`robots.txt`](https://www.rfc-editor.org/rfc/rfc9309), [Google Search Central](https://developers.google.com/search), and [llms.txt](https://llmstxt.org/)
- Next.js: [Metadata API](https://nextjs.org/docs/app/getting-started/metadata-and-og-images), [next-sitemap](https://github.com/iamvishnusankar/next-sitemap), and [schema-dts](https://github.com/google/schema-dts)
- Search consoles: [Google Search Console](https://search.google.com/search-console/), [Naver Search Advisor](https://searchadvisor.naver.com/), and [Bing Webmaster Tools](https://www.bing.com/webmasters/about)
- Debugging: [Google Rich Results Test](https://search.google.com/test/rich-results), [OpenGraph.xyz](https://www.opengraph.xyz/), and [Meta Sharing Debugger](https://developers.facebook.com/tools/debug/)

### Analytics and privacy

- Web analytics: [Google Analytics](https://analytics.google.com/), [Plausible](https://plausible.io/), and [Statcounter](https://statcounter.com/)
- Product analytics: [Amplitude](https://amplitude.com/), [Mixpanel](https://mixpanel.com/), and [PostHog](https://posthog.com/)
- Session replay: [Microsoft Clarity](https://clarity.microsoft.com/) and [Hotjar](https://www.hotjar.com/)
- Tag management: [Google Tag Manager](https://tagmanager.google.com/)
- Consent: [Google Consent Mode](https://developers.google.com/tag-platform/security/guides/consent), [Klaro](https://klaro.org/), and [Cookiebot](https://www.cookiebot.com/)

### Payments, monetization, and advertising

- Global payments: [Stripe](https://stripe.com/), [PayPal](https://www.paypal.com/), [Paddle](https://www.paddle.com/), and [Lemon Squeezy](https://www.lemonsqueezy.com/)
- Korean payments: [Toss Payments](https://www.tosspayments.com/), [PortOne](https://developers.portone.io/), [KG Inicis](https://www.inicis.com/), and [NHN KCP](https://www.kcp.co.kr/)
- Sponsorships: [GitHub Sponsors](https://github.com/sponsors), [Patreon](https://www.patreon.com/), [Buy Me a Coffee](https://buymeacoffee.com/), and [Ko-fi](https://ko-fi.com/)
- Advertising: [Google AdSense](https://adsense.google.com/), [Google AdMob](https://admob.google.com/), [Taboola](https://www.taboola.com/), and [Outbrain](https://www.outbrain.com/)
- Affiliate programs: [Coupang Partners](https://partners.coupang.com/) and [Amazon Associates](https://affiliate-program.amazon.com/)

### Maps and location

- [Google Maps Platform](https://developers.google.com/maps), [Kakao Maps](https://apis.map.kakao.com/), and [Naver Maps](https://www.ncloud.com/product/applicationService/maps)
- [Mapbox](https://www.mapbox.com/) and [Leaflet](https://leafletjs.com/)
- [deck.gl](https://deck.gl/) for large-scale geospatial visualization

## Data visualization

- Charts: [Chart.js](https://www.chartjs.org/), [Recharts](https://recharts.org/), [Apache ECharts](https://echarts.apache.org/), [D3](https://d3js.org/), [Plotly](https://plotly.com/javascript/), and [AG Charts](https://www.ag-grid.com/charts/)
- Graphics: [Three.js](https://threejs.org/) and [PixiJS](https://pixijs.com/)

## Cross-platform development

- [React Native](https://reactnative.dev/): Native application framework based on React
- [Flutter](https://flutter.dev/): Dart-based multi-platform UI framework
- [Ionic](https://ionicframework.com/): Cross-platform application framework built on web technologies and WebView

## Developer services

- [CodePen](https://codepen.io/) and [JSFiddle](https://jsfiddle.net/) for browser-based examples
- [Transform](https://transform.tools/) for developer data and code conversion
- [Bitly](https://bitly.com/) for short URLs
- [Lorem Picsum](https://picsum.photos/) for placeholder images

## AI development

- [AI SDK](https://ai-sdk.dev/): TypeScript toolkit for AI applications and agents
- [LM Studio](https://lmstudio.ai/): Local AI model runtime
- [Hugging Face](https://huggingface.co/): Community for models, datasets, and AI applications
- [OpenRouter](https://openrouter.ai/): Unified API platform for multiple AI models

## Git and releases

- [Git](https://git-scm.com/) and the official [Git Cheat Sheet](https://git-scm.com/cheat-sheet)
- [GitHub Flow](https://docs.github.com/get-started/using-github/github-flow) for short-lived branches and pull requests
- [Trunk Based Development](https://trunkbaseddevelopment.com/) for frequent integration into the main branch
- [Semantic Versioning](https://semver.org/) and [Conventional Commits](https://www.conventionalcommits.org/)
- [Shields.io](https://shields.io/) and [Badgen](https://badgen.net/) for repository badges

## Created by

Created and maintained by [Dokkabi Club](https://dokkabiclub.dev/?utm_source=github&utm_medium=referral&utm_campaign=tech-stack-handbook).

## License

Copyright © 2026 Lee Jihye. This work is licensed under the [Creative Commons Attribution 4.0 International License](LICENSE).
