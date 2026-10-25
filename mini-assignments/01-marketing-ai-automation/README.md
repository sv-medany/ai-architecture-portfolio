# Mini Assignment 1: Marketing Automation with AI & Agents

## Overview
Architecture governance proposal for an AI-driven
marketing automation platform, with real-time cart
triggers and scheduled segmentation, where
authorization stays outside the model.

## Deliverables
- [governance-design-proposal.pdf](governance-design-proposal.pdf):
  governing principles, ADRs, review board evidence,
  policy guardrails and reference architecture with
  trust boundaries
- [component-architecture-diagram.pdf](component-architecture-diagram.pdf):
  component-level architecture and data flows

## Governing Principles
- AP-01 Risk-based oversight
- AP-02 Privacy and least privilege (PDPL)
- AP-03 Reliable, auditable execution
- AP-04 Measurable, cost-aware AI

## Key Decisions
- ADR-001: Hybrid campaign processing (nightly batch + event-driven triggers)
- ADR-002: Tiered model routing (rules, small models, managed LLMs)
- ADR-003: Structured and semantic retrieval (authoritative stores + optional vector index)

## Open Decisions
- Confirm PDPL jurisdiction and approval owners
- Benchmark model costs and latency
- Verify provider idempotency
- Define whether the five-second SLA covers submission or delivery
