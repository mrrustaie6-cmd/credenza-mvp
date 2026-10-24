# Credenza — Building AI course project

## Summary

Credenza is a concept prototype for a consent-based financial identity layer designed for migrants who carry a real history of payments and financial activity but whose records are not easily portable across borders. The project explores how AI and data verification could help organize scattered evidence into a human-readable trust signal for lenders, onboarding teams, and case reviewers.

This repository is a Building AI course project. It is intentionally framed as a demonstration: it shows how an AI-assisted trust profile could work, while remaining explicit about what is still a concept and what is not yet operational.

## Background

Many people move across borders with a real financial history that exists in bank statements, payment records, local registries, social references, or transaction trails. However, in practice, that history is often fragmented, hard to verify, or unavailable to new institutions in a different country.

Credenza imagines a system that does not automatically grant trust or credit. Instead, it gathers and organizes evidence, improves explainability, and lets a human reviewer decide whether the information is relevant and reliable.

## How is it used?

The prototype is designed for a simple user journey:

1. A person chooses which sources to share.
2. The system collects or reviews a few representative signals.
3. A lightweight AI-assisted summary ranks the evidence into an experimental trust signal.
4. A bank or reviewer evaluates the result together with documents and context.

In this demo, the user interaction is front-end only. No real financial data is processed, no live bank API is queried, and no credit decision is made.

## Data sources and AI methods

The project uses synthetic, illustrative data for the demo. Example signal categories include:

- Verified pay slips and statements
- On-chain transaction history
- Reference or guarantor signals
- Home-country registry information

The AI logic demonstrated here is intentionally modest and transparent:

- Transaction classification using simple rule-based patterns and label assignment
- Anomaly detection for unusual or high-risk payment behavior
- Aggregation into a single experimental trust signal that summarizes signal quality, consistency, and confidence

This is not a production credit model, and it does not replace underwriting expertise. It is designed to make evidence easier to inspect.

## Challenges

The concept raises several important limitations and risks:

- Consent and data removal: users must be able to revoke access and request deletion of shared evidence
- Bias and exclusion: migrants with different banking histories may be unfairly penalized if signals are interpreted without context
- Document extraction errors: OCR, parsing, and source verification can fail or misread records
- Privacy risk: storing and linking financial evidence across platforms raises serious data protection concerns
- Appeal and correction: users need a clear path to challenge inaccurate or incomplete information

This demo addresses these issues in principle but does not claim to solve them fully.

## What next?

The next step would be to move from synthetic demo data to a small, well-bounded pilot with explicit governance:

- define signal schemas and consent flow
- run a limited evaluation on anonymized or synthetic test data
- test fairness checks against different user profiles
- build a review interface for human decision-making and dispute handling
- clearly separate evidence presentation from final lending decisions

The main goal is not to automate trust. The goal is to improve transparency, reduce manual effort, and let human reviewers act with better context.

## Acknowledgments

This project is a concept and demo prepared as part of the Building AI course project. It draws inspiration from conversations about portable identity, financial inclusion, cross-border onboarding, and explainable AI systems.

It is not a real financial service, credit model, or regulated product. All numbers, signals, and data shown in the interface are illustrative and meant to demonstrate an idea, not to reflect actual creditworthiness.

---

This repository is intentionally explicit about the boundary between prototype and production: the demo helps explain the concept, but the final decision remains with a human reviewer and the relevant institutions.
