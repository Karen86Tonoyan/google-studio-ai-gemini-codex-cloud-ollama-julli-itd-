# Provider Registry

## Purpose

The Provider Registry manages all available AI providers and model endpoints.

## Supported Types

- OpenAI-compatible APIs
- Anthropic
- Gemini
- Ollama
- DeepSeek
- Mistral
- Custom providers

## Provider Lifecycle

```text
Discover
  -> Review
  -> Sandbox
  -> Register
  -> Enable
```

## Provider Metadata

Suggested fields:

- provider_name
- model_name
- endpoint
- api_key_source
- context_window
- pricing_notes
- local_or_cloud
- enabled
- notes

## Safety Rules

- Disabled providers cannot be used.
- Experimental providers should remain sandboxed.
- New providers require review before activation.
