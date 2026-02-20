# mcp-wikivoyage

MCP server for travel destination information via the [Wikivoyage](https://www.wikivoyage.org)
MediaWiki API. Get travel guides, destination overviews, and practical travel information for
cities and regions worldwide.

> **Status: Work in Progress** — Server scaffolding is in place. Tools are not yet implemented.

---

## Prerequisites

- [Bun](https://bun.sh) runtime (`curl -fsSL https://bun.sh/install | bash`)
- No API keys needed — Wikivoyage is free and open

---

## Planned Tools

- `wikivoyage_search` — Search for travel destinations by name
- `wikivoyage_get_article` — Get the travel guide for a destination (sections: understand, get in, get around, see, do, eat, sleep, connect)
- `wikivoyage_get_nearby` — Find Wikivoyage articles for destinations near a coordinate

---

## Data Source

[Wikivoyage](https://www.wikivoyage.org) is a free, community-written travel guide, part of
the Wikimedia Foundation. Content is licensed under CC BY-SA 3.0. The MediaWiki API is free
to use with no registration required (rate limits apply for bulk access).

---

## Install

```bash
git clone git@github.com:McCullonas/mcp-wikivoyage.git
cd mcp-wikivoyage
bun install
```

---

## MCP Client Configuration (once implemented)

```json
{
  "mcpServers": {
    "wikivoyage": {
      "command": "bun",
      "args": ["run", "/path/to/mcp-wikivoyage/src/index.ts"]
    }
  }
}
```

---

## Licence

MIT
