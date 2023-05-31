# ROADMAP

## User Features

- [x] Premade contents
- [x] Light and dark mode theme
- [x] Site layout and routes/pages
- [x] Admin dashboard and metrics/statistics
- [x] Register, log in, log out
  - [x] Data validation and check availability
  - [ ] Send welcome or verification email
- [x] Public pages and search
- [x] User dashboard, profile, settings
  - [x] Manage notes (create, read, update, delete, search)
  - [x] Change profile and avatar image
  - [x] Change email
  - [x] Change and reset password
  - [ ] Notification
- [x] Admin dashboard and search
  - [x] Manage users, notes, etc
- [x] Various others
  - [x] Share URL with preview image from Open Graph
  - [x] Add to home screen as app on mobile
  - [x] Search data
    - [ ] Full text search
  - [x] Upload and manage image assets
  - [ ] Map viewer

## Developer Setup

- [x] Full stack type safety with Remix, TypeScript, Zod
  - [x] Follow the practices from the official docs and popular Remix Stacks
  - [x] v2 future flags while still in v1
    - [x] v2 flat routes convention
    - [x] v2 meta data management
    - [x] v2 normalized form method
    - [x] v2 error boundary
    - [x] Tailwind CSS and PostCSS support
    - [x] New dev server with config for HMR/HDR (hot module/data reload)
- [x] More than 50 of ready to use and 100% customizable UI components
  - [x] Layouts and demo examples
  - [ ] Rich text or WYSIWYG editor with TipTap
  - [ ] Keyboard shortcuts with cmdk
- [x] Preselected styles, colors, fonts, icons, and responsive design
  - [x] Customize in Tailwind Config, for brand (primary) and surface (secondary) colors
  - [x] Default avatar image with Dicebear API
  - [x] Icon set system to avoid name conflict
    - [x] Lucide
    - [x] Iconoir
    - [ ] Bring your own favorite
- [x] Database with Prisma ORM and MySQL on PlanetScale
  - [x] tRPC-style or GraphQL-style data models file structure
- [x] Auth with Remix Auth using a session cookie
- [x] Data validation with Zod for general and Zodix for Remix loader/action
- [x] Form handling with Conform
  - [x] Check for unallowed usernames
  - [x] Upload file to Uploadcare
  - [ ] Redirect to previous route
  - [ ] Password strength meter
- [ ] Image hosting integration
- [ ] Email delivery system
  - [ ] Transactional email with Mailjet/Resend and React Email
  - [ ] Marketing email with ConvertKit/Bento
- [x] SEO functions with meta tags
  - [x] `robots.txt`
  - [x] `canonical` tag
  - [x] `sitemap.xml` generator
  - [x] Open Graph and Twitter card
- [x] Various utilities with external libraries
  - [x] Root loader data for env, theme, user, etc
  - [x] Cache control header
- [x] Lighthouse score or Pagespeed Insights optimized
  - [x] No CLS on loading screens/skeletons, only loading bar on top and loading button state
- [x] ESM, pnpm, Prettier, ESLint, Stylelint, and many more
- [x] [GitHub-related files](../.github): issue template, PR template, codeowners, funding
- [x] [VS Code-related files](../.vscode): extensions, settings, launch config

## UI Components

- [ ] Button Group
- [x] Badge
- [x] Breadcrumbs
- [ ] Combobox
- [ ] List Group
- [x] Progress Bar
- [ ] Ribbon
- [ ] Toast
- [ ] Tags
- [ ] Table
- [x] Avatar
- [ ] Divider
- [x] Chip
- [ ] Drawer
- [ ] Slider
- [ ] Multi-Modal
