# Launch Llama for Cursor

Launch your product without leaving Cursor. This plugin connects Cursor to the [Launch Llama](https://tools.launchllama.co) MCP server and adds skills for the jobs founders do around a launch.

## What you get

**MCP server** (`launchllama`, no sign-in needed)

| Tool | What it does |
|---|---|
| `check_launch_readiness` | Audits a URL for meta tags, Open Graph, favicon, pricing and more |
| `list_launch_directories`, `plan_directory_campaign` | Where to launch and in what order |
| `search_products`, `get_top_products`, `get_product`, `list_categories` | Search the live Launch Llama tools directory |
| `submit_product`, `get_submission` | Open a free listing draft (the founder finishes it by email) |
| `get_badge_snippet`, `verify_badge` | Add and verify the Launch Llama badge |
| `get_newsletter_ad_options`, `get_first_users_report` | Newsletter ads and first-users ideas |

**Skills**

- `launch-readiness-check`: audit your site and fix the issues in your code
- `directory-launch-campaign`: plan your directory launch and open a listing
- `find-tools`: find and compare SaaS and AI tools

**Rules**

- `launch-llama.mdc`: guardrails so the agent uses real data and never publishes or pays for you

## Install

Install from [Cursor Directory](https://cursor.directory), or add the server by hand in `~/.cursor/mcp.json`:

```json
{
  "mcpServers": {
    "launchllama": { "url": "https://tools.launchllama.co/mcp" }
  }
}
```

Founders who want to manage their own listing (analytics, edits, changelog) can add the signed-in server instead: `https://tools.launchllama.co/mcp/founder`.

## Links

- Website: https://tools.launchllama.co
- MCP docs: https://tools.launchllama.co/developers/docs/mcp-install
- REST API (OpenAPI): https://kxdushqmihjyuddcwkpw.supabase.co/functions/v1/api-v1/openapi.json

## License

MIT
