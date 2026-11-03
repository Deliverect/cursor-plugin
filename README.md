# Deliverect for Cursor

Connects Cursor to [Deliverect](https://www.deliverect.com), so you can ask about your restaurant's sales, orders, menus and opening hours across every location and ordering channel, using live data.

Deliverect connects restaurants and retailers to the delivery apps, web shops and kiosks their customers order from. This plugin adds the hosted Deliverect MCP server (`https://mcp.deliverect.com/mcp`) to Cursor.

## What you can ask

- Which products sold best this month?
- How does revenue compare between locations?
- Which orders failed yesterday?
- What are the holiday hours for my stores?

The server can look up orders and their status, billing and product sales reports, stores and their opening hours, menus and the product catalog, menu schedules and special hours, and operational health such as paused channels and failed menu pushes.

## Install

Install it from the Cursor Marketplace, or add it by hand:

[Add to Cursor](cursor://anysphere.cursor-deeplink/mcp/install?name=deliverect&config=eyJ1cmwiOiJodHRwczovL21jcC5kZWxpdmVyZWN0LmNvbS9tY3AifQ==)

Or put this in `~/.cursor/mcp.json`:

```json
{
  "mcpServers": {
    "deliverect": {
      "url": "https://mcp.deliverect.com/mcp"
    }
  }
}
```

## Sign in

Cursor opens a browser window the first time a tool runs. Sign in with your Deliverect account. There are no API keys to configure. The first time, you'll be asked to accept the connector's terms.

## Privacy and access

- Every tool is read-only: nothing can change menus, prices, orders or opening hours.
- You see only what your Deliverect user can see in the Deliverect portal.
- Customer and courier details are never returned.

[Privacy policy](https://deliverect.com/en/deliverect-mcp-connector-privacy-policy)

## Support

- Help article: https://help.deliverect.com/
- Email: integrations-support@deliverect.com
