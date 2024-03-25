## Install Medusa with create-medusa-app

Medusa is a toolkit for developers to create digital commerce applications. In its simplest form, Medusa is a Node.js backend with the core API, plugins, and modules installed through npm.

```bash
npx create-medusa-app@latest
```

or 

```bash
pnpm dlx create-medusa-app@latest
```

`create-medusa-app` is a command that facilitates creating a Medusa ecosystem. It installs the Medusa backend and admin dashboard, along with the necessary configurations to run the backend.

## Prerequisites

Before you can install and use Medusa, you need the following tools installed on your machine:

- Node.js v16+
- Git
- PostgreSQL. The PostgreSQL server should also be running during your installation process.

## Backend (DB)

### Connect to a Vercel PostgreSQL Database

Use a PostgreSQL database hosted on Vercel, you must use the `--db-url` option and add to the end of your connection URL `?sslmode=require`. For example:

```bash
npx create-medusa-app@latest --db-url "postgres://default:<password>@<host-region>.postgres.vercel-storage.com:5432/verceldb?sslmode=require"
```

