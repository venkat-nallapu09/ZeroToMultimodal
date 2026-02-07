# ZeroToMultimodal

> **No APIs. No shortcuts. No magic. Just math, gradients, and systems.**

![ViT](https://img.shields.io/badge/ViT-from--scratch-success?style=flat-square)
![CLIP](https://img.shields.io/badge/CLIP-contrastive--learning-success?style=flat-square)
![QLoRA](https://img.shields.io/badge/QLoRA-4bit--finetuning-success?style=flat-square)
![Agents](https://img.shields.io/badge/Agents-ReAct%20%2B%20Tools-success?style=flat-square)
![Production](https://img.shields.io/badge/Production-Docker%20%7C%20FastAPI%20%7C%20vLLM-success?style=flat-square)


ZeroToMultimodal is a ** from-scratch build log** that goes end-to-end from a raw Vision Transformer to a **production-ready multimodal agent**.

This repo is not a tutorial.
It is a **proof of work**.

What lives here:
- A **vanilla Vision Transformer** implemented from first principles (no Hugging Face crutches)
- A **CLIP-style vision–language model** trained with contrastive learning
- **QLoRA fine-tuning** of a large vision–language model (LLaVA) on custom data
- An **agentic system** that reasons, calls tools, handles failures, and ships results
- A **production deployment** with latency, cost, and reliability constraints

What does *not* live here:
- Copy-pasted notebooks  
- Pretrained model cosplay  
- “Just trust the library” abstractions  

Every branch corresponds to a **hard technical milestone**.  
Every model was trained, debugged, and broken at least once.

If you’re here to learn by osmosis, read the code.  
If you’re here to judge competence, check the branches.  
If you’re here to cargo-cult—leave.

---

**Status:** Actively built, ruthlessly iterated.  
**Standard:** If I can’t explain it on a whiteboard, it doesn’t ship.

---

![No Magic](https://img.shields.io/badge/No%20Magic-Just%20Math-critical?style=flat-square)

---

## Build Log (Non-Negotiable Milestones)

| Phase | Branch | What Was Built |
|------|-------|----------------|
| Days 1–3 | `day3-vit-basics` | Vanilla ViT from scratch, CIFAR-10 >85% |
| Days 4–7 | `week1-clip-lite` | CLIP-style contrastive V+L model |
| Days 8–12 | `llava-fails` | QLoRA fine-tuned LLaVA on custom video data |
| Days 13–17 | `meme-agent` | ReAct agent with tools + error handling |
| Days 18–21 | `main` | Dockerized, deployed, stress-tested system |
