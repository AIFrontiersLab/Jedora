# Jedora

![AI](https://img.shields.io/badge/domain-AI%20%2B%20Agentic-0ea5e9?style=for-the-badge) ![Jedora](https://img.shields.io/badge/project-Jedora-111827?style=for-the-badge) ![Status](https://img.shields.io/badge/status-isolated%20prototype-22c55e?style=for-the-badge)

> A product that only exists because Authorization and Robotics now work together.

**Concept:** Authorization × Robotics Operator

**Repository:** [https://github.com/AIFrontiersLab/Jedora](https://github.com/AIFrontiersLab/Jedora)

---

## Why this exists

Authorization and Robotics are appearing in overlapping research and product activity.

**Why now:** These technologies started showing up in the same signal clusters this cycle.

**What recently changed:** Signal cluster formed across independent sources.

**Why it was hard before:** At least one of the ingredients was too weak, expensive, or unstandardized.

---

## Product thesis

| | |
|---|---|
| **Future thesis** | Independent signals mention both Authorization and Robotics; their joint capability is not yet a named product category. |
| **First customer** | A lab or startup already combining two of the three |
| **Market** | Emerging infrastructure |
| **Convergence** | Authorization, Robotics |
| **Moat** | Workflow data at the intersection. |

---

## MVP

A narrow demo that only works if all colliding capabilities are present.

### Core loop

1. Accept an agent (or human-on-behalf-of-agent) intent
2. Enforce scope / policy / evidence
3. Execute the smallest useful autonomous step
4. Leave an audit trail a human can kill-switch

---

## Architecture

```text
Adapters for each capability + a joint orchestration core.
```

```mermaid
flowchart LR
  subgraph Product["Jedora"]
  A["Intent / capture"]
  B["Policy & clustering"]
  C["Proposal UI"]
  D["Operator / audit"]
  end
  A --> B
  B --> C
  C --> D
```

---

## Start

```bash
python3 -m http.server 4173 --directory .
```

---

## Why it may win

Category does not yet have an incumbent owner.

## Why it may fail

The collision is interesting but not a job-to-be-done.

### Risks

- One of the technologies remains a toy

### Unknowns

- Which node is actually the bottleneck

### Current alternatives

- Stitching tools together manually

### Assumptions

- Agent workflows will keep expanding into real systems

---

## Scope

This project is intentionally scoped to **AI and Agentic AI** only.

---

## Tags

`ai` `agentic-ai` `autonomous-agents` `jedora` `prototype` `authorization` `robotics`
