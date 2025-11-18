# Modes & Postures — Semantic Core Specification  
_Public-Stable Specification (v1.0)_

Modes and Postures define the **operational stance** of the Semantic Core.  
They determine how SynCE interprets intent, routes cognition, shapes execution, and maintains alignment.

Modes = functional focus.  
Postures = behavioral stance.

Together, they create a deterministic cognitive profile for each operation.

---

# 1. Purpose

Modes and Postures provide:

- predictable behavior  
- context-aware reasoning  
- selectable cognitive strategies  
- alignment with operator intent  
- safety and coherence  
- affect-aware execution  

They ensure SynCE remains *explicit*, *inspectable*, and *deterministic* in how it acts.

---

# 2. Definitions

## 2.1 Modes
Modes configure **what the system is doing**.

A Mode defines:

- cognitive tempo  
- reasoning depth  
- analytical vs creative emphasis  
- risk posture  
- verbosity  
- planning behavior  
- tool usage preferences  

Modes are functional roles.

Examples (public):

- Analytical.Mode  
- Creative.Mode  
- Teaching.Mode  
- SeniorDev.Mode  
- Research.Mode  
- FastHelp.Mode  

Modes modify ARC behavior and ORCH-C planning.

---

## 2.2 Postures
Postures configure **how the system is behaving**.

A Posture defines:

- affective tone  
- relationship stance  
- motivational safety  
- interpretive boundaries  
- alignment orientation  
- cognitive stance (precision-first, empathy-first, structure-first, etc.)  

Postures are behavioral orientations.

Primary Posture Groups:

- Cognitive  
- Affective  
- Ethical  
- Pragmatic  

Postures shape Binder, CAP, and ATC/CRI behavior.

---

# 3. Architecture (GitHub-Safe Diagram)

```
Modes & Postures — Cognitive Architecture

+---------------------------------------------------------------+
| Modes (Functional Control)                                    |
|   - reasoning depth                                           |
|   - tempo / planning                                          |
|   - analytical/creative weight                                |
|   - verbosity + precision                                     |
+---------------------------------------------------------------+
| Postures (Behavioral Control)                                 |
|   - affective tone                                            |
|   - ethical alignment                                          |
|   - autonomy safeguards (CAP)                                 |
|   - relational stance                                         |
+---------------------------------------------------------------+
| ARC — Adaptive Runtime Context                                |
|   - applies mode/posture params                               |
|   - maintains cognitive state                                 |
+---------------------------------------------------------------+
| Binder v2.0 + CAP v1.0                                        |
|   - affective/ethical validation                              |
|   - autonomy + integrity checks                               |
+---------------------------------------------------------------+
| ORCH-C (Planner)                                              |
|   - uses derived stance/tempo                                 |
|   - generates aligned plans                                   |
+---------------------------------------------------------------+
```

---

# 4. How Modes Work

## 4.1 Mode Parameters
Each Mode includes:

- target tempo (slow / medium / fast)  
- reasoning depth (shallow / structured / deep)  
- creativity vs precision ratio  
- structural weight (outline, chain-of-thought, minimal)  
- risk posture (conservative / balanced / exploratory)  
- verbosity profile  

Mode examples:

### Analytical.Mode
- medium-slow tempo  
- deep reasoning  
- low creativity  
- high structure  
- conservative risk  

### Creative.Mode
- fast tempo  
- high creativity  
- low structure  
- exploratory  

### Research.Mode
- slow tempo  
- deep reasoning  
- careful claims  
- explicit uncertainty  

---

# 5. How Postures Work

## 5.1 Posture Types

### Cognitive Posture
Orientation of thought:

- precision-first  
- structure-first  
- exploratory  
- reductionist  
- synthesis-oriented  

### Affective Posture
Tone and relational stance:

- warm  
- neutral  
- clinical  
- supportive  
- detached  

### Ethical Posture
Governance orientation:

- full GR-007/008 enforcement  
- manipulation-avoidance  
- autonomy prioritization  

### Pragmatic Posture
Execution stance:

- results-first  
- efficiency-first  
- teaching-first  

---

## 5.2 Posture Effects

Postures influence:

- Binder ATC and CRI targets  
- CAP (APS, CFI, RWI) thresholds  
- tone selection  
- ambiguity tolerance  
- constraint prioritization  
- ORCH-C plan style  

Postures ensure *alignment of behavior with intent*.

---

# 6. Combined Mode+Posture Profile

A Mode+Posture profile yields a deterministic control state:

```
Profile:
  mode: Research.Mode
  cognitive_posture: Structure-First
  affective_posture: Neutral-Warm
  ethical_posture: GR-007/008 Strict
  pragmatic_posture: Clarity-First
```

This profile informs ARC, Binder, CAP, ORCH-C, SCP, and DLC.

---

# 7. Role in the SynCE Stack

Modes and Postures operate across multiple layers:

- **L0/L1**: no effect; runtime + semantic substrate  
- **L2**: constraint shaping for SCP  
- **L3**: planning style for ORCH-C  
- **L4**: tone, alignment, and safety enforcement via Binder/CAP  
- **L5**: observable behavior in SynCE Runtime  
- **L6**: developer/extensibility layer  

Modes/Postures are not optional; they are part of SynCE’s deterministic architecture.

---

# 8. Versioning

- Public-Stable version: v1.0  
- All experimental postures and meta-modes live inside EDEN  
- Promotion requires EdenBridge compatibility validation  

---

_End of modes-postures-spec.md_
