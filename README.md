# AGI-Development (AGIPragma)

Documentation core for AGIPragma: a research framework for **developmental intelligence under changing worlds**.

This repository contains the conceptual foundation, doctrine, and theoretical definitions
of the AGIPragma research program. It has no runnable code — for the implemented Decision
Intelligence Core and reproducible benchmarks, see AGI-Pragma-Core below.

---

## Documents

- `AGI_DEVELOPMENT.md` — framework definition and core thesis
- `WORLD_VARIABLES_CATALOGUE.md` — conceptual variable map for World Shifts
- `DOCTRINE_OF_DISCONNECTED_INTELLIGENCE.md` — autonomy without central guidance
- `SAFETY_AND_DOCTRINE.md` — safety commitments and research boundary
- `PROJECT_SCOPE.md` — what this is / is not
- `CITATION.cff` — citation metadata
- `CHANGELOG.md` — release notes
- `COMMERCIAL_LICENSE.md` — commercialisation boundary (separate agreement required)

---

## Related Repositories

### [AGI-Pragma-Core](https://github.com/zabinskirafal/AGI-Pragma-Core) — runnable implementation

The primary implementation repository. Contains:

- **Decision Intelligence Core (DIC)** — the full 7-stage pipeline:
  Branching → Critical Path (Monte Carlo) → FMEA → Decision Gate → Circuit Breaker → Selection → Belief Update
- **Snake benchmark** — 10×10 grid, avg score 22.8 over 50 episodes
- **Maze benchmark** — 15×15 grid, 100% solve rate (50/50) after BFS distance utility
- `docs/decision-governance.md` — DIC as a governance layer for agentic AI systems
- `docs/applications.md` — domain application example (accelerometer-based anomaly detection)

If you want to run AGIPragma, start there:
```bash
git clone https://github.com/zabinskirafal/AGI-Pragma-Core.git
cd AGI-Pragma-Core
pip install -r requirements.txt
python3 -m benchmarks.snake.run
python3 -m benchmarks.maze.run
```

### [developmental-agi-sandbox](https://github.com/zabinskirafal/developmental-agi-sandbox) — simulation environment

Unity-based reverse-physics sandbox for testing AGIPragma under non-stationary world rules
(inverted gravity, reversed causality, non-binary logic). Designed to stress-test
decision integrity where the rules of the environment change mid-episode.

---

## How the Repositories Relate

```
AGI-Development (this repo)
  Concepts, doctrine, theoretical framework
        │
        │ implements
        ▼
AGI-Pragma-Core
  Decision Intelligence Core + benchmarks (Snake, Maze)
        │
        │ stress-tests under non-stationary rules
        ▼
developmental-agi-sandbox
  Unity physics-breaking simulation environment
```

This repo defines **what** AGIPragma is.  
AGI-Pragma-Core defines **how** it works in code and measures it in benchmarks.  
developmental-agi-sandbox defines the **adversarial environment** it must survive.

---

## Licensing & Commercial Use

**Author:** Rafał Żabiński

**Free use:** academic research, education, non-commercial projects.

**Commercial use:** requires a separate written agreement. See `COMMERCIAL_LICENSE.md`.

zabinskirafal@outlook.com  
https://www.linkedin.com/in/zabinskirafal
