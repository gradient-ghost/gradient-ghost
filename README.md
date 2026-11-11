# Hey, I'm Saksham.

I build **End-to-end AI systems and tools**, with a focus on ML engineering, LLM engineering, AI agents, and retrieval-augmented generation (RAG).

I'm interested in the engineering behind these systems: designing architectures, evaluating outputs, improving reliability, and making practical tradeoffs.

My recent work includes a credit-risk decision system and a Pydantic v1 → v2 migration CLI. I'm also building out projects around LLM applications, RAG, and agentic systems.

## Technical Stack

**Languages:** Python

**ML & Data:** PyTorch · scikit-learn · Keras · NumPy · pandas

**LLM & Retrieval:** Hugging Face Transformers · FAISS · Qdrant · RAGAS 

**Backend & Development:** FastAPI · Pydantic · Docker · Streamlit · Git · Linux


## Areas of Focus

Machine Learning Engineering · LLM Engineering · RAG · AI Agents · Model & LLM Evaluation

## Featured Projects

### [Credit Risk Decision System](https://github.com/gradient-ghost/credit-risk-decision)

An end-to-end credit-risk system that turns default probabilities into a three-band lending policy: approve, manual review, or reject.

Built a temporal ML pipeline with leakage controls, probability calibration, and out-of-time evaluation.

Designed an expected-loss policy engine with explicit approval and review constraints.

Served predictions through FastAPI, with a Streamlit dashboard, Docker Compose deployment, and automated tests.

Evaluation: 47.51% lower estimated expected loss than the approve-all baseline in a historical out-of-time backtest, at a 61.47% auto-approval rate. This is a counterfactual simulation, not realised financial savings.

[Architecture decisions](https://github.com/gradient-ghost/credit-risk-decision/blob/main/docs/ADR_log.md)

### [Pydantic v2 Migration Copilot](https://github.com/gradient-ghost/pydantic-v2-copilot)

A CLI developer tool for modernising legacy Pydantic v1 code towards Pydantic v2.

Combines deterministic Python AST transformations with scoped RAG and multi-provider LLMs.

Uses a four-gate verification pipeline to check generated changes before writing them to disk.

Includes SHA-256 caching so reviewed diffs can be applied without repeating LLM calls.

Validation: 114 offline automated tests and evaluation against a 72-file FastAPI application.

[Architecture decisions](https://github.com/gradient-ghost/pydantic-v2-copilot/blob/main/DECISIONS.md)
