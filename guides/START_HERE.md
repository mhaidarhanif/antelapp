# START HERE

To build a real production application, these are the recommended steps:

1. Goal
2. User Experience
3. User Interface
4. Data Modeling
5. Backend Development
6. Frontend Development
7. Deployment
8. Presentation
9. Maintenance
10. Celebration

## 1. Goal

Set the application goal and its effect on the business to solve a very specific problem.

- [ ] Write it down with [Markdown](https://markdownguide.org) on the README.
- [ ] Then push the repo to a [Git](https://git-scm.com) repo with [GitHub](https://github.com) or [GitLab](https://gitlab.com).
- [ ] Complete more details especially the most important features, tech stack, and the team members if any.

While on it:

- [ ] Choose a project or product name.
- [ ] Define the branding aspects such as the logo, colors, fonts, styles, and more.
- [ ] Even better to prepare the domain as well.
  - [ ] Use [Cloudflare](https://cloudflare.com/products/registrar) Domain Registrar and DNS management.

Especially more important if you work with a team, company, or organization.

## 2. User Experience

Specify the User Experience (UX) or business logic to accomplish the goal.

- [ ] Write the documentation (docs) about the expectation.
- [ ] Arrange the flow with a diagram or chart with [Excalidraw](https://excalidraw.com), [Eraser.io](https://eraser.io), or [FigJam](https://figma.com/figjam).
- [ ] Map the user journey with [Miro](https://miro.com).
- [ ] Make sure to aligns with the goal.

Usually the basic CRUD features:

- [ ] Show, list, or get resources/items
- [ ] Create a new resource/item
- [ ] Update existing resource/item
- [ ] Delete existing resource/item
- [ ] Search or filter resources/items with a keyword

Especially more important if some specific algorithms or data structures would be the core of the app.

## 3. User Interface

Design the User Interface (UI) that will be used by the end users, and then the other type of users.

- [ ] Use UI design tool with [Figma](https://figma.com) or [Framer](https://framer.com).
- [ ] Make sure to aligns with the goal and UX.

The variety of design formats:

- [ ] Sketch
- [ ] Wireframe
- [ ] Mockup
- [ ] Prototype

The important design artifacts:

- [ ] Pages such as home or landing page, about, auth (register/login), and various pages to use the app that comply with the core UX.
- [ ] Layouts such as navigation, header, content, footer, form, and more.

## 4. Data Modeling

Model the database schema to define the tables, fields, data types, and more.

- [ ] Use a diagram tool for quick collaboration.
- [ ] Use the [Prisma](https://prisma.io) Schema file directly.
- [ ] Set up the database with [MySQL](https://mysql.com) or [PostgreSQL](https://postgresql.org) using a [Docker](https://docker.com) container and [Docker Compose](https://docker.com/compose).
  - [ ] Run it locally or in production with a cloud service.
  - [ ] Can also use a platform like [Render](https://render.com), [Railway](https://railway.app), [PlanetScale](https://planetscale.com), [Neon](https://neon.tech), [Supabase](https://supabase.com), or your favorite.
  - [ ] In case there is a specific case like caching, [Redis](https://redis.com) can also help, and a platform like [Upstash](https://upstash.com) or [Vercel KV](https://vercel.com/storage/kv).
- [ ] Then push or migrate the schema to the database.

## 5. Backend Development

Implement the backend or server-side layer.

For the backend app or API service:

- [ ] With [Remix](https://remix.run) or [Next.js](https://nextjs.org), they provide a backend layer without having a separate backend.
- [ ] With [NestJS](https://nestjs.com) to create REST API or [GraphQL Yoga](https://the-guild.dev/graphql/yoga-server) to create [GraphQL](https://graphql.org) API.

For the API documentation:

- [ ] If building a full stack app without a separate backend, the routes would speak for themselves.
- [ ] If building a REST API, there should be either simple API documentation on the README or auto-generated docs with [Swagger](https://swagger.io).
- [ ] If building a GraphQL API, the docs should be accessible via the GraphQL Schema.

Make sure to aligns with the goal and UI/UX.

## 6. Frontend Development

Implement the frontend or client-side layer and UI components that have already been designed before.

For the frontend app:

- [ ] Plan for the routes or pages.
- [ ] With [Remix](https://remix.run) or [Next.js](https://nextjs.org), the components use [React](https://react.dev) and might be a Multi Page Application (MPA).
- [ ] With [Vite](https://vitejs.dev), the React components are client-side only or become a Single Page Application (SPA).

For the styling:

- [ ] Use [Tailwind CSS](https://tailwindcss.com) and some plugins.
- [ ] Use unstyled React components like [Radix UI](https://radix-ui.com), [Headless UI](https://headlessui.com), or [Ariakit](https://ariakit.org).
  - [ ] Use the provided Anison UI that adapted from [shadcn UI](https://ui.shadcn.com) for premade UI components.

Make sure to aligns with the goal and UI/UX.

## 7. Deployment

Deploy the services for the backend, frontend, or full stack. This can also be done simultaneously while in development from the very beginning.

- [ ] Use [Vercel](https://vercel.com) or [Netlify](https://netlify.com) to deploy the frontend, full stack, or included with a serverless backend.
- [ ] Use [Render](https://render.com) or [Railway](https://railway.app) to deploy the backend if separated or served in a long-running server.
- [ ] Use [Google Cloud](https://cloud.google.com) or [Amazon Web Services (AWS)](https://aws.amazon.com) to handle the whole infrastructure.
- [ ] Use Continuous Integration/Delivery (CI/CD) with [GitHub Actions](https://github.com/features/actions), [GitLab CI](https://docs.gitlab.com/ee/ci), or [Circle CI](https://circleci.com).

Make sure everything is working, also can be accessed by the expected users by connecting to a domain.

## 8. Presentation

Present or showcase the app to the actual users.

- [ ] Create a brief explanation, demo video, or slide deck that highlights the features, benefits, and impact of the application.
- [ ] Use [Apple Quicktime](https://example.com), [Windows Game Bar](https://example.com), [Open Broadcaster Studio (OBS)](https://example.com), [Screenflow](https://example.com), or [Screen Studio](https://example.com) to record the demo video.
- [ ] Use [Apple Keynote](https://example.com), [Google Slides](https://example.com), [Microsoft PowerPoint](https://example.com), or [Slidev](https://sli.dev) to create the slide deck.

## 9. Maintenance

Maintain the application over time.

- [ ] Improve existing functionalities, fix bugs, add new features, update dependencies, also optimize performance and usability.
- [ ] Continually gather feedback from users and iterate on the application to improve the user experience and accomplish the goal.
- [ ] Use various tools like [Better Uptime](https://example.com) to monitor the service uptime, [Sentry](https://example.com) to track errors, [Dependabot](https://example.com) to update dependencies, and [Google Lighthouse](https://example.com) to measure performance.

## 10. Celebration

🥳 Congratulations! 🎉
