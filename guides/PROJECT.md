# PROJECT

## Monorepo

When working with monorepo, here are some important aspects to be aware of:

- How to manage and upgrade all dependencies faster? ncu (npm-check-updates)
- How to manage and use environment variables (global env) in the apps?
- How to manage shared assets and images?
- How to enable/disable build cache on local?
- How to resolve "failed to contact turbod"?
- How to manage Tailwind CSS config and styles?
- How to deploy on Vercel or other places properly?
- Do we need to sync different dependencies in apps and packages? Like TypeScript? Yes
- Do we need to cache tasks related to Prisma? No

## Project Structure

- `apps`
  - `web`: Default main app with Remix (SSR)
  - `play`: Playground app to experiment with Remix (SSR)
  - `docs`: Documentation app with Next.js and MDX (SSR)
  - `admin`: Admin app with React and React Router with Vite (no SSR)
- `packages`
  - `ui`: Styled UI component library
  - `database`: Database schema/model and client of Prisma
  - `tsconfig`: Shared TypeScript config
  - `eslint-config-custom`: Shared ESLint config
  - `utils`: Reusable utilities
  - `hooks`: Reusable React Hooks
  - `configs`: Global app configuration
  - `domains`: Domain layer or business logic

There are several packages because each of them can be used or not separately across different apps.

## Name

Key ideas to decide the project/product name:

- Brandable: Google, IKEA
- Word combination: YouTube, Facebook
- Word blend (Portmanteau): Brunch, Instagram, Pinterest, FedEx
- Alternate spellings: Dribbble, Lyft, Fiverr
- International: Toyota, Nissan, Audi
- Random: Be Creative 🎨

Use [oneword.domains](https://oneword.domains) to help decide the domain TLD.
