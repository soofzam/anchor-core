Anchor Research Note v0.1
Epistemic Responsibility Failures in Modern LLM Outputs
Status

Version 0.1 – Foundational probe
Scope: Behavioral stress test, not statistical benchmark
Intent: Motivate normative requirements for epistemically responsible AI systems

Abstract

This note reports findings from a behavior-focused probe evaluating epistemic responsibility in large language model (LLM) outputs.

The objective is not to rank models or claim statistical generality.
The objective is to identify repeatable failure classes induced by common prompt structures.

Across 52 responses from four models, 42.3% violated predefined epistemic-responsibility expectations under adversarially normal prompts.

These findings motivate the need for a vendor-neutral standard defining minimum responsible behaviors for AI-generated answers.

Dataset

Source: Test A+c+d.xlsx
Prompts: 13

A01–A10 (epistemic traps)

C01 (closed-world recall)

D01–D02 (real-world resource recommendations)

Total responses evaluated: 52 (13 prompts × 4 models)

Rows C02–C05 and D03–D05 exist in the file but were excluded due to missing responses.

Scoring Method

Each response was scored against the “Expected Responsible Behavior” defined per prompt.

Binary classification:

Compliant — behavior matches expected responsible response class

Noncompliant — behavior violates epistemic responsibility

Noncompliant responses were tagged with failure types.

This probe is structure-first: it is designed to reveal systematic epistemic weaknesses triggered by prompt structure.

Headline Results

Overall compliance:

30 / 52 compliant (57.7%)

22 / 52 noncompliant (42.3%)

Interpretation: Under epistemic pressure, noncompliance is frequent.

Prompt Sensitivity

Performance varied sharply by prompt type:

100% pass: A01, A03, A09

75% pass: A04, D02

50% pass: A06, A07, A08, D01

25% pass: A02, A05, A10, C01

Interpretation: Certain question structures systematically induce failure across models.

Failure Classes Observed

False precision under uncertainty

Speculative single-winner certainty

Forced binary acceptance

Unjustified objective ranking

Authority or citation misrepresentation

Closed-world hallucination

Actionable contact-detail mismatch

Failures appear across vendors and are not isolated to a single system.

High-Stakes Spot Checks

Closed-world recall:
At least one response cited specific episode information that does not align with documented episode descriptions.

Real-world resources:
At least one response provided concrete contact details conflicting with official sources.

These represent high-severity epistemic risk classes.

Limitations

Small-N probe

Single-rater scoring

Stress-case prompts

Limited external verification

This document motivates standards discussion.
It does not claim universal prevalence.

Implication

LLMs frequently prefer plausible specificity over explicit uncertainty under epistemic stress.

This structural tendency motivates a minimum behavioral standard for responsible AI systems.
