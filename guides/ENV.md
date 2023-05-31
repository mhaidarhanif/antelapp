# ENV

Before running the project anywhere, setup the environment variables or secrets. Keep in mind they are used in different places such as local/development, staging/preview, and production (such as Vercel).

In local development, to manage the environment variables, use either:

- Plain `.env` file, based on `.env.example` file
- Secrets management platform such as Doppler or Dotenv, [as listed in the stack](STACK.md)

In production, use their provided settings. Can also sync with Doppler or Dotenv.

The client and server environment variables are managed in `packages/env` so we use it like this. Therefore we won't accidentally access `process.env`.

```ts
import { env } from "env";

console.log(env.HELLO_WORLD);
console.log(env.NEXT_PUBLIC_HELLO_WORLD);
```

The `env` package exports a type-safe environment variables using [t3-env](https://env.t3.gg) and [Zod](https://zod.dev).

Notes:

- Don't read the environment variables directly from `process.env`.
- Only edit the `packages/env/.env` file if you want to add, edit, or remove environment variables. Keep the `packages/env/.env` as the single source
- Use `env.NEXT_PUBLIC_<name>` if you want to read the variable from a Client component. If you read a `env.<name>` variable from a Client component, you'll get error.
- If you make changes to server environment variables or the client environment variables, you need to edit the `packages/env/src/index.ts` file too.

## Options

### If using `.env` fie

```sh
cp -i .env.example .env
# -i or --interactive will ask before overwrite
```

Then edit `.env` as needed.

### If using secrets management platform

Alternatively, it's recommended to use [Doppler](https://doppler.com), or
[Dotenv](https://dotenv.org), or something similar to manage the credentials.

```sh
doppler login

# ? Select an option: Overwrite global login (/)
# ? Open the authorization page in the browser? Yes
# Complete authorization at https://dashboard.doppler.com/workplace/auth/cli
# The auth code is:
# Waiting...
# Welcome, User Name
```

```sh
doppler setup

# ? Select a project: project-name
# ? Select a config: env
# ┌─────────┬─────────┬───────────────┐
# │ NAME    │ VALUE   │ SCOPE         │
# ├─────────┼─────────┼───────────────┤
# │ config  │ dev     │ /path/to/repo │
# │ project │ name    │ /path/to/repo │
# └─────────┴─────────┴───────────────┘
```

To use the secrets directly without `.env` file:

```sh
doppler -- pnpm <command>
```

To download the secrets into the `.env` file:

```sh
doppler secrets download --no-file --format env > .env
```

## Variables

### Required

```sh
DATABASE_URL="mysql://example_username:example_password@region.connect.psdb.cloud/example_database?sslaccept=strict"
```

`DATABASE_URL` is the primary database used with Prisma ORM. Get it from either:

- Local database or Docker container via [Docker compose](../docker-compose.yaml) for development
- [PlanetScale](https://planetscale.com/docs/concepts/connection-strings) for production and staging

### Optionals

Optionals because they have default values in the config.

#### Session Secret

For cookie after authenticated or logged in.

```sh
SESSION_SECRET="the_remix_session_secret"
```

Can be generated more securely using OpenSSL:

```sh
openssl rand -base64 32
```

#### Uploadcare

Upload image assets solution. Used with [Uploadcare's file uploader widget](packages/ui/uploadcare.tsx). Get it from [Uploadcare](https://uploadcare.com/docs/start/settings)

```sh
UPLOADCARE_PUBLIC_KEY="the_uploadcare_public_key"
```

#### Mapbox

Map image view and picker

```sh
MAPBOX_PUBLIC_TOKEN="the_mapbox_public_token"
```

#### Google Analytics

Google Analytics.

```sh
GA_MEASUREMENT_ID="the_ga_id"
```

#### Sentry

Error reporting.

```sh
SENTRY_BROWSER_DSN="the_sentry_dsn"
```

#### Posthog

Product analytics.

```sh
POSTHOG_API_HOST="the_posthog_api_host"
POSTHOG_API_KEY="the_posthog_api_key"
```
