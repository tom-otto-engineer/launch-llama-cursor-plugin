---
name: launch-readiness-check
description: Audit a product URL before launch (meta tags, Open Graph, favicon, pricing, social proof and more) with the Launch Llama MCP, then fix what it finds in the codebase. Use when someone is about to launch or asks "is my site ready to launch?".
---

# Launch readiness check

1. Ask for the live URL of the product if it is not obvious from the repo (look for `homepage` in package.json, a `CNAME`, or the site URL in config).
2. Call the `check_launch_readiness` tool from the `launchllama` MCP server with that URL.
3. Group the result into: blocking issues, quick wins, and nice-to-haves.
4. For every issue that can be fixed in this codebase (missing `<title>`, meta description, `og:image`, favicon, canonical tag, sitemap, robots.txt), find the file and propose the exact change.
5. Re-run `check_launch_readiness` after the fixes are deployed and report the new result.

Never invent scores. Only report what the tool returned.
