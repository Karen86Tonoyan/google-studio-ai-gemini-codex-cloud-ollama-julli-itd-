# ALFA 360 Studio

ALFA 360 Studio is a multi-agent AI operations workbench.

It combines model comparison, project-aware coding workflows, browser inspection, AI output validation, prompt-injection scanning, audit logging, and human-in-the-loop control.

This project is not a clone of Google AI Studio, Claude Code, Codex, Gemini, or any commercial product.

It is an ALFA-native control environment for working with multiple AI systems safely.

## Product Positioning

This repository may explore workflow patterns commonly found in modern AI developer environments:

- playground-style prompt testing,
- multi-model comparison,
- project and repository context,
- coding-agent workflows,
- browser inspection,
- local model routing,
- cloud model routing,
- audit and validation layers.

The product identity, architecture, safety layer, UI language, and execution model must remain ALFA-native.

Do not copy branding, UI assets, logos, product names, protected layouts, or proprietary UX text from Google, OpenAI, Anthropic, or any other provider.

## Core Idea

One prompt can be sent to many models.

No model output is trusted automatically.

Every output can pass through the ALFA 360 Control Layer before it becomes a decision, stored memory, public content, or downstream action.

## Planned Modules

- Provider Registry
- Mass Chat
- Single Model Chat
- Repository Workspace
- Browser Workspace
- Tonoyan Filters
- Cerber Decision Gate
- Lasuch Prompt-Injection Scanner
- Guardian Monitoring
- Audit Log
- Human Review Queue

## Safety Model

```text
User intent
  -> model/provider selection
  -> AI output
  -> validation layer
  -> PASS / HOLD / REJECT
  -> audit event
  -> human/operator decision
  -> controlled action
```

## Provider Onboarding

New providers must follow:

```text
Discover -> Review -> Sandbox -> Register -> Enable
```

No unreviewed provider, plugin, or external model connector should be enabled automatically in production.

## MVP Scope

### Phase 1

- Provider Registry
- OpenAI-compatible provider interface
- Gemini provider
- Anthropic provider
- Ollama/local provider
- Mass Chat
- Response comparison
- Audit log JSONL
- Manual PASS / HOLD / REJECT

### Phase 2

- Tonoyan Filters integration
- Cerber automated decision gate
- Prompt injection scanner
- Repository workspace
- Browser snapshot workspace

### Phase 3

- Human review queue
- Project memory
- WordPress / GitHub connectors
- Local deployment package

## Status

Architecture draft / MVP planning.
