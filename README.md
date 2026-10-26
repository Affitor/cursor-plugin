# Affitor for Cursor

Read your [Affitor](https://affitor.com) affiliate program from Cursor: partners, commissions, earnings, payouts and billing.

This plugin connects Cursor to the Affitor MCP server at `https://mcp.affitor.com/mcp`. It is **read-only**: it cannot change data or move money.

## What you can ask

**Brands** (program owners) connect one program:
- "Which partners drove the most sales in the last 30 days?"
- "List my pending commissions."
- "How is my program set up, and is the tracker installed?"
- "What is my Affitor bill this week?"

**Partners** connect their partner account:
- "Which programs have I joined?"
- "How much have I earned, and when is it paid?"
- "List my referral links."

## Install

Install **Affitor** from the Cursor Marketplace. Or add the server yourself in `~/.cursor/mcp.json`:

```json
{
  "mcpServers": {
    "affitor": { "url": "https://mcp.affitor.com/mcp" }
  }
}
```

Then open **Cursor Settings** › **MCP**, click **Connect** next to Affitor and sign in with your Affitor account. On the consent screen, choose the program (brands) and click **Allow**.

## Tools

| For | Tools |
|---|---|
| Brands | `get_program`, `list_partners`, `get_partner`, `list_applications`, `list_commissions`, `get_commission_summary`, `get_billing` |
| Partners | `list_my_programs`, `list_my_links`, `get_my_earnings`, `list_my_commissions`, `list_my_payouts` |

What each tool returns, the limits and troubleshooting are in the [MCP guide](https://affitor.com/docs/api-reference/mcp).

## Privacy and support

- Privacy policy: https://affitor.com/privacy
- Terms: https://affitor.com/terms
- Help: https://affitor.com/docs/support or hello@affitor.com

You can disconnect at any time in Affitor: brands under **Settings** › **Developers** › **AI agents**, partners under the account menu › **Integrations**.

## License

MIT
