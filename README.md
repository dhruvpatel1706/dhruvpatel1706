# Hi, I'm Dhruv 👋

Building at the intersection of ML systems and quant finance. I like shipping things that are honest about their failure modes, not allergic to benchmarks, and actually usable by other developers.

## 🚀 Currently shipping

- **[algo-trader](https://github.com/dhruvpatel1706/algo-trader)** — Paper-first algorithmic trading system. Wheel + mean-reversion strategies on ETFs, walk-forward backtests with realistic costs, risk + compliance gates on every order, FastAPI + Next.js 15 dashboard. Python · Polars · Alpaca · PostgreSQL.
- **[mlops-customer-support](https://github.com/dhruvpatel1706/mlops-customer-support)** — End-to-end MLOps pipeline for support ticket analytics. Multi-store architecture (Postgres, MongoDB, Qdrant, Redis), HuggingFace sentiment + topic + NER models, Prometheus + Grafana + Evidently for drift detection.
- **[personal-rag](https://github.com/dhruvpatel1706/personal-rag)** `v0.2` — Local RAG over your PDFs/notes. Embeddings on-device via fastembed; LanceDB vector store; FastAPI + CLI. **v0.2 ships [Contextual Retrieval](https://www.anthropic.com/news/contextual-retrieval)** — prefix every chunk with a Haiku-generated situating context (with the full doc prompt-cached) for ~35-50% better recall.
- **[paper-digest](https://github.com/dhruvpatel1706/paper-digest)** `v0.2` — arXiv URL/ID or PDF → structured summary (problem / method / results / limitations) via Claude with adaptive thinking and schema-constrained output. **v0.2 adds interactive follow-up Q&A** grounded in the paper (full paper prompt-cached for cheap multi-turn).
- **[agent-interviewer](https://github.com/dhruvpatel1706/agent-interviewer)** — Mock interview CLI with 4 specialized Claude personas (behavioral, system design, coding, case). Post-session feedback agent returns per-dimension 1-5 scores with observations grounded in the transcript.
- **[mcp-zettel](https://github.com/dhruvpatel1706/mcp-zettel)** — MCP server exposing a Zettelkasten knowledge base to any MCP client (Claude Desktop, Claude Code, Cursor). Atomic markdown notes, bidirectional `[[wiki-links]]`, title/tag-weighted search. Built on the official [MCP Python SDK](https://github.com/modelcontextprotocol/python-sdk).
- **[claude-pr-reviewer](https://github.com/dhruvpatel1706/claude-pr-reviewer)** `v0.2` — Open-source Claude-powered PR reviewer. CLI + drop-in GitHub Action. **v0.2 posts proper inline GitHub reviews** (one atomic review, per-finding line-specific comments) via `gh api` — parity with what Greptile / CodeRabbit / Codium sell as SaaS.

## 🌱 Up next

- `personal-rag v0.3` — hybrid BM25 + dense retrieval for better recall on rare terms
- `claude-pr-reviewer v0.3` — per-file chunking for very large PRs
- A small evals framework for comparing prompts/models on custom benchmarks
- `mcp-zettel v0.2` — semantic search as a second MCP tool (keyword + dense, fused)

## 🛠️ Tech I reach for

**Languages** — Python 3.12 · TypeScript 5 · SQL
**Backend** — FastAPI · Next.js · Docker · PostgreSQL · Redis · MongoDB · Qdrant · LanceDB
**LLM / ML** — Claude API (Messages, structured outputs, prompt caching, adaptive thinking) · MCP (Model Context Protocol) · HuggingFace Transformers · PyTorch · Polars · fastembed · LangChain
**Observability** — Prometheus · Grafana · Evidently · structlog
**Tooling** — uv · ruff · black · pytest · GitHub Actions · Typer · Rich · unidiff

## 📫 Reach me

[dhruv17062000@gmail.com](mailto:dhruv17062000@gmail.com)
