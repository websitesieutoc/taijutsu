# Taijutsu Stack

The stack that use Tailwind

## Features

This template includes the following:

- Next.js 14
- TypeScript
- ESLint
- Prettier
- Tailwind CSS
- Prisma
- Next-Auth
- Docker Compose with:
    - PostgresQL
    - Redis
    - Mailpit

## Demo

https://taijutsu.sieutoc.website

## Getting Started

#### For Development

- We use `pnpm` package manager. Get it [here](https://pnpm.io/installation).
- Make sure Docker up and running.
- If your Docker account has 2FA enabled, you have to create a Personal Access Token and login before:
    - Follow [this guide](https://docs.docker.com/docker-hub/access-tokens/).
    - Login with `docker login --username <your-username>`

#### Clone the project

You can either use this template by:

- Click the **"Use this template"** button and follow the instruction
- Or using the script below:

```bash
npx tiged websitesieutoc/taijutsu your-project
```

Then, search and replace `taijutsu` with your project slug.

#### Install dependencies

```bash
cd your-project
pnpm install
```

#### Setup environment variables

For the first time, you need some default environment variables:

```bash

cp .env.example .env
```

Then, run the development server:

```bash
pnpm dev
```

Then, run the development server:

```bash
pnpm dev
```

#### Setup Prisma

NOTE: The dev server need to be running, because we need Postgres instance.

Sometimes, for example in fresh database situation when you have just started:

```bash
pnpm prisma migrate dev
```

#### Create New Component

We use [ shadcn-ui ](https://ui.shadcn.com/) in this stack, and create 2 helper scripts for you:

```bash
# for adding new component
pnpm ui:add <compnent-name>

# for checking diffs
pnpm ui:diff
```

#### Start developing!

Open [http://localhost:3000](http://localhost:3000) with your browser and start developing.

## Good to know

- This project uses `App Router` feature.
- We try to take adventage of Next.js's ecosystem, thus most of the features here are built on top of Next.js best practices.
- We use Chakra UI as our primary library. For ready-made themes, please find it at our [themes](https://github.com/websitesieutoc/themes) repo.
- In the future we will launch a tool for customising your own themes soon!

## Deployment

#### EasyPanel Schema

```json
{

}
```
