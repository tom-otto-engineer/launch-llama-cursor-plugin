---
name: find-tools
description: Find and compare SaaS and AI tools from the live Launch Llama directory. Use when someone asks "what's a good tool for X", wants alternatives to a product, or wants the top launches this week.
---

# Find tools

1. For a specific need, call `search_products` with a short keyword query. Add a category filter from `list_categories` if the need is clear.
2. For "what's trending" or "best this week", call `get_top_products`.
3. Call `get_product` on the two to four best matches to get pricing and details.
4. Answer with a short comparison: name, what it does, pricing, and the Launch Llama link from the tool result.

Only recommend products the tools returned. Do not make up pricing or features.
