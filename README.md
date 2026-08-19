# UREx_LuJianyi

## Active Mapping using 3D Scene Graphs: A Review and Implementation

This project investigates active mapping using hierarchical 3D scene graphs. It studies how scene-graph information can guide robot exploration and Next-Best-View (NBV) selection, with the goal of understanding whether structured semantic representations can improve active exploration compared with geometry-only approaches.

The project combines paper-level code analysis, simulation-based reproduction, systematic evaluation, targeted improvements, and, where feasible, real-robot validation on TIAGo or B2.

## Research Questions

1. How have 3D scene representations evolved from geometric and hierarchical scene graphs to semantic and open-vocabulary representations?
2. Which existing methods perform genuine active mapping, where the current representation influences the next sensing or viewpoint action?
3. How can hierarchical 3D scene graphs support NBV selection and active exploration?
4. Does scene-graph-guided exploration outperform geometry-only frontier exploration under equivalent exploration budgets?
5. What lightweight improvements can improve NBV performance and robustness to real-world sensor noise?

## Project Structure

### Task 1 — Baseline Framework Programming Analysis and Simulation Reproduction

Analyze and reproduce selected existing methods on a paper-by-paper basis, with particular emphasis on source-code analysis and the complete perception–mapping–planning loop.

### Task 2 — Active Mapping Capability Evaluation

Evaluate active mapping methods in cluttered, irregular, and semantically ambiguous environments and assess their usefulness for downstream scene-graph tasks.

### Task 3 — Targeted Lightweight Improvements

Investigate improvements to NBV objectives and robustness to RGB-D and pose noise.

### Task 4 — Real-Robot Validation

Validate the scene-graph and NBV pipeline on TIAGo and/or B2 where feasible.

### Task 5 — Project Consolidation

Consolidate the literature review, implementations, experiments, evaluation, ablations, visualizations, and research findings into a reproducible technical report and final presentation.

## Research Hypotheses

**H1:** Compared with fixed-trajectory and geometry-only frontier methods, hierarchical scene-graph-guided NBV planning achieves higher scene-graph accuracy, semantic and geometric coverage, uncertainty reduction, and object/room discovery rates under equivalent exploration budgets.

**H2:** The resulting actively constructed scene graphs provide more reliable support for high-level tasks such as semantic queries, object localization, and goal-directed navigation, particularly in cluttered or atypical environments.

## Repository Organization

```text
UREx_LuJianyi/
├── README.md
├── proposal/
│   └── proposal.md
├── task1-reproduction/
│   ├── README.md
│   ├── paper-list.md
│   └── papers/
├── task2-evaluation/
│   └── README.md
├── task3-improvements/
│   └── README.md
├── task4-real-robot/
│   └── README.md
└── task5-consolidation/
    └── README.md