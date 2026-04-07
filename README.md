# financelog-ai — AI Finance Companion

You talk money with an AI. Your conversation is processed by your chosen LLM provider, not by us. No accounts, no tracking, and no data uploads to our servers. You run this.

**Live Demo:** https://financelog-ai.casey-digennaro.workers.dev

---

## Why This Exists
Many financial tools require extensive data access. This provides a simple alternative: a private space to run calculations, weigh purchase decisions, or plan savings, without the surrounding product ecosystem.

## Quick Start
1.  **Fork** this repository.
2.  Deploy to Cloudflare Workers: `npx wrangler deploy`
3.  Add your LLM API key (e.g., for DeepSeek, OpenRouter, or OpenAI-compatible providers) as a Worker secret. No other configuration is required.

## Features
- **Your Data, Your Worker:** All chat data is processed within your own Cloudflare Worker instance.
- **Minimal Interface:** A single-page UI that functions adequately on mobile.
- **Zero Dependencies:** One TypeScript file under 300 lines.
- **Stateless Design:** By default, conversations are ephemeral and vanish on refresh. You can optionally add Cloudflare KV for persistence.
- **Fork-First:** This is a starting template. Modify or replace any part of the code.

## What Makes This Different
1.  **No Central Service:** Your fork operates independently. We do not host, monitor, or access your instance.
2.  **No Product Funnel:** There is no onboarding, account creation, or feature upselling.
3.  **No Financial Steering:** The AI provides calculations and discussion. It does not promote financial products or services.

## Limitations
- This is a basic, single-file application. It does not include features like file uploads for statement analysis or built-in multi-turn conversation memory without manual KV setup.

## License
MIT License.

<div style="text-align:center;padding:16px;color:#64748b;font-size:.8rem"><a href="https://the-fleet.casey-digennaro.workers.dev" style="color:#64748b">The Fleet</a> &middot; <a href="https://cocapn.ai" style="color:#64748b">Cocapn</a></div>