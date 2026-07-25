# 🎯 LangGraph Agent Template

Production-grade **LangGraph agent** template with state machines, tool-calling, human-in-the-loop checkpoints, and persistent memory.

![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?logo=openai&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-6366F1)

## ✨ Features

- 🧠 **State machine** — typed nodes, edges, conditional routing
- 🛠 **Tool calling** — pluggable tools with Zod schemas
- 🙋 **Human-in-the-loop** — interrupt & resume checkpoints
- 💾 **Persistent memory** — Postgres/Redis checkpointer
- 🔁 **Retry + fallback** — automatic error recovery per node
- 📊 **Tracing** — LangSmith integration ready
- 🧪 **Evals** — deterministic test harness for agent runs

## 🏗 Graph

```
        ┌──────────┐
        │  Router  │
        └────┬─────┘
     ┌───────┼────────┐
     ▼       ▼        ▼
  Tools   Reason   HumanReview
     └───────┴────────┘
             ▼
          Finalize
```

## 🚀 Quick Start

```bash
git clone https://github.com/danyorllc-stack/langgraph-agent-template
cd langgraph-agent-template
npm install
cp .env.example .env   # OPENAI_API_KEY, DATABASE_URL, LANGSMITH_API_KEY
npm run dev
```

## 📁 Structure

- `src/graph/` — nodes, edges, state schema
- `src/tools/` — tool definitions (Zod-validated)
- `src/checkpointer/` — Postgres persistence
- `src/evals/` — deterministic agent tests

## 💡 Use Cases

- AI SDR / lead-qualification agents
- Multi-step research assistants
- Customer-support triage bots
- Autonomous workflow orchestrators

## 💼 Built by

[Muhammad Daniyal](https://agenticcore.tech) — AI Solutions Architect.
Powers **LeadCore AI** — production SDR agent at AgenticCore.

**Custom LangGraph agents for your SaaS:** 📩 danyorllc@gmail.com
