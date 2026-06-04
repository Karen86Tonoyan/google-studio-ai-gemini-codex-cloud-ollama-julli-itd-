# ALFA 360 Studio Overview

Status: architecture draft  
Scope: public-safe technical overview

## Purpose

ALFA 360 Studio is a multi-agent AI operations workbench.

It is designed to help an operator compare model outputs, work with repositories, inspect browser state, validate AI responses, detect prompt-injection risk, and keep a structured audit trail.

It is not a clone of any commercial product.

## Core Workflow

```text
User / Operator
  -> intent capture
  -> provider selection
  -> model execution
  -> response comparison
  -> ALFA 360 Control Layer
  -> PASS / HOLD / REJECT
  -> audit event
  -> human/operator decision
  -> controlled action
```

## Main Components

### Provider Registry

Stores available AI providers, local models, API-compatible endpoints, model metadata, cost notes, limits, and activation status.

### Mass Chat

Sends one prompt to multiple selected models and displays responses side by side.

### Repository Workspace

Allows project-aware coding workflows, file inspection, diff review, task planning, and GitHub-oriented work.

### Browser Workspace

Captures browser/page state for inspection, navigation, testing, and website audits.

### Control Layer

Validates AI output before trust, storage, publication, or downstream execution.

### Audit Log

Stores structured events for every important operation.

## Safety Principle

No model output is trusted automatically.

An AI response is a candidate, not a fact.

## MVP Boundary

The first MVP should focus on:

- provider registry,
- mass chat,
- local/Ollama support,
- OpenAI-compatible provider interface,
- manual PASS / HOLD / REJECT,
- JSONL audit log,
- public-safe documentation.

Do not start with automatic execution of external actions.
