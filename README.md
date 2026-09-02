# Autoview MCP

Trade across [22+ exchanges and brokers](https://autoview.com/platforms/) from any MCP-capable AI agent. Autoview's MCP server is a hosted, remote endpoint, no install, no local server to run.

## Endpoint

```
https://api.autoview.com/mcp/
```

## Authentication

Generate a personal access token at [autoview.com/account/tokens/](https://autoview.com/account/tokens/) (Account menu -> MCP tokens). Set a label, an expiry, and the scopes you want, then copy the token when it appears -- it's shown once. Pass it as the `token` argument on every tool call.

## Tools

- **entry** -- place an order (dry-run by default; every call is a preview unless you explicitly set `live: true`)
- **events** -- read back the outcome of an entry call by its trace id

## Live trading coverage

Live (real-money) trading is currently available on Kraken and Crypto.com through the MCP. Every other supported exchange is simulation-only for now (Tradovate, OANDA Practice, Bybit Testnet/Spot Testnet, Crypto.com Demo, and more), so you can wire up an agent and watch it work before pointing it at a funded account.

## Full guide

The complete getting-started guide, including a step-by-step token walkthrough, request/response examples, and the custom-client connection handshake, lives at:

**[autoview.com/guides/mcp-getting-started/](https://autoview.com/guides/mcp-getting-started/)**

## About Autoview

[Autoview](https://autoview.com/) turns any webhook-driven signal (TradingView alerts, custom bots, AI agents) into live, automated execution across 22+ exchanges and brokers.
