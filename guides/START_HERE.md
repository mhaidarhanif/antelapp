# START HERE

These are the recommended steps to build a real production application:

1. Goal
2. User Experience
3. User Interface
4. Data Modeling
5. Backend Implementation
6. Frontend Implementation
7. Deployment
8. Presentation
9. Maintenance

## 1. Goal

Set the application goal and its effect on the business.

Write it down with Markdown on the README, then push the repo to a Git repo with GitHub or GitLab.

## 2. User Experience

Specify the User Experience (UX) or business logic to accomplish the goal.

Write the documentation (docs), arrange the flow with a chart with Eraser.io, or map the user journey with Miro.

## 3. User Interface

Design the User Interface (UI) that will be used by the end users, and then the other type of users. Use UI design tool with Figma or Framer.

## 4. Data Modeling

Model the database schema with Prisma. Then push or migrate it to the database of choices like MySQL or PostgreSQL; either set it up manually or use a platform like PlanetScale, Neon, or Supabase.

## 5. Backend Implementation

Implement the backend or server-side layer.

With Remix or Next.js, they provide a backend layer without separating the backend from another app service.

With NestJS to create REST API, or GraphQL Yoga to create GraphQL API.

## 6. Frontend Implementation

Implement the frontend or client-side layer and UI components that have already been designed before.

With Remix or Next.js, the components use React.

With plain React components with client-side only or Single Page Applications (SPA), better to use Vite

## 7. Deployment

Deploy the services for the backend, frontend, or full stack.

Use Vercel or Netlify to deploy the frontend, full stack, or included with a serverless backend.

Use Render.com or Railway.app to deploy the backend if separated or served in a long-running server.

Use Google Cloud or Amazon Web Services (AWS) to handle the whole infra.

## 8. Presentation

Present or showcase the app to the actual users.

Create a brief explanation, demo video, or slide deck that highlights the features, benefits, and impact of the application.

Use Apple Keynote, Google Slides, Microsoft PowerPoint, or Slidev.

## 9. Maintenance

Maintain the application by improving existing functionalities, fixing bugs, adding new features, updating dependencies, and optimizing performance.

Continually gather feedback from users and iterate on the application to improve the user experience and accomplish the goal.

Use various tools like Better Uptime to monitor the service uptime, Sentry to track errors, Dependabot to update dependencies, and Google Lighthouse to measure performance.

## 10. Celebration

🥳 Congratulations! 🎉
