# AI Copilot Instructions for AIEngineering

## Project Overview

**AIEngineering** is a structured 12-week learning roadmap for mastering AI engineering end-to-end. This is a **learning-by-doing** repository where each week builds a specific capability: from Python fundamentals → Transformers → RAG → AI Agents → MCP systems → a shipped product AI agent.

Each week has 7 days (or more), with specific assignments. The philosophy is **no passive learning**—every day requires code commits, working implementations, and breaking things intentionally.

## Critical Developer Workflows

### When assisting learners:
- **Daily cadence**: Help implement one assignment per day, not multiple days at once
- **Break things intentionally**: Encourage deliberate exploration of edge cases and failure modes
- **Always commit**: Each assignment should result in a git commit with clear messages
- **Document learning**: Require learners write READMEs explaining *why* components work, not just *how*
- **Evaluation first**: Before coding, discuss what success looks like (precision@k, loss curves, etc.)

### Typical workflow for an assignment:
1. **Understand the goal**: What specific skill/concept is being taught?
2. **No frameworks initially**: Weeks 1-7 heavily emphasize building "from scratch" (NumPy, not PyTorch; implement attention, not use transformers)
3. **Add tests immediately**: Each assignment should have unit tests for edge cases
4. **Measure & compare**: Later weeks emphasize benchmarking (latency/quality tradeoffs, tokenization comparisons)
5. **Refactor before moving on**: Week 7 is explicitly a "Review + Refactor" checkpoint

## Repository Structure & Patterns

### Week-based organization:
- **Week 1-7**: Foundational skills (Python, math, models, prompt engineering, RAG, agents)
- **Week 8-9**: Advanced patterns (multi-agent systems, MCP-style orchestration)
- **Week 10-12**: Integration & delivery (training, capstone, hardening)

### Assignment patterns:
- **"from scratch"** assignments: NumPy, pure Python—no high-level frameworks initially
- **Comparative assignments**: Compare 2-3 approaches side-by-side (tokenizers, embedding models, chunking strategies)
- **Evaluation-heavy**: Later weeks require metrics, benchmarks, and measured results
- **Documentation-first**: Each checkpoint requires a README explaining internals

## Key Architectural Concepts to Reference

### Progression flow:
- **Chunking** (Week 1) → **Embeddings** (Week 1) → **RAG pipeline** (Week 5) → **Multi-agent RAG** (Week 8-9)
- **Attention math** (Week 2) → **Transformer blocks** (Week 2) → **Model loading** (Week 3) → **LoRA fine-tuning** (Week 3)
- **Simple tools agents** (Week 7) → **Multi-agent systems** (Week 8) → **MCP orchestration** (Week 9)

### Critical boundaries:
- **From scratch** (Weeks 1-2, 5): Use foundational libraries only (NumPy, FAISS)
- **Framework introduction** (Week 3+): HuggingFace, PyTorch become primary, but build understanding of *how* models work first
- **Production concerns** (Weeks 8-10): Cost control, caching, logging, permission systems, guardrails

## Project-Specific Conventions

### Naming & structure:
- Use `argparse` for CLI apps (Day 1 assignment blueprint)
- Dataclasses + typing for structured data (Day 2 teaches this)
- Separate `test_*.py` files with edge case coverage
- Each checkpoint day (7, 14, 21, etc.) has a standalone README explaining deliverables

### Evaluation metrics to enforce:
- **RAG**: precision@k, recall, F1 on retrieval
- **Embedding models**: NDCG, cosine similarity comparisons
- **Agents**: success rate, step count, fallback frequency
- **Inference**: latency vs quality tradeoffs (BLEU, perplexity, custom metrics)

### Guardrails to instill:
- **No magic**: Explain matrix math, attention weights, loss curve trends
- **Intentional failures**: Create test cases that *should* fail, then fix them
- **Version everything**: Commit frequently, document why changes happened
- **Measure before optimizing**: Always baseline first (Week 8 cost control)

## Integration Points & External Dependency Patterns

### Primary external libraries:
- **PyTorch**: Model training and inference (Weeks 2-3, 10)
- **Hugging Face**: Pre-trained models, embedding models, PEFT/LoRA (Week 3)
- **FAISS**: Vector store for RAG (Week 5)
- **LangChain paradigms**: Agent architecture, tool definitions (Week 7-9)

### When to use each:
- **NumPy**: Math fundamentals, tokenization, attention (Weeks 1-2)
- **PyTorch**: Transformer blocks, custom layers, training loops (Weeks 2-3, 10)
- **HuggingFace**: Pre-built models, inference, LoRA adaptation (Week 3+)
- **FAISS**: Semantic search, large-scale retrieval (Week 5+)

## Guidance for AI Agents

### During implementation:
1. **Ask about week/day**: Context matters—Day 8 (tokenization) has different "from scratch" requirements than Day 18 (LoRA)
2. **Enforce testing**: Every assignment needs `test_*.py` with 3+ edge cases
3. **Require documentation**: If a learner skips README updates, redirect them
4. **Guide toward patterns, not solutions**: If stuck, point to similar assignments in earlier weeks
5. **Emphasize reproducibility**: All results should be repeatable (seed randomness, version models)

### Common pitfalls to avoid:
- **Framework too early**: Don't use `transformers.pipeline()` for Week 2's attention implementation
- **Skipping math**: Ensure learner understands *why* scaled dot product attention works before implementing multi-head
- **No evaluation**: Don't accept "this looks good" without metrics
- **Isolated checkpoints**: Cross-reference previous weeks (Week 5 RAG uses Week 1 chunking, Week 2 embeddings)

## Success Indicators

A learner is on track when:
- ✅ Daily commits with descriptive messages (implementation + docs)
- ✅ Unit tests for all assignments (edge cases included)
- ✅ Measured results (benchmarks, comparisons, metrics)
- ✅ Week checkpoints have standalone READMEs explaining internals
- ✅ Code progresses from "from scratch" → "framework-based" intentionally
- ✅ Multi-agent systems (Week 8+) inherit tools/memory/policies from earlier weeks

---

**Final note**: By Week 11, the capstone should integrate everything: open-source model + RAG + tools + policies + memory + evaluation. This is not a hypothetical project—it should be deployable.
