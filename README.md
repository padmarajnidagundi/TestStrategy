# TestStrategy

A public-facing Lean Canvas test strategy for AI agents and MCP-enabled systems.

## Live Demo

- https://padmarajnidagundi.github.io/TestStrategy/

## Overview

This repository hosts a one-page Lean Canvas that turns AI agent quality risks into test scenarios, measurable quality gates, and a continuous improvement loop.

## QA/Test Engineer Steps: Lean Canvas for Test Strategy in the AI Agentic Era

Based on the thesis document (`PD_Nidagundi_FINAL_A4.pdf`) and the public page in `index.html`, use the canvas as a focused, continuously updated test strategy:

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

- Nine-block AI Agent test strategy Lean Canvas
- MCP and API contract-testing considerations
- Scenario, safety, drift, and rollback test priorities
- Risk and quality metrics for release decisions
- Continuous discover-specify-execute-improve workflow
- Supporting thesis document

## Project Files

- `index.html` — public AI Agent test strategy Lean Canvas
- `README.md` — project overview and usage information
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
