# AIEngineering


# 🔥 12-WEEK HARD-MODE AI ENGINEERING ROADMAP (LEARN BY DOING)

> Goal: Master AI Engineering end-to-end — Transformers, Training, RAG, AI Agents, MCP-style systems, and shipping a product-grade AI agent using open-source models.

Rules:
- ❌ No passive learning
- ❌ No skipping exercises
- ❌ No “I understand” without building
- ✅ Write code + docs every day
- ✅ Commit daily
- ✅ Break things intentionally

---

## WEEK 1 — PYTHON + AI ENGINEERING FOUNDATIONS

### Day 1
- Setup environment (Python, venv, PyTorch, HF, FAISS)
- Repo structure
- README with goals

**Assignment**
- Create a CLI app skeleton (`argparse`)
- Commit

---

### Day 2
- Python: async, typing, dataclasses
- JSON/YAML handling

**Assignment**
- Write async file loader + parser
- Unit tests

---

### Day 3
- Linear algebra refresh (vectors, dot product)
- Cosine similarity

**Assignment**
- Implement cosine similarity from scratch
- Compare with NumPy

---

### Day 4
- Text preprocessing
- Chunking strategies

**Assignment**
- Write chunker with overlap
- Add tests for edge cases

---

### Day 5
- Embeddings concept
- Semantic search basics

**Assignment**
- Build local embedding store (no frameworks)
- Query top-k chunks

---

### Day 6
- Evaluation basics

**Assignment**
- Write evaluation script (precision@k)
- Document results

---

### Day 7
- Review + refactor

**Checkpoint**
- CLI tool: file → chunks → embeddings → search

---

## WEEK 2 — TOKENIZATION & ATTENTION (FROM SCRATCH)

### Day 8
- Tokenization (BPE, WordPiece)

**Assignment**
- Compare tokenization of code vs English vs Hinglish
- Write analysis

---

### Day 9
- Attention math

**Assignment**
- Implement scaled dot-product attention (NumPy)

---

### Day 10
- Multi-head attention

**Assignment**
- Extend attention to multi-head
- Visualize weights

---

### Day 11
- Positional encoding

**Assignment**
- Implement sinusoidal encodings
- Explain why order matters

---

### Day 12
- Transformer blocks

**Assignment**
- Build single transformer block in PyTorch

---

### Day 13
- Decoder-only models

**Assignment**
- Implement next-token prediction loop

---

### Day 14
**Checkpoint**
- Mini transformer trained on toy dataset
- README explaining internals

---

## WEEK 3 — OPEN-SOURCE MODELS (HUGGING FACE CORE)

### Day 15
- HF model loading
- Inference pipelines

**Assignment**
- Load 2 LLMs
- Same prompt, compare outputs

---

### Day 16
- Quantization (4-bit, 8-bit)

**Assignment**
- Measure latency vs quality tradeoffs

---

### Day 17
- Embedding models

**Assignment**
- Compare 3 embedding models
- Create benchmark table

---

### Day 18
- PEFT / LoRA theory

**Assignment**
- Prepare dataset for fine-tuning

---

### Day 19
- LoRA fine-tuning

**Assignment**
- Fine-tune on domain data
- Evaluate before vs after

---

### Day 20
- Model evaluation

**Assignment**
- Write automated eval script

---

### Day 21
**Checkpoint**
- Tuned model + evaluation report

---

## WEEK 4 — PROMPT ENGINEERING (ENGINEERING DISCIPLINE)

### Day 22
- Prompt anatomy

**Assignment**
- Write 5 prompt variants
- Compare determinism

---

### Day 23
- Few-shot & instruction hierarchy

**Assignment**
- Build instruction templates

---

### Day 24
- Output schemas

**Assignment**
- Enforce JSON schema outputs

---

### Day 25
- Prompt testing

**Assignment**
- Build prompt test harness

---

### Day 26
- Prompt attacks

**Assignment**
- Jailbreak your own prompts
- Patch failures

---

### Day 27
- Prompt versioning

**Assignment**
- Version prompts + changelog

---

### Day 28
**Checkpoint**
- Production-ready prompt library

---

## WEEK 5 — RAG (FROM SCRATCH)

### Day 29
- Chunking deep dive

**Assignment**
- Compare 3 chunking strategies

---

### Day 30
- Vector stores

**Assignment**
- Implement FAISS-based retriever

---

### Day 31
- Query rewriting

**Assignment**
- Build query rewriter module

---

### Day 32
- Context construction

**Assignment**
- Dynamic context assembly

---

### Day 33
- RAG failure modes

**Assignment**
- Create hallucination cases
- Fix them

---

### Day 34
- RAG evaluation

**Assignment**
- Precision / Recall measurement

---

### Day 35
**Checkpoint**
- Product-grade RAG system

---

## WEEK 6 — ADVANCED RAG

### Day 36
- Hybrid search

**Assignment**
- Keyword + vector hybrid retriever

---

### Day 37
- Metadata filtering

**Assignment**
- Add metadata constraints

---

### Day 38
- Context compression

**Assignment**
- Summarize before retrieval

---

### Day 39
- RAG caching

**Assignment**
- Implement query cache

---

### Day 40
- Source attribution

**Assignment**
- Enforce citations in output

---

### Day 41
- Stress testing

**Assignment**
- Large dataset tests

---

### Day 42
**Checkpoint**
- Scalable RAG pipeline

---

## WEEK 7 — AI AGENTS (LANGCHAIN-STYLE, REAL)

### Day 43
- Agent architecture

**Assignment**
- Build simple tool-using agent

---

### Day 44
- Tool calling

**Assignment**
- Agent with search + code tools

---

### Day 45
- Memory types

**Assignment**
- Short-term + long-term memory

---

### Day 46
- Planning vs execution

**Assignment**
- Planner → Executor agent split

---

### Day 47
- Reflection loops

**Assignment**
- Self-correcting agent

---

### Day 48
- Failure handling

**Assignment**
- Retry + fallback logic

---

### Day 49
**Checkpoint**
- Robust single-agent system

---

## WEEK 8 — MULTI-AGENT SYSTEMS

### Day 50
- Multi-agent design

**Assignment**
- Planner / Executor / Critic agents

---

### Day 51
- Communication protocols

**Assignment**
- Structured agent messages

---

### Day 52
- Cost control

**Assignment**
- Token & step limits

---

### Day 53
- Evaluation

**Assignment**
- Agent success metrics

---

### Day 54
- Debugging agents

**Assignment**
- Trace agent failures

---

### Day 55
- Optimization

**Assignment**
- Reduce loops & latency

---

### Day 56
**Checkpoint**
- Multi-agent AI system

---

## WEEK 9 — MCP-STYLE SYSTEMS (MODEL + CONTEXT + POLICY)

### Day 57
- Context orchestration

**Assignment**
- Dynamic context router

---

### Day 58
- Policy enforcement

**Assignment**
- Allowed tools & actions

---

### Day 59
- Authorization layers

**Assignment**
- Tool permission system

---

### Day 60
- Memory boundaries

**Assignment**
- Scoped memory rules

---

### Day 61
- Observability

**Assignment**
- Logging + traces

---

### Day 62
- Guardrails

**Assignment**
- Output filtering

---

### Day 63
**Checkpoint**
- MCP-style orchestration engine

---

## WEEK 10 — TRAINING & DATA

### Day 64
- Dataset creation

**Assignment**
- Build dataset pipeline

---

### Day 65
- Data cleaning

**Assignment**
- Deduplication & normalization

---

### Day 66
- Instruction tuning

**Assignment**
- Train instruction-following model

---

### Day 67
- Overfitting analysis

**Assignment**
- Loss curve analysis

---

### Day 68
- Evaluation

**Assignment**
- Regression tests

---

### Day 69
- Deployment strategy

**Assignment**
- Inference optimization plan

---

### Day 70
**Checkpoint**
- Trained & evaluated model

---

## WEEK 11 — CAPSTONE BUILD

### Day 71–76
- Build **Product AI Agent**
  - Open-source model
  - RAG
  - Tools
  - Policies
  - Memory
  - Evaluation

**Daily Requirement**
- Commit + docs

---

## WEEK 12 — HARDENING & DELIVERY

### Day 77
- Architecture diagram

### Day 78
- Cost analysis

### Day 79
- Failure case report

### Day 80
- Load & stress testing

### Day 81
- Refactor & cleanup

### Day 82
- README (product-grade)

### Day 83–84
**FINAL CHECKPOINT**
- Deployable AI agent
- Interview-ready explanation

---

## 🏁 FINAL OUTCOME
You can now:
- Train and adapt models
- Build RAG systems
- Engineer AI agents
- Enforce policies
- Ship AI products

You are no longer “learning AI”.
You are **doing AI engineering**.
