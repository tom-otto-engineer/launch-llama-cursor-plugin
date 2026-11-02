---
name: directory-launch-campaign
description: Plan where to launch a product (Product Hunt alternatives, AI and SaaS directories, newsletters) using Launch Llama's directory data, and open a free Launch Llama listing draft. Use when someone asks where to launch, how to get backlinks, or how to get their first users.
---

# Directory launch campaign

1. Collect the product URL, a one-line description, and the category. Use `list_categories` to pick a category that exists.
2. Call `list_launch_directories` to see the directories Launch Llama tracks, then `plan_directory_campaign` with the product details to get an ordered plan.
3. Present the plan as a short table: directory, why it fits, dofollow or not, effort.
4. Offer to open a free listing on Launch Llama with `submit_product` (needs the founder's email). This only creates a draft: the founder gets an email with a link and finishes the listing themselves.
5. Once the listing is live, call `get_badge_snippet` and add the badge to the site footer, then `verify_badge` to confirm it is detected.

Never publish, pay or choose a plan on the founder's behalf.
