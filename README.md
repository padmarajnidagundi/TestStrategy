# Test Strategy - Software Testing in AI SDLC (AI-native or agentic software development lifecycle)

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

## Short Case Studies

### 1. MCP Tool Timeout in an Order Support Agent

**Context:** An AI support agent used an MCP inventory tool to check stock before confirming an order.

**Scenario:** The tool was slow, unavailable, and intermittently returned malformed responses during peak traffic.

**Test approach:** QA exercised tool success, timeout, retry, cancellation, partial-failure, and fallback flows. Contract tests verified the required fields and response types, while end-to-end tests confirmed that the agent did not promise an order it could not fulfill.

**Quality gate:** No false confirmations, graceful degradation within the agreed timeout, and 100% pass of critical tool-contract tests.

**Reusable lesson:** Test the agent and its tool boundary together; an agent's natural-language response is only as reliable as the tool result and fallback policy.

### 2. Policy Drift in a Benefits Assistant

**Context:** An employee benefits assistant answered policy questions using a frequently updated knowledge source.

**Scenario:** The model produced outdated eligibility rules and cited source documents that no longer matched the answer.

**Test approach:** QA maintained a versioned evaluation set of policy questions, compared answers across model and knowledge-source versions, and added groundedness checks against approved documents. Human reviewers labeled ambiguous and high-risk answers before release.

**Quality gate:** Critical policy scenarios pass at the approved threshold, every cited source is current, and no high-severity answer is released without human review.

**Reusable lesson:** Test model behavior, retrieval data, citations, and policy updates as one versioned system, not as separate components.

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
