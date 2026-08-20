# Task 1 — Paper List & Reproduction Plan

## 1. Paper Categories

| Type | Papers | Relevant to UREx | Main Learning Point |
|---|---|---|---|
| **A. 3DSG Foundations** | Hydra, HOV-SG, DAAAM | Understand the 3DSG representation | How is a 3DSG constructed, updated, and queried? |
| **B. 3DSG / Task-Oriented Understanding** | ConceptGraphs, Clio, 3D-Mem | Understand task-driven representations and alternative scene memory | What information should the robot's memory/graph contain for downstream tasks? |
| **C. Active Mapping without Conventional 3DSG** | ActiveSGM | Learn active-mapping and NBV methodology | How are uncertainty, information gain, and viewpoint selection formulated? |
| **D. 3DSG + Genuine Active Mapping** | Active Semantic Perception, RGB-only Active 3DSG, SCOUT | Directly relevant to the UREx research question | How can the current scene graph determine the next observation? |

---

## 2. Paper Reproduction Plan

### Reproduction Levels

| Level | Meaning |
|---|---|
| **Deep** | Run the system + source-code analysis + reproduce experiments + selected ablations/modifications |
| **Medium** | Run the system + source-code analysis + reproduce selected experiments |
| **Light** | Paper/code analysis + run demo if feasible; no full reproduction |

---

### Type A — 3DSG Foundations

| Paper | Reproduction Level | Main Focus |
|---|---|---|
| **Hydra** | **Deep** | 3DSG construction, hierarchy, graph update, ROS/data pipeline |
| **HOV-SG** | **Medium** | Open-vocabulary semantics and hierarchical graph construction |
| **DAAAM** | **Light** | Semantic representation and scene-graph construction |

---

### Type B — 3DSG / Task-Oriented Understanding

| Paper | Reproduction Level | Main Focus |
|---|---|---|
| **ConceptGraphs** | **Medium** | Open-vocabulary 3DSG and downstream planning |
| **Clio** | **Medium** | Task-driven scene representation; investigate connection to active exploration |
| **3D-Mem** | **Medium** | Visual scene memory, frontier snapshots, and active exploration as an alternative to conventional 3DSG |

**Key question for Type B:**

> Does the task only affect reasoning after mapping, or can task information determine what the robot should observe next?

---

### Type C — Active Mapping without Conventional 3DSG

| Paper | Reproduction Level | Main Focus |
|---|---|---|
| **ActiveSGM** | **Deep** | Uncertainty, information gain, NBV, viewpoint selection, exploration loop |

**Key question:**

> Which parts of the active-mapping/NBV methodology can be transferred to a 3DSG-based system?

---

### Type D — 3DSG + Genuine Active Mapping

| Paper | Reproduction Level | Main Focus |
|---|---|---|
| **Active Semantic Perception** | **Deep** | Hierarchical 3DSG → information gain → next viewpoint |
| **RGB-only Active 3DSG** | **Deep** | Incremental 3DSG construction + active viewpoint selection |
| **SCOUT** | **Deep** | Scene-graph uncertainty + semantic/geometric coverage + active traversal |

**Key question:**

> How does the current scene graph directly influence the next sensing/action decision?

---

## 3. Overall Research Workflow

```text
A. 3DSG Foundations
        ↓
B. Task-Oriented 3DSG / Scene Memory
        ↓
C. Active Mapping / NBV Methodology
        ↓
D. 3DSG + Active Mapping
        ↓
Cross-paper comparison
        ↓
Task-driven Active Mapping
        ↓
Task 2 / Task 3
```
