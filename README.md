# TestStrategy

A public-facing Lean Canvas page for an AI testing strategy dashboard, plus real-use-case example boards for test strategy building.

## Live Demo

- https://padmarajnidagundi.github.io/TestStrategy/

## Overview

This repository hosts a single-page Lean Canvas and twelve test strategy example boards. The goal is to show both a primary canvas and practical real-use-case examples of how Lean Canvas can be used for test strategy planning.

## QA/Test Engineer Steps: Lean Canvas for Test Strategy in the AI Agentic Era

Based on the thesis document (`PD_Nidagundi_FINAL_A4.pdf`) and the visual board in `index.html`, use Lean Canvas as a one-page, continuously updated test strategy:

1. Define **Problem**: capture top quality risks (non-deterministic agent behavior, tool-call failures, safety/policy gaps, drift).
2. Identify **Customer Segments**: QA leads, engineering teams, release managers, product stakeholders.
3. Write **Unique Value Proposition**: one clear statement of quality value (fast, visible, risk-based confidence).
4. Define **Solution**: scenario-flow tests, tool/API contract tests, safety guardrail tests, benchmark/evaluation datasets, resilience checks.
5. Select **Key Metrics**: escaped defects, risk-based coverage, scenario pass rate, strategy-to-execution cycle time.
6. Set **Channels**: sprint planning, strategy workshops, release-readiness reviews, project governance meetings.
7. Record **Unfair Advantage**: reusable templates, domain test patterns, institutional knowledge, proven framework.
8. Estimate **Cost Structure**: dashboard/automation effort, environments, data preparation, training and maintenance.
9. Clarify **Revenue Streams / Impact**: lower rework, faster safe releases, improved reliability and decision quality.
10. Iterate continuously: update the board every sprint/release based on defects, incidents, and feedback.

## Included

- Public GitHub Pages Lean Canvas page
- One-page business model overview
- Featured AI Agents test strategy Lean Canvas example
- Twelve Lean Canvas examples with problem, solution, and impact
- Full nine-block Lean Canvas example based on the doctoral thesis case
- Supporting visual asset for the initiative
- Simple project documentation

## Project Files

- `index.html` — one-page Lean Canvas with twelve test strategy examples and one full thesis-based nine-block board
- `README.md` — project overview and usage information
- `Lean_Canvas_Test_Strategy_Dashboard.jpg` — dashboard image asset
- `PD_Nidagundi_FINAL_A4.pdf` — supporting project document

## Local Preview

From the repository root, run:

```bash
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Repository

- GitHub: https://github.com/padmarajnidagundi/TestStrategy

## Notes

The project is intentionally kept simple and easy to navigate, with the public site centered around the dashboard concept and core project information.
