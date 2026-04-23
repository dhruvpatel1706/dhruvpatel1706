<p align="center">
  <samp>
    <a href="#selected-work">work</a> &nbsp;·&nbsp;
    <a href="#stack">stack</a> &nbsp;·&nbsp;
    <a href="mailto:dhruv17062000@gmail.com">email</a>
  </samp>
</p>

<br>

### Dhruv Patel

I build small, useful developer tools around the Claude API — retrieval
systems, agent workflows, and safety evals — plus a little mechanistic
interpretability and algorithmic trading on the side. Everything below
is something I actually use.

Repos here are active — the commit graphs show the current cadence.

<br>

<h4 id="selected-work">Selected work</h4>

**Safety, evals, and interpretability**

- [**mech-interp-starter**](https://github.com/dhruvpatel1706/mech-interp-starter) — reproduces the induction-head result from Olsson et al. (Anthropic, 2022) on GPT-2 small. **v0.2**: prefix-matching score (recovers 5/5 published heads), copying score via OV-circuit introspection, and a head-ablation experiment — zeroing the top 5 induction heads increases ICL loss by +642.7% vs +27.7% for matched non-induction heads (23× specificity). Real run artifacts committed.
- [**claude-evals**](https://github.com/dhruvpatel1706/claude-evals) — open-source safety eval suite for Claude. Three evals: sycophancy, refusal calibration (XSTest-style), jailbreak robustness. **v0.2**: hand-labeled *gold set* per eval so you can measure the *judge's* accuracy before trusting any subject pass rate — `calibrate` subcommand reports judge precision / recall / confusion matrix.
- [**swe-agent-lite**](https://github.com/dhruvpatel1706/swe-agent-lite) — SWE-bench-style agent benchmark for Claude. **v0.2**: 13 curated bug-fix tasks including 3 multi-file ones, 5-tool agent surface, sandboxed workspace, failure-mode tags (`hit_iteration_limit`, `edit_but_no_retest`, `exit_early`, …) so you know *why* a task failed, not just that it did.
- [**prompt-gym**](https://github.com/dhruvpatel1706/prompt-gym) — regression tests for LLM prompts. YAML specs, four matchers (`exact` / `contains` / `regex` / `llm_judge`), `run` / `diff` subcommands. Non-zero exit codes so it drops into CI as a gate.

**Retrieval, agents, and LLM tooling**

- [**personal-rag**](https://github.com/dhruvpatel1706/personal-rag) — local RAG over your own notes and PDFs. LanceDB + fastembed, hybrid BM25 / dense retrieval, [Anthropic Contextual Retrieval](https://www.anthropic.com/news/contextual-retrieval), inline citations, watch-mode reindex, a server-rendered web UI, and `similar` for finding related chunks.
- [**mcp-zettel**](https://github.com/dhruvpatel1706/mcp-zettel) — MCP server for a personal Zettelkasten. `[[wiki-link]]` graph, keyword + semantic search, prompt templates, Mermaid diagrams, and hybrid link suggestions on note create.
- [**claude-pr-reviewer**](https://github.com/dhruvpatel1706/claude-pr-reviewer) — CLI + GitHub Action that posts real inline PR review comments via `gh api`. Per-file chunking for big diffs, `.claude-review.yml` repo config, diff-hash review cache, and a calibration harness that actually measures precision / recall.
- [**agent-interviewer**](https://github.com/dhruvpatel1706/agent-interviewer) — mock interview CLI with four Claude personas (behavioral, system design, coding, case). Per-dimension scoring grounded in the transcript, YAML persona packs, replay through a different model, side-by-side diff between feedback variants in a small web viewer.
- [**paper-digest**](https://github.com/dhruvpatel1706/paper-digest) — arXiv / OpenReview / ACL PDF → structured summary (problem · method · results · limitations). Interactive follow-up Q&A grounded in the paper, reading-list batch mode, watch-a-folder auto-digest, searchable history.

**Trading & MLOps**

- [**algo-trader**](https://github.com/dhruvpatel1706/algo-trader) — options wheel + mean-reversion paper-trading system. Walk-forward backtests with realistic slippage and costs, risk and compliance gates on every order, FastAPI + Next.js 15 control plane.
- [**mlops-customer-support**](https://github.com/dhruvpatel1706/mlops-customer-support) — end-to-end support-ticket analytics pipeline. PostgreSQL / MongoDB / Qdrant / Redis, HuggingFace sentiment / topic / NER, Prometheus + Grafana + Evidently for drift detection.

<br>

<h4 id="stack">Stack</h4>

- **Languages** — Python 3.12 · TypeScript · SQL
- **Backend** — FastAPI · Next.js · Docker · PostgreSQL · Redis · MongoDB · LanceDB · Qdrant
- **LLM / ML** — Claude API (structured output, prompt caching, adaptive thinking) · MCP · fastembed · HuggingFace · Polars
- **Ops** — Prometheus · Grafana · Evidently · GitHub Actions · uv · pytest

<br>

<p align="center">
  <samp><a href="mailto:dhruv17062000@gmail.com">dhruv17062000@gmail.com</a></samp>
</p>
