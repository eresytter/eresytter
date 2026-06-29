# Eres Ferro Bastian

AI Platform Engineer at AYANA — building and running a production multi-surface LLM platform across four Indonesian resort properties. MA Linguistics (Computational) from Leiden University. Research interest: how LLMs process figurative language, and eventually *why*, from the inside.

---

### What I build at work

**Multi-surface LLM platform** — three distinct production AI surfaces on a shared FastAPI backend: an in-app guest concierge scoped by reservation, an anonymous booking widget embedded on ayana.com, and a Gmail draft assistant for the Reservations team. Sole or primary author across the AI repos.

**Production RAG** — 9-collection Weaviate knowledge base with Cohere + Voyage rerankers, Notion/Drive/Sheets ingestion, and Redis-locked live reloads. Audit-driven k-tuning (200 questions × 4 languages) achieved −28% cost and −8% latency with accuracy flat at 0.96.

**Agentic features** — 5-tool LLM amenity-ordering system (lookup/cart/confirm/cancel). A lookup pre-fire architectural pattern broke a prompt-iteration plateau: eval score lifted from 0.881 to 0.972 across 90+ scenarios × 4 languages × 3 reps. Rolled out under deterministic 50/50 A/B with a kill-switch.

**On-prem inference evaluation** — structured evaluation program on NVIDIA DGX Spark (GB10, 121 GB unified): multi-model chat evals, quantization sweeps (Q8→Q2 imatrix), VLM OCR benchmarks, and a 1000-clip ASR benchmark across 4 languages × 5 noise conditions. A local 1.7B ASR model outperformed the best paid API by 41% WER at $0/req.

**MCP gateway** — Auth0 OIDC → API-key migration with prefix-keyed dispatch, constant-time comparison, role-based routing, and fail-closed handling. Distributed as a signed `.mcpb` bundle.

**Multi-agent fleet** — seven stakeholder LLM agents on Telegram and an ops dashboard, with per-profile systemd unit templates and a 3-layer skill-drift guardrail.

**Eval harness (Langsmith)** — used Langsmith as an evaluation framework; TTFT tracking, multi-provider, warehouse-stored results.

---

### Active research

**[pain_metaphor](https://github.com/eresytter/pain_metaphor)** — Do LLMs know that "stabbing pain" isn't literal? Behavioral evaluation of GPT-4o, Gemini, Llama-2, and BioMistral on pain metaphor comprehension using elenchus and maieutic prompting. MA thesis (Leiden, 2023), now being resurrected with modern models, expanded metaphor coverage, and a Multi-Agent Debate evaluation framework. Targeting ACL Fig-Lang 2027.

**Mechanistic interpretability** *(in progress)* — Learning to reverse-engineer transformer internals with TransformerLens. Goal: trace the internal circuit responsible for the emotional/physical mislabeling error found in the pain_metaphor research.

---

### Stack

**LLM** — Python · FastAPI · tool use / function calling · MCP · structured outputs · reasoning models (gpt-5 / o-series) · prompt engineering with eval discipline

**RAG & vector** — Weaviate · Cohere + Voyage reranking · Notion / Drive / Sheets ingestion

**Evaluation** — AQUA (custom harness) · LangSmith · A/B testing · WER/CER · difference-in-differences

**On-prem inference** — NVIDIA DGX Spark (GB10) · LM Studio · llama.cpp / GGUF · quantization sweeps

**Data / infra** — PostgreSQL · Redis · Airflow · Docker · GitHub Actions · uv

**Web** — Next.js 15 · TypeScript · Rollup

**Direction** — TransformerLens (in progress)

---

**Languages:** English · Indonesian
