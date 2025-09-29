# Enable Claude Sonnet 4 for All Clients

This repo now ships with a LiteLLM proxy that exposes an OpenAI-compatible API and routes common model names (like `gpt-4o`) to Anthropic Claude Sonnet 4.1.

## Quick Start

1. Create a `.env` file from the example and add your key(s):

```bash
cp .env.example .env
# Edit .env and set ANTHROPIC_API_KEY=sk-ant-...
```

1. Start services:

```bash
docker-compose up -d
```

1. Point your clients at the proxy:

- Base URL: `http://localhost:4000/v1`
- API Key: any string (or set `x-litellm-api-key` if you configure one)
- Model: use any of these and they’ll route to Claude Sonnet 4.1:
  - `gpt-4o`, `gpt-4o-2024-08-06`, `gpt-4.1`, `gpt-4`, `gpt-4-turbo`, `gpt-3.5-turbo`
  - `claude-3-7-sonnet`, `claude-3-7-sonnet-2025-06-20`
  - `default`

This makes most existing OpenAI-compatible workflows work without changes.

## Using Inside n8n

For nodes that expect OpenAI:

- Set the base URL to `http://litellm:4000/v1` (in Docker network) or `http://localhost:4000/v1` from your host.
- Put any string as the API key (or configure LiteLLM auth).
- Choose a mapped model name (e.g., `gpt-4o`).

For nodes that support Anthropic directly:

- You can keep using Anthropic nodes with your `ANTHROPIC_API_KEY`.

## Notes

- Ensure `ANTHROPIC_API_KEY` is set; otherwise, Claude routing will fail.
- You can extend `config/litellm_config.yaml` to add more routes (e.g., Gemini, Mistral via OpenRouter).
