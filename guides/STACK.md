# Stack

The complete primary stack are Node.js, TypeScript, Remix, Remix Auth, React, Tailwind CSS, Radix UI, Zod, Conform, Prisma ORM, PlanetScale, and Vercel. We also aim to prioritize which has open source option, free-tier, or freemium.

Legends:

- 🧰 = required or should not be changed
- 🎉 = 3rd party service or platform
- 🧩 = optional or interchangeable
- 💠 = available as open source
- 🚧 = still in development or not available

Reminder:

> "Software is a just a tool to help accomplish something for people - many programmers never understood that. Keep your eyes on the delivered value, and don’t over focus on the specifics of the tools" — John Carmack

## Base

- [JavaScript](https://developer.mozilla.org/javascript): main language 🧰
- [TypeScript](https://typescriptlang.org) v5: typed language 🧰💠
- [Node.js](https://nodejs.org) v18+: JavaScript runtime 🧰💠
- [pnpm](https://pnpm.io) v8+: package manager 🧩💠
- [Turborepo](https://turbo.build/repo): monorepo and build tool

## App

- [React](https://react.dev) v18: UI library 🧰💠
- [Remix](https://remix.run) v1-v2: web framework 🧰💠

## Styling and Components

- [Tailwind CSS](https://tailwindcss.com) v3: styling 🧰💠
- [Fontsource](https://fontsource.org): web fonts 🧰
- [Radix UI](https://radix-ui.com): unstyled UI components 🧰🧩💠
  - [Headless UI](https://headlessui.dev): unstyled UI components 🧩💠
  - [Ariakit](https://ariakit.org): unstyled UI components 🧩💠
  - [shadcn UI](https://github.com/shadcn/ui): styled component library 🧩💠
- [Icones](https://icones.js.org): icon search 💠
  - [Lucide](https://lucide.dev): icon set 💠
  - [Iconoir](https://iconoir.com): icon set 💠
- [React Email](https://react.email): email styling 🚧🧩💠
- [TanStack Table](https://tanstack.com/table): unstyled table grid component 🚧🧩💠

## Form Handling and Data Validation

- [Conform](https://conform.guide): form handling 🧰💠
- [Zod](https://zod.dev): data validation 🧰💠
  - [Zodix](https://github.com/rileytomasek/zodix) 🧩💠
  - [zod-form-data](https://npmjs.com/package/zod-form-data) 🧩💠

## Database and ORM

- [Prisma ORM](https://prisma.io) v4: database ORM 🧰💠
- [MySQL](https://mysql.com) v8: database management system 🧰💠
- [PlanetScale](https://planetscale.com): MySQL platform 🧩🎉💠

## Auth Provider

- [Remix Auth](https://github.com/sergiodxa/remix-auth) 🧰💠
  - [Lucia](https://lucia-auth.com) 🧩💠
  - [Clerk](https://clerk.dev) 🧩🎉

## Tools: Code Quality

- [Prettier](https://prettier.io): code formatter 🧰💠
- [ESLint](https://eslint.org): code linter 🧰💠
- [Stylelint](https://stylelint.io): styling linter 🧰💠

## Tools: Deployment

- [Vercel](https://vercel.com) 🧰🧩🎉
- [Fly](https://fly.io) 🧩🎉
- [Render](https://render.com) 🧩🎉
- [Railway](https://railway.app) 🧩🎉
- [Google Cloud](https://cloud.google.com) 🧩🎉
- [Amazon Web Services (AWS)](https://aws.amazon.com) 🧩🎉

## Tools: Domain and DNS and SSL/TLS

- [Cloudflare](https://cloudflare.com) 🧩🎉

## Tools: Environment Variable/Secret

- [Doppler](https://doppler.com) 🧩🎉
- [Dotenv](https://dotenv.org) 🧩🎉
  - [EnvShare](https://envshare.dev) 🧩🎉

## Tools: Analytics

- [Vercel Analytics](https://vercel.com/docs/concepts/analytics) 🧩🎉
  - Enable it on your Vercel projects dashboard
  - [Vercel Pro](https://vercel.com/docs/concepts/payments-and-billing/pro) to have easier code review with preview deployments, also use shared build cache from Turborepo
- [Posthog](https://posthog.com): product platform and data tools 🧩🎉💠
- [Jitsu](https://jitsu.com): data pipeline and ingestion 🚧🧩🎉💠

## Tools: Image

- Placeholders
  - [Dicebear](http://dicebear.com): avatar placeholder 🧩🎉💠
- Stock
  - [Unsplash](http://unsplash.com): image placeholder 🚧🧩🎉
- Upload and assets
  - [Uploadcare](https://uploadcare.com): assets management 🧩🎉
  - [ImageKit](https://imagekit.io): assets management 🚧🧩🎉
  - [Cloudinary](https://cloudinary.com): assets management 🚧🧩🎉
  - [UploadThing](http://uploadthing): upload management 🚧🧩💠
- Maps
  - [Mapbox](https://example.com) 🚧🧩💠
  - [`mapbox-gl`](https://example.com)
  - [`react-map-gl`](https://example.com)

## Tools: Video

- [Mux](https://mux.com): video streaming and management 🚧🧩🎉

## Tools: Transactional Email 🚧

- [Resend](https://resend.com) 🚧🧩🎉
- [Mailjet](https://mailjet.com) 🚧🧩🎉

## Tools: Marketing Email 🚧

- [ConvertKit](https://convertkit.com) 🚧🧩🎉
- [Bento](https://bentonow.com) 🚧🧩🎉

## Tools: Cache and Rate Limiter

- [Upstash](https://upstash.com) 🚧🧩🎉

## Tools: Payment 🚧

- [Lemon Squeezy](https://lemonsqueezy.com) 🚧🧩🎉
- [Paddle](https://paddle.com) 🚧🧩🎉
- [Stripe](https://stripe.com) 🚧🧩🎉

## Tools: Testing 🚧

- [Vitest](https://vitest.dev) 🚧🧩💠
- [Testing Library](https://testing-library.com) 🚧🧩💠
- [Mock Service Worker (MSW)](https://msw.io) 🚧🧩💠
- [Playwright](https://playwright.dev) 🚧🧩💠
- [Ladle](https://ladle.dev) 🚧🧩

## Tools: Container

- [Docker](http://www.docker.com): container 🧩💠
  - [Docker Compose](https://docs.docker.com/compose) v3: multiple container 🧩💠
  - [Docker Hub](https://hub.docker.com) 🚧🧩💠

## Tools: Monitoring

- [Better Uptime](https://betteruptime.com) 🧩🎉
- [Hyperping](https://hyperping.io) 🧩🎉
- [Instatus](https://instatus.com) 🧩🎉

## Tools: Log Management

- [Axiom](https://axiom.co) 🧩🎉

## Tools: Error Reporting and Analysis

- [Highlight](https://highlight.io) 🧩🎉
- [Sentry](https://sentry.io) 🧩🎉

## Tools: SEO

- [Google Search Console](https://search.google.com/search-console/about) 🧩🎉
  - Check the sitemap and SERP-related stuffs

## Tools: Workflow

- [Kodiak](https://github.com/marketplace/kodiakhq): automate GitHub pull requests 🧩🎉
- [Socket Security](https://github.com/marketplace/socket-security): prevent malicious open source dependencies from infiltrating your apps 🧩🎉

---

# Extra

Only require a separate backend app, server, or service.

## REST API

- [NestJS](https://nestjs.com)
  - [Express](https://expressjs.com)
  - [Fastify](https://fastify.io)

## GraphQL

- [GraphQL](https://graphql.org)
- [GraphQL Yoga](https://github.com/dotansimha/graphql-yoga)
  - [Express](https://expressjs.com)
- [Pothos](https://github.com/hayes/pothos)

## tRPC

- [tRPC](https://trpc.io)

## Auth

- [Passport](https://passportjs.org)
