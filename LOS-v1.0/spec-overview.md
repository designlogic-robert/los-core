# LOS v1.0 — Specification Overview (High-Level)

## 1. Purpose

LOS provides a governed execution layer for AI instructions.

Instead of sending raw prompts directly to a model, LOS:

1. Interprets the instruction
2. Validates it against Binder rules and constraints
3. Routes it through the appropriate mode/agent (via AMC)
4. Tracks context in ARC
5. Persists important semantic state via LLpL

---

## 2. Core Components

### 2.1 Binder v2.0

- Validates inputs and candidate outputs
- Enforces ethics, constraints, and safety rules
- Integrates alignment and autonomy protection logic
- Emits validation decisions and fix-hints

### 2.2 ARC (Adaptive Runtime Context)

- Holds session-level context: goals, constraints, state
- Tracks which agents/modes are active
- Provides a stable “runtime picture” for multi-step reasoning

### 2.3 AMC (Adaptive Mode Controller)

- Selects which mode/agent should handle a given instruction
- Supports posture overlays and behavior routing
- Coordinates between tools, evaluators, and generators

### 2.4 LLpL (Language-Level Persistence Layer)

- Stores semantic snapshots, hashes, and references
- Enables replay, auditing, and cross-session continuity
- Keeps language-level state portable between environments

---

## 3. Stack Relationship

- **Engine (L0):** base compute / model
- **LOS (L1):** this spec — OS for language
- **AdaptE (L2):** framework for agents, workflows, and products
- **DLStudio (L3):** application suite and product layer

LOS does not dictate application UX.  
It defines the **contracts and behaviors** the rest of the system can rely on.

---

## 4. Notes

This document is deliberately high-level and public-safe.  
Deeper implementation details (SCP, WaN, internal governance extensions) are tracked in private design docs.
