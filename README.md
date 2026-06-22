<div align="center">

<h1>DevRadar</h1>

### See the developer job market before you apply.

Indexes 50,000+ job postings to track skill trends, surface your resume gaps, and prep you for the interview — powered by a multi-provider LLM router, pgvector RAG, and its own **MCP server**.

<br/>

[![Live](https://img.shields.io/badge/▶_Live_App-dev--radar--web.vercel.app-6366f1?style=for-the-badge&labelColor=1e1b4b)](https://dev-radar-web.vercel.app)
[![Demo](https://img.shields.io/badge/Watch_the_demo-▶-6366f1?style=for-the-badge&labelColor=1e1b4b)](#-demo)

![Turborepo](https://img.shields.io/badge/Turborepo-EF4444?style=flat-square&logo=turborepo&logoColor=fff)
![Next.js](https://img.shields.io/badge/Next.js-000?style=flat-square&logo=next.js)
![tRPC](https://img.shields.io/badge/tRPC-2596BE?style=flat-square&logo=trpc&logoColor=fff)
![Prisma](https://img.shields.io/badge/Prisma_+_pgvector-2D3748?style=flat-square&logo=prisma)
![MCP](https://img.shields.io/badge/MCP_Server-6366f1?style=flat-square)

</div>

---

## 🎬 Demo

> Open [`index.html`](./index.html) for the animated product reel, or explore the live app.

**▶ Live:** **https://dev-radar-web.vercel.app**

<!-- ![DevRadar demo](./assets/demo.gif) -->

---

## The problem

The job market moves faster than any developer can track. Which skills are actually rising? What do they pay? Are you ready for the interview? Most devs find out *after* they apply — and get filtered out.

## The solution

DevRadar turns 50K+ live job postings into a personal radar: real demand signals, an honest read on your gaps, and AI interview prep grounded in real market data.

---

## ✨ What makes it different

| | |
|---|---|
| 📡 **Skill-trend radar** | Tracks demand, growth rate and salary bands across 50K+ postings — see what's rising before it's obvious. |
| 🎯 **Resume gap analysis** | Drop your resume; pgvector embeddings map your skills against the live market and surface the real gaps. |
| 🧠 **AI interview prep** | Generates role-specific question sets and a career-chat agent that answers from live data, not generic advice. |
| 🔌 **An MCP server** | Exposes the market data as a **Model Context Protocol server** — query it from Claude Desktop or Cursor. (Most engineers *use* MCP; this *is* a server.) |
| 🔀 **Multi-provider router** | Groq / Gemini / OpenAI / Ollama with three strategies (cheapest, free-only, fallback) + per-call cost tracing via Langfuse. |
| 🔎 **Hybrid retrieval** | Dense pgvector + Postgres full-text, fused with Reciprocal Rank Fusion — catches exact terms pure vectors miss. |

---

## 🏗️ Tech

- **Monorepo:** Turborepo + pnpm
- **App:** Next.js 14 (App Router), tRPC v11, Prisma 6 + Neon Postgres + **pgvector(768)**
- **AI:** multi-provider router (Groq/Gemini/OpenAI/Ollama), RAG + hybrid search, ReAct tool-calling chat agent, Langfuse tracing
- **MCP:** standalone `@modelcontextprotocol/sdk` server exposing 5 market-data tools over stdio
- **Infra:** Vercel, Upstash Redis + QStash, Sentry

---

## 📊 By the numbers

- **50K+** job postings indexed
- **5** MCP tools exposed to any AI client
- **3** LLM routing strategies (cheapest / free / fallback)
- **768-dim** pgvector embeddings for semantic match

---

<div align="center">

**Built by Ali Shahid** · [Portfolio](https://alishahid-dev.vercel.app) · [LinkedIn](https://linkedin.com/in/alishahid-fswebdev)

</div>
