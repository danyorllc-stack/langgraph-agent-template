# LangGraph Agent Template

A reference template for experimenting with LangGraph state machines, tool calling, human-in-the-loop checkpoints, persistent memory, and typed TypeScript workflows. This is a standalone template/reference project, not LeadCore source and not a client deployment.

## What it demonstrates

- Typed graph nodes, edges, and conditional routing
- Zod-validated tool definitions
- Interrupt and resume checkpoints
- Postgres persistence patterns
- Retry and fallback handling
- Deterministic evaluation harnesses
- Optional LangSmith tracing integration

## Graph

`Router -> tools / reasoning / human review -> finalize`

## Quick start

```bash
git clone https://github.com/danyorllc-stack/langgraph-agent-template
cd langgraph-agent-template
npm install
cp .env.example .env
# Set provider and database values locally
npm run dev
```

## Structure

- `src/graph/` - nodes, edges, and state schema
- `src/tools/` - Zod-validated tool definitions
- `src/checkpointer/` - persistence integration
- `src/evals/` - deterministic agent tests

## Scope and limitations

Use this repository for learning and architecture experiments. Review authentication, authorization, persistence, provider failure handling, and operational controls before adapting it to another system. LangGraph is used here; LeadCore is a separate custom TypeScript implementation.
