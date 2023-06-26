# DEPLOYMENT

## Vercel

On Vercel, select the framework preset to Remix.

Override the "Build Command" to be:

```
cd ../../ && pnpm turbo build --filter=web...
```

Set "Root Directory" to be:

```
apps/web
```

Check:

- [x] Include source files outside of the Root Directory in the Build Step.

### Other Setup

- Go to vercel.com
- Deploy
- Congratulations!
- Go to "Project Settings"
  - Go to "General" tab to check if everything's okay
  - Go to "Domains" tab to setup the domains
  - Go to "Integrations" tab to setup:
    - Doppler
    - After this go to "Environment Variables" tab to check if everything's okay
  - Go to "Functions" tab then change the "Function Region" that's closer to your location
  - Go to "Cron Jobs" tab to check if everything's okay

### Env

Setup the environment variables as [explained in the development process](DEVELOPMENT.md) for the corresponding deployment server, like Vercel.

The recommended way is to use integration between Vercel and Doppler:

- [Vercel Integration on Doppler](https://doppler.com/integrations/vercel)
- [Doppler Integration on Vercel](https://vercel.com/integrations/doppler)

### Build

To make it automatic for Vercel CI to push the database schema changes (especially to PlanetScale) while building for Preview and Production, use the `ci` command/script instead of regular `build`.

Put this into the **Build Command** in the **Project Settings**:

```sh
pnpm ci
```

### Turbo Ignore

https://vercel.com/changelog/intelligent-ignored-builds-using-turborepo

## Domain and DNS

The recommended way is to use either:

- [Vercel Domain](https://vercel.com)
- [Cloudflare Domain](https//cloudflare.com)
- [Cloudflare DNS](https//cloudflare.com)
  - Can connect to any domain registrar
