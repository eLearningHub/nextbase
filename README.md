# nextbase

## Getting started

- Define the following variables:

  ```{bash}
  export PROJECT_ID=supabase_project_name
  export PROJECT_REF=supabase_project_reference_key
  ```

- `supabase link --project-ref ${PROJECT_REF}`
- `pnpm prepare:remote`
- `pnpm dev`

## T3 stack + Supabase + App directory

This project is Edge ready (Vercel Edge runtime)

This is a starter project/boilerplate to start out with:

- TRPC
- App directory/router
- Prisma
- Supabase (Auth, Storage, Serverless Queries)
- Tailwind
- Edge Ready
- Umami analytics

It allows us to call database in server components through supabase-js, for client component we are using trpc+prisma due to the superior DX

## Projects using this starter

- PortfolioQuiz [Website](https://www.portfolio-quiz.com/)
- FreeLogo.dev [Website](https://www.freelogo.dev/)
- FeastQR [Repo](https://github.com/jakubczarnowski/FeastQR) [Website](https://www.feastqr.com)
- Instagram Clone [Repo](https://github.com/jakubczarnowski/instagram-clone) [Website](https://instagram-clone-eight-mu.vercel.app/)

## What's next? How do I make an app with this?

- Clone this project
- Run

```
pnpm install
```

- Copy the .env.example into .env and fill out the envs

### Initial Setup

## If you want to develop on local supabase instance, follow the steps below:

Then go to supabase/config.toml file and change your service name.

Start the database:

- supabase start
- pnpm prepare:local

## If you want to develop on remote supabase instance, follow the steps below:

Connect supabase to remote instance:

- supabase link --project-ref <_your_project_id_>
- pnpm prepare:remote

## Common steps

- Fill out environment variables
- Create Secrets on Github

#### If you want to create migrations by hand, go ahead and use this command:

- supabase migration new <_migration_name_>

Then go to supabase/migrations folder and add your SQL there.

#### If you want to make changes with studio, use

- pnpm db:diff <_migration_name_>

## Run these initial commands

Every time you change something on local instance:

```
pnpm prepare:local
```

- If you develop on cloud supabase run:

```
pnpm prepare:remote
```

- Run the project

```
pnpm dev
```

If you are not familiar with the different technologies used in this project, please refer to the respective docs.

- [Next.js app router](https://nextjs.org/docs)
- [Prisma](https://prisma.io)
- [Tailwind CSS](https://tailwindcss.com)
- [tRPC](https://trpc.io)
- [Supabase](https://supabase.com/docs)

## Authors

👤 **Milosz Jankiewicz**

- Twitter: [@twitter.com/jaaneek/](https://twitter.com/jaaneek)
- Github: [@Jaaneek](https://github.com/Jaaneek)
- LinkedIn: [@https://www.linkedin.com/in/jaaneek](https://www.linkedin.com/in/mi%C5%82osz-jankiewicz-554562168/)

👤 **Jakub Czarnowski**

- Twitter: [@twitter.com/charnowsky/](https://twitter.com/charnowsky)
- Github: [@jakubczarnowski](https://github.com/jakubczarnowski)
- LinkedIn: [@https://www.linkedin.com/in/czarnowskijakub/](https://www.linkedin.com/in/czarnowskijakub/)

## Learn More

To learn more about the [T3 Stack](https://create.t3.gg/), take a look at the following resources:

- [Documentation](https://create.t3.gg/)
- [Learn the T3 Stack](https://create.t3.gg/en/faq#what-learning-resources-are-currently-available) — Check out these awesome tutorials

You can check out the [create-t3-app GitHub repository](https://github.com/t3-oss/create-t3-app) — your feedback and contributions are welcome!

## How do I deploy this?

Follow deployment guides for [Vercel](https://create.t3.gg/en/deployment/vercel), [Netlify](https://create.t3.gg/en/deployment/netlify) and [Docker](https://create.t3.gg/en/deployment/docker) for more information.
