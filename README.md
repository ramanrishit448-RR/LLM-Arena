<div>
    <img src="https://img.shields.io/badge/-Next.js-black?style=for-the-badge&logo=nextdotjs&logoColor=white" />
    <img src="https://img.shields.io/badge/-Prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white" />
    <img src="https://img.shields.io/badge/-PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white" />
    <img src="https://img.shields.io/badge/-Clerk-6C47FF?style=for-the-badge&logo=clerk&logoColor=white" />
    <img src="https://img.shields.io/badge/-Arcjet-000000?style=for-the-badge&logo=arcjet&logoColor=white" />
  <img src="https://img.shields.io/badge/-PostHog-8B4513?style=for-the-badge&logo=posthog&logoColor=white" />
  <img src="https://img.shields.io/badge/-Greptile-22c55e?style=for-the-badge" />
</div>


  <h2 align="center">LLM Arena | Real-Time AI Model Racing</h2>


## 📋 <a name="table">Table of Contents</a>

1. ✨ [Introduction](#introduction)
2. ⚙️ [Tech Stack](#tech-stack)
3. 🔋 [Features](#features)
4. 🤸 [Quick Start](#quick-start)
5. 🔗 [Assets](#links)
6. 🚀 [More](#more)

## <a name="introduction">✨ Introduction</a>

LLM Arena is a unique measuring instrument built to evaluate open-source AI models based on real data, not just vibes. Users submit a single prompt, and the arena races up to three different models side-by-side in real-time, streaming their answers and tracking exact metrics like tokens per second, time to first token, and cost. Users then vote on the winning response, dynamically updating a public leaderboard to reveal which models actually perform best for real-world tasks.

## <a name="tech-stack">⚙️ Tech Stack</a>

- **[Next.js](https://nextjs.org/)** is a production-ready React framework that offers server-side rendering, static site generation, and powerful routing features. It streamlines the development of full-stack web applications by providing a comprehensive ecosystem for performance optimization and API development.

- **[Prisma ORM](https://www.prisma.io/)** is a next-generation ORM for Node.js and TypeScript that simplifies database interactions. It provides a type-safe client generated from your schema, making querying intuitive and highly efficient.

- **[PostgreSQL](https://www.postgresql.org/)** is an advanced, open-source object-relational database system recognized for its reliability and performance. It serves as the persistent storage layer for tracking votes, metrics, and the public leaderboard.

- **[Clerk](https://jsm.dev/arena-clerk)** is a specialized authentication and user management platform for React and Next.js. It offers drop-in pre-built components for secure sign-in and profile management out of the box.

- **[PostHog](https://jsm.dev/arena-posthog)** is an all-in-one product analytics platform. It provides comprehensive observability on every single model call, tracking essential usage data and user interactions across the arena.

- **[Arcjet](https://jsm.dev/arena-arcjet)** is an advanced security layer built for modern applications. It locks down the API endpoints to protect against malicious bots and prompt injection attacks.

- **[Greptile](https://jsm.dev/arena-greptile)** is an AI-powered code review tool. It seamlessly reviews every pull request opened by our agent live during the development workflow to ensure code quality.

## <a name="features">🔋 Features</a>

👉 **Real-Time Model Racing**: Submit a single prompt and watch up to three open-source models stream their answers side-by-side simultaneously.

👉 **Live Performance Metrics**: Accurately track and display exact tokens per second, time to first token, and cost for honest model evaluation.

👉 **Public Voting & Leaderboard**: Vote on the best generated response to feed into a public leaderboard that ranks models based on actual user preference.

👉 **Agentic Development Workflow**: The entire application architecture and codebase were generated agentically using Claude Code based on a plain English specification.

👉 **Full Observability**: Detailed tracking and product analytics on every model call powered by PostHog.

👉 **Endpoint Security**: Intelligent bot protection and prompt injection defense managed by Arcjet.

👉 **Live PR Reviews**: Automated, AI-driven code reviews on every pull request submitted by the agent using Greptile.

And many more, including code architecture and reusability.

## <a name="quick-start">🤸 Quick Start</a>

Follow these steps to set up the project locally on your machine.

**Prerequisites**

Make sure you have the following installed on your machine:

- [Git](https://git-scm.com/)
- [Node.js](https://nodejs.org/en)
- [npm](https://www.npmjs.com/) (Node Package Manager)

**Cloning the Repository**

```bash
git clone https://github.com/adrianhajdin/llm-arena
cd llm-arena
```

**Installation**

Install the project dependencies using npm:

```bash
npm install
```

**Set Up Environment Variables**

Create a new file named `.env` in the root of your project and add the following content:

```env
# https://openrouter.ai/keys
OPENROUTER_API_KEY=

# Postgres connection string
DATABASE_URL=postgresql://user:password@localhost:5432/llm_arena

# https://dashboard.clerk.com -> API keys
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=

# https://app.posthog.com -> Project settings
NEXT_PUBLIC_POSTHOG_KEY=
NEXT_PUBLIC_POSTHOG_HOST=https://us.i.posthog.com

# https://app.arcjet.com -> your site -> SDK key
ARCJET_KEY=ajkey_
```
Replace the placeholder values with your real credentials. You can get these by signing up at: [**Clerk**](https://jsm.dev/arena-clerk), [**PostHog**](https://jsm.dev/arena-posthog), [**Arcjet**](https://jsm.dev/arena-arcjet), [**Greptile**](https://jsm.dev/arena-greptile), [**OpenRouter**](https://openrouter.ai/), and your PostgreSQL provider.

**Running the Project**
```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser to view the project.

