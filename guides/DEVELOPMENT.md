# DEVELOPMENT

## Quick Start

Choose your preference to start:

- Generate? [Use this template](https://github.com/haidar-dev/antelapp-dev/generate).
- Clone? `git clone git@github.com:haidar-dev/antelapp.git`
- `npx`? `npx create-remix@latest --template haidar-dev/antelapp`
- [Deploy with Vercel?](https://vercel.com)

In the local repo:

1. `git init` or `git status`
2. `pnpm install` to install dependencies
3. `cp .env.example .env` and setup the environment variables
4. `docker compose up -d` to run the database
5. `pnpm db:setup --filter=database` to push the schema, generate Prisma client, seed some data based on `database` package only
6. `pnpm build` to build all the apps, make sure everything's fine
7. `pnpm dev` to run all the apps for development
   - `pnpm dev:web` to run the web app only

In the browser, either open:

- `localhost:3000` (`web`) for default primary web app (Remix)
- `localhost:3001` (`admin`) for admin (Vite) 🚧
- `localhost:3002` (`docs`) for docs (Next.js + MDX) 🚧
- `localhost:3003` (`play`) for playground (Vite) 🚧
- `localhost:4000` (`graphql`) for GraphQL API (GraphQL Yoga) 🚧
- `localhost:4040` (`rest`) for REST API (NestJS) 🚧

Make sure everything can run first. Then to explore the repo to replace the contents. As this is a template, not a repo generator.

## Install Dependencies

Install dependencies using the preferred package manager agent:

```sh
npm i
yarn i
pnpm i
```

Or use [`@antfu/ni`](https://github.com/antfu/ni) which can detect the lockfile and auto choose npm/yarn/pnpm:

```sh
npm i -g @antfu/ni
yarn add -g @antfu/ni
pnpm i -g @antfu/ni
```

| `ni`    | `npm`      | `yarn`            | `pnpm`      |
| ------- | ---------- | ----------------- | ----------- |
| `ni`    | `npm i`    | `yarn`            | `pnpm i`    |
| `ni -D` | `npm i -D` | `yarn add -D`     | `pnpm i -D` |
| `ni -g` | `npm i -g` | `yarn global add` | `pnpm i -g` |
| `nlx`   | `npx`      | `yarn dlx`        | `pnpm dlx`  |

To install new package to a workspace:

```sh
pnpm i <package_name> --filter=<workspace_name>
```

## Upgrade Dependencies

Install and use `npm-check-updates` to make things easier:

```sh
ni -g npm-check-updates
```

Upgrade everything:

```sh
ncu --deep     # dry run to check version changes
ncu --deep -u  # update all package.json
ni             # install updated dependencies
```

Upgrade interactively:

```sh
ncu --interactive --format group
```

## Prisma ORM and Database Connection

The database/DBMS can be anything that supported by Prisma ORM. Although this repo is already suited to use MySQL on PlanetScale.

> ⚠️ Just don't use SQLite because it doesn't have `@db.Text` annotation and `model.createMany()` function.

### If using PlanetScale

1. [Sign up a free account](https://auth.planetscale.com/sign-up).
2. [Create a database](https://planetscale.com/docs)
3. Get the database URL connection string as `DATABASE_URL`

```sh
DATABASE_URL='mysql://username:pscale_pw_password@region.connect.psdb.cloud/name?sslaccept=strict'
```

### If using local database

Start [Docker](https://docker.com) service with Docker Engine, Docker Desktop, or Orbstack. Then run [Docker Compose](../docker-compose.yml):

```sh
docker compose up -d
```

While in development:

- Generate Prisma types for `@prisma/client` with `nr prisma:generate` (it runs `prisma generate`)
- Check generated Prisma documentation with `nr docs:prisma` (it runs `prisma-docs-generator serve`) then open <http://localhost:5858>
- Visualize the schema with [Prisma Editor](https://github.com/mohammed-bahumaish/prisma-editor) or [Prismaliser](https://prismaliser.app)
- Push Prisma schema changes for PlanetScale with `nr prisma:push` (it runs `prisma db push`)
  - Notice that with [PlanetScale](https://planetscale.com/docs/tutorials/prisma-quickstart) approach with [Prisma](https://prisma.io/docs/guides/database/using-prisma-with-planetscale), we don't need migration files in our repo, but rather managed in their platform.
- Read the [official Prisma docs](https://prisma.io/docs) and [How to Prisma](https://howtoprisma.com)
  - Follow the [PlanetScale & Prisma happy practices](https://planetscale.com/docs/prisma/prisma-best-practices)
  - Can also try [PrismaGPT](https://gpt.howtoprisma.com) to help learn the query.

Check the Prisma Schema examples:

- <https://pris.ly/d/prisma-schema>
- <https://github.com/remix-run/indie-stack/blob/main/prisma/schema.prisma>
- <https://github.com/planetscale/beam/blob/main/prisma/schema.prisma>

### REPL

Use `prisma-repl` to try various things.

## File Upload with Uploadcare

[Uploadcare](https://uploadcare.com) is used to primarily upload, store, and host the uploaded assets, images, and files. If these need to be stored in an account, paste the [Public API key](https://uploadcare.com/docs/start/settings/#keys-public) as `UPLOADCARE_PUBLIC_KEY`.

1. [Create an Uploadcare account](https://uploadcare.com).
2. Go to the Dashboard and get the public key string.
3. Put it as `UPLOADCARE_PUBLIC_KEY` to the environment variables.

## Run Development Server

```sh
nr dev
```

Open up the shown host and ports.

## Language Server and Types

If there are some significant changes in the TypeScript config, ESLint config, or Prisma schema, restart the code editor or just the language servers in the code editor.

## Remix SEO Configuration

As there's no official way yet to handle SEO related output for metadata and sitemap, here are the options ordered by preference:

1. [`balavishnuvj/remix-seo`](https://github.com/balavishnuvj/remix-seo): Collection of SEO utilities like sitemap, robots.txt, etc. for a Remix Application
2. [`chaance/remix-seo`](https://github.com/chaance/remix-seo): A package for easily managing SEO meta and link tags in Remix
3. [`fedeya/remix-sitemap`](https://github.com/fedeya/remix-sitemap): Sitemap generator for Remix applications

## Database backup

Syntax to backup using PlanetScale's `pscale` CLI:

```sh
pscale db dump database_name branch --output database_name.dump
```

## Notes

Look up for these comments:

- `EDITME`: Edit them as needed
- `TODO`: Still in progress

[Customize the GitHub repo social preview](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/customizing-your-repositorys-social-media-preview)
