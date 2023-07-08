# Stack

The complete primary stack are JavaScript, TypeScript, Node.js, React, Remix, Remix Auth, Tailwind CSS, Radix UI, Zod, Conform, Prisma ORM, PlanetScale, and Vercel. Also aim to prioritize which has open source option, free-tier, or freemium.

Legends:

- 🎩 = Prioritized (_top hat_)
- 🧰 = Required or should not be changed (_toolbox_)
- 🎉 = 3rd party service or platform (_party popper_)
- 🧩 = Optional or interchangeable (_puzzle piece_)
- 💎 = Available as open source (_gem stone_)
- 🚧 = Still in development or not available yet (_construction_)

If this is too much, just focus on the things with the 🧰 (_toolbox_) emoji.

Reminder:

> "Software is a just a tool to help accomplish something for people - many programmers never understood that. Keep your eyes on the delivered value, and don’t over focus on the specifics of the tools" — John Carmack

---

## Tech Stack

### Base

- [GitHub](https://github.com): repository 🎩🧰
- [JavaScript](https://developer.mozilla.org/javascript): main language 🎩🧰
- [TypeScript](https://typescriptlang.org) v5: typed language 🎩🧰💎
- [Node.js](https://nodejs.org) v20+: JavaScript runtime 🎩🧰💎
- [Turborepo](https://turbo.build/repo): monorepo and build tool 🎩🧰💎
- [pnpm](https://pnpm.io) v8+: package manager 🎩🧩💎

### App

- [React](https://react.dev) v18: UI library 🎩🧰💎
- [Remix](https://remix.run) v1-v2: web framework 🎩🧰💎

### Styling and Components

- [Tailwind CSS](https://tailwindcss.com) v3: styling 🎩🧰💎
- [Radix UI](https://radix-ui.com): unstyled UI components 🎩🧩💎
  - [Headless UI](https://headlessui.dev): unstyled UI components 🧩💎
  - [Ariakit](https://ariakit.org): unstyled UI components 🧩💎
  - [shadcn UI](https://github.com/shadcn/ui): styled UI components 🎩🧩💎
- [Icones](https://icones.js.org): icon search 💎
  - [Lucide](https://lucide.dev): icon set 💎
  - [Iconoir](https://iconoir.com): icon set 💎
  - [Phosphor](https://phosphoricons.com): icon set 💎
- [Fontsource](https://fontsource.org): web fonts 🎩💎
- [TanStack Table](https://tanstack.com/table): unstyled table grid component 🚧🧩💎
- [React Email](https://react.email): email styling 🚧🧩💎

### Form Handling and Data Validation

- [Conform](https://conform.guide): full stack validated form handling 🎩🧰💎
- [Zod](https://zod.dev): data validation 🎩🧰💎
  - [Zodix](https://github.com/rileytomasek/zodix) 💎
  - [zod-form-data](https://npmjs.com/package/zod-form-data) 💎

Alternatives:

- [Remix Forms by Seasoned](https://remix-forms.seasoned.cc) 💎

### Data, Database, ORM

- [Prisma ORM](https://prisma.io) v4: database ORM 🎩🧰💎
- [MySQL](https://mysql.com) v8: database management system 🎩🧰💎
- [PlanetScale](https://planetscale.com): MySQL platform 🎩🧩🎉💎
- [Tier](https://tier.run): Pricing data management 🎩🧰💎

Alternatives:

- [Drizzle ORM](https://orm.drizzle.team) 💎

### Data: Cache and Rate Limiter

- [Upstash](https://upstash.com) 🧩🎉🚧

### Auth Provider

- [Remix Auth](https://github.com/sergiodxa/remix-auth) 🎩🧰💎

Alternatives:

- [Lucia](https://lucia-auth.com) 🧩💎
- [Clerk](https://clerk.dev) 🧩🎉

### Tools: Repository

- [GitHub](https://github.com) 🎩🧰🎉

### Tools: Code Quality

- [Prettier](https://prettier.io): code formatter 🧰💎
- [ESLint](https://eslint.org): code linter 🧰💎
- [Stylelint](https://stylelint.io): styling linter 🧰💎

Alternatives:

- [dprint](https://dprint.dev): blazing fast code formatter 💎

### Tools: Deployment

- [Vercel](https://vercel.com) 🧰🧩🎉

Alternatives:

- [Render](https://render.com) 🧩🎉
- [Railway](https://railway.app) 🧩🎉
- [Fly](https://fly.io) 🧩🎉
- [Google Cloud](https://cloud.google.com) 🧩🎉
- [Amazon Web Services (AWS)](https://aws.amazon.com) 🧩🎉

### Tools: Domain and DNS and SSL/TLS

- [Cloudflare](https://cloudflare.com) 🧩🎉
  - Domain
  - DNS

### Tools: Environment Variable/Secret

- [Doppler](https://doppler.com) 🧩🎉

Alternatives:

- [Dotenv](https://dotenv.org) 🧩🎉
  - [EnvShare](https://envshare.dev) 🧩🎉

### Tools: Analytics

- [Vercel Analytics](https://vercel.com/docs/concepts/analytics) 🎩🧩🎉
  - Enable it on your Vercel projects dashboard
  - [Vercel Pro](https://vercel.com/docs/concepts/payments-and-billing/pro) to have easier code review with preview deployments, also use shared build cache from Turborepo

Alternatives:

- [Posthog](https://posthog.com): product platform and data tools 🧩🎉💎
- [Jitsu](https://jitsu.com): data pipeline and ingestion 🚧🧩🎉💎

### Tools: Image

#### Placeholder Images

- [Dicebear](http://dicebear.com): avatar placeholder 🧩🎉💎

#### Stock Images

- [Unsplash](http://unsplash.com): image placeholder 🚧🧩🎉

#### Upload Images and assets

- [Uploadcare](https://uploadcare.com): assets management 🎩🧩🎉

Alternatives:

- [ImageKit](https://imagekit.io): assets management 🚧🧩🎉
- [Cloudinary](https://cloudinary.com): assets management 🚧🧩🎉
- [UploadThing](http://uploadthing): upload management 🚧🧩💎

#### Maps

- [Mapbox](https://mapbox.com) 🚧🧩
  - [Mapbox GL JS](https://github.com/mapbox/mapbox-gl-js) 🚧🧩💎
  - [`react-map-gl`](https://visgl.github.io/react-map-gl) 🚧🧩💎

### Tools: Video

- [Mux](https://mux.com): video streaming and management 🚧🧩🎉

### Tools: Transactional Email 🚧

- [Resend](https://resend.com) 🎩🧰🧩🎉🚧
- [Mailjet](https://mailjet.com) 🧩🎉🚧

### Tools: Marketing Email 🚧

- [ConvertKit](https://convertkit.com) 🧩🎉🚧
- [Bento](https://bentonow.com) 🧩🎉🚧

### Tools: Payment 🚧

- [Lemon Squeezy](https://lemonsqueezy.com) 🧩🎉🚧

Alternatives:

- [Paddle](https://paddle.com) 🧩🎉🚧
- [Stripe](https://stripe.com) 🧩🎉🚧

### Tools: Testing 🚧

- [Vitest](https://vitest.dev) 🚧🧩💎
- [Testing Library](https://testing-library.com) 🚧🧩💎
- [Mock Service Worker (MSW)](https://msw.io) 🚧🧩💎
- [Playwright](https://playwright.dev) 🚧🧩💎
- [Ladle](https://ladle.dev) 🚧🧩

### Tools: Container

- [Docker](http://www.docker.com): container 🧩💎
  - [Docker Compose](https://docs.docker.com/compose) v3: multiple container 🧩💎
  - [Docker Hub](https://hub.docker.com) 🚧🧩💎

### Tools: Monitoring

- [Better Uptime](https://betteruptime.com) 🧩🎉
- [Hyperping](https://hyperping.io) 🧩🎉
- [Instatus](https://instatus.com) 🧩🎉

### Tools: Log Management

- [Axiom](https://axiom.co) 🧩🎉

### Tools: Error Reporting and Analysis

- [Highlight](https://highlight.io) 🧩🎉
- [Sentry](https://sentry.io) 🧩🎉

### Tools: SEO

- [Google Search Console](https://search.google.com/search-console/about) 🧩🎉
  - Check the sitemap and SERP-related stuffs

### Tools: Workflow

- [Kodiak](https://github.com/marketplace/kodiakhq): automate GitHub pull requests 🧩🎉
- [Socket Security](https://github.com/marketplace/socket-security): prevent malicious open source dependencies from infiltrating your apps 🧩🎉

---

## Extra

Especially when require a separate backend app, server, or service.

### REST API

- [NestJS](https://nestjs.com)
  - [Express](https://expressjs.com)
  - [Fastify](https://fastify.io)

### GraphQL

- [GraphQL](https://graphql.org)
- [GraphQL Yoga](https://github.com/dotansimha/graphql-yoga)
  - [Express](https://expressjs.com)
- [Pothos](https://github.com/hayes/pothos)

### tRPC

- [tRPC](https://trpc.io)

### Auth

- [Passport](https://passportjs.org)

---

## Misc Tools

Especially when work with a management in place as a team. Everything here is optional 3rd party services 🧩🎉.

### Tools: Email

- [Skiff](https://skiff.com)
  - [Skiff Mail](https://skiff.com/mail)
  - [Skiff Calendar](https://skiff.com/calendar)
  - [Skiff Drive](https://skiff.com/drive)
  - [Skiff Pages](https://skiff.com/pages)

> 💡 Connect Skiff Mail to Cloudflare Domain and DNS for free custom domain email

### Tools: Credentials

- [Bitwarden](https://bitwarden.com)

### Tools: Data

- [Airtable](https://airtable.com)

### Tools: Social Media

- [YouTube](https://youtube.com) with [Google Account](https://google.com/account/about)
  - Use existing email created with Skiff
  - Use Brand Account for the Channel
