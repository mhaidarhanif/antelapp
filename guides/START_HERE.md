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

## 1. Goal

Set the application goal and its effect on the business to solve a very specific problem.

- Write it down with Markdown on the README.
- Then push the repo to a Git repo with GitHub or GitLab.
- Complete more details especially the most important features, tech stack, and the team members if any.

Especially more important if you work with a team, company, or organization.

## 2. User Experience

Specify the User Experience (UX) or business logic to accomplish the goal.

- Write the documentation (docs) about the expectation.
- Arrange the flow with a diagram or chart with Excalidraw, Eraser.io, or FigJam.
- Map the user journey with Miro.
- Make sure it aligns with the goal.

Especially more imporatnt if there are some specific algorithms or data structures that would be the core of the app.

## 3. User Interface

Design the User Interface (UI) that will be used by the end users, and then the other type of users.

- Use UI design tool with Figma or Framer.
- Make sure it aligns with the goal and UX.

The variety of design formats:

- Sketch
- Wireframe
- Mockup
- Prototype

The important design artifacts:

- Pages such as home or landing page, about, auth (register/login), where to use the app, and more.
- Layouts such as navigation, header, content, footer, form, and more.

## 4. Data Modeling

Model the database schema to define the tables, fields, data types, and more.

- Use diagram tool for quick collaboration.
- Use Prisma Schema file directly.
- Setup the database with MySQL or PostgreSQL using a Docker container.
  - Run it locally or in production with a cloud service.
  - Can also use a platform like Render, Railway, PlanetScale, Neon, Supabase, or your favorite.
  - In case there is a specific case like caching, Redis can also help.
- Then push or migrate it to the database.

## 5. Backend Development

Implement the backend or server-side layer.

For the backend app or API service:

- With Remix or Next.js, they provide a backend layer without having a separated backend.
- With NestJS to create REST API or GraphQL Yoga to create GraphQL API.

For the API docs:

- If building a full stack app without a separated backend, the routes would speak for themselves.
- If building a REST API, there should be either a simple API docs on the README or auto-generated docs with Swagger.
- If building a GraphQL API, the docs should be accessible via the GraphQL Schema.

Make sure it aligns with the goal and UI/UX.

## 6. Frontend Development

Implement the frontend or client-side layer and UI components that have already been designed before.

For the frontend app:

- Plan for the routes or pages.
- With Remix or Next.js, the components are using React.
- With Vite, the React components are client-side only or become a Single Page Application (SPA).

For the styling:

- Use Tailwind CSS and some plugins.
- Use unstyled React components like Radix UI, Headless UI, or Ariakit.
  - Use Anison UI or [shadcn UI](https://ui.shadcn.com) for premade UI components.

Make sure it aligns with the goal and UI/UX.

## 7. Deployment

Deploy the services for the backend, frontend, or full stack. This can also be done simultaneously while in development since the very beginning.

- Use Vercel or Netlify to deploy the frontend, full stack, or included with a serverless backend.
- Use Render.com or Railway.app to deploy the backend if separated or served in a long-running server.
- Use Google Cloud or Amazon Web Services (AWS) to handle the whole infrastructure.

Make sure everything is working and can be accessed by the expected users.

## 8. Presentation

Present or showcase the app to the actual users.

- Create a brief explanation, demo video, or slide deck that highlights the features, benefits, and impact of the application.
- Use Apple Quicktime, Windows Game Bar, Open Broadcaster Studio (OBS), Screenflow, or Screen Studio to record the demo video.
- Use Apple Keynote, Google Slides, Microsoft PowerPoint, or Slidev to create the slide deck.

## 9. Maintenance

Maintain the application over time.

- Improve existing functionalities, fix bugs, add new features, update dependencies, also optimize performance and usability.
- Continually gather feedback from users and iterate on the application to improve the user experience and accomplish the goal.
- Use various tools like Better Uptime to monitor the service uptime, Sentry to track errors, Dependabot to update dependencies, and Google Lighthouse to measure performance.

## 10. Celebration

🥳 Congratulations! 🎉
