# version-aware-support-assistant
A version-aware RAG support assistant with source citations and reproducible evaluation.

# Version-Aware Technical Support Assistant

> Status: Planning. Implementation has not started.

## Problem

Developers and support engineers troubleshoot software using
documentation, release notes, and GitHub discussions. Information
can be scattered, outdated, or relevant only to particular versions.

## Goal

Build an assistant for one open-source Python product that answers
technical questions using retrieved evidence and provides citations.

The product will be selected after reviewing candidate datasets.

## Intended behavior

- Retrieve relevant information from a defined collection of sources.
- Generate answers supported by those sources.
- Explain version differences when the evidence supports them.
- Acknowledge insufficient or conflicting evidence.

## Initial scope

- One open-source Python product.
- Official documentation, release notes, and selected GitHub issues.
- A repeatable ingestion and retrieval pipeline.
- Answers with inspectable citations.
- A reproducible evaluation harness.
- A simple deployed interface with latency and cost tracking.

## Outside the initial scope

- Training a language model.
- Supporting multiple products.
- Searching the entire internet.
- Executing generated code or changing a user's environment.

## Evaluation plan

Create manually checked questions with expected facts and supporting
sources. Compare a baseline with improved retrieval approaches.

Measure retrieval quality, answer correctness, faithfulness,
citation support, abstention behavior, latency, and cost.

Keep a held-out test set separate from development questions.
Set numerical targets after establishing the baseline.

## Planned deliverables

- Working application.
- Reproducible source code and setup instructions.
- Evaluation dataset and results.
- Architecture diagram.
- Engineering case study and short demo.
