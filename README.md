# OptiAI connector for AI assistants (MCP)

[OptiAI](https://myoptiai.com) is a family life manager: tasks, calendar, home, health, wealth, childcare, pets and more. This connector lets your AI assistant use OptiAI on **your own data**, with your permission, through the open [Model Context Protocol](https://modelcontextprotocol.io) (MCP).

This repository contains documentation only. There is no source code here. The connector is a hosted remote server.

## Connector details

| | |
|---|---|
| Server URL | `https://optiai.me/mcp` |
| Transport | Streamable HTTP (remote server) |
| Authentication | OAuth 2.1 with PKCE. You sign in with your OptiAI account and approve access on a consent screen. |
| Plan | Included with the OptiAI One plan |
| Support | support@optiai.me |

## Connect

You need an OptiAI account. Create one at [myoptiai.com](https://myoptiai.com).

### Claude

1. In Claude, open **Settings > Connectors > Add custom connector** (available on plans that support custom connectors).
2. Paste `https://optiai.me/mcp`.
3. Sign in with your OptiAI account when prompted and choose which areas of OptiAI the assistant may access.

### ChatGPT

A ChatGPT listing is coming. Where your ChatGPT plan supports custom MCP connectors, you can add `https://optiai.me/mcp` the same way.

### Cursor and other MCP clients

Any MCP client that supports remote streamable-HTTP servers with OAuth can connect using `https://optiai.me/mcp`. A one-tap Cursor install is on the in-app connect page at https://optiai.me/connect-ai.

## What your assistant can do

With the access you approve, an assistant can read, and where you allow it, update:

- Goals, tasks and planning
- Calendar and routines
- Home: groceries, pantry and inventory
- Wealth: net worth, accounts and savings goals
- Health: fitness, metrics and medications (kept private and shared only on your terms)
- Travel: trips, packing lists and budgets
- Family and childcare: members, schedules and milestones
- Documents: find a document, check expiry, set reminders (the file itself is never sent)
- Kids' Money: jars, allowance and goals (parent approvals stay confirm-first)

Example requests:

- "Plan my week around my goals."
- "Add milk to the grocery list."
- "How am I tracking toward my savings goal?"

## Privacy and safety

- **You choose the scope.** Access is granted per area, read and write separately, on a consent screen.
- **Your own data only.** The assistant sees only what your own account can see.
- **Confirm before destructive actions.** Deleting or clearing things requires a separate explicit permission and an explicit confirmation.
- **Revoke any time** from Settings > Connected Apps in OptiAI.
- OptiAI does not sell your data. Read the [privacy policy](https://myoptiai.com/privacy).

## Support and security

Questions: support@optiai.me. Security reports: see [SECURITY.md](SECURITY.md).

Learn more: [myoptiai.com](https://myoptiai.com) | [For AI agents](https://myoptiai.com/ai)

## License

Documentation in this repository is MIT licensed (see [LICENSE](LICENSE)). OPTIAI is a registered trademark of Aspire Digital LLC; the name and logo are not covered by this license.
