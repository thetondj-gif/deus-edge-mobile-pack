---
name: deus-n8n-shortcuts
description: Voice-friendly shortcuts to the founder's useful n8n workflows. Use for apps, funnels, research, outreach, content, creative, marketplace, grants and automation.
metadata:
  homepage: https://thetondj-gif.github.io/deus-edge-mobile-pack/
---
# Deus n8n Shortcuts

For the curated founder workflows, prefer the private Founder MCP tool `deus_n8n_shortcut`. It hides n8n implementation detail, keeps the phone tool context small and requires no n8n credential on the phone.

## Shortcut mapping
- "route this request" -> request_router
- "research this decision" -> research_decision
- "turn this idea into an offer/funnel" -> idea_offer_funnel
- "make outreach for this opportunity" -> opportunity_outreach
- "build an app" -> app_builder
- "build this outcome" -> outcome_foundry
- "make/render an image" -> creative_generate
- "turn this config into content" -> content_hype
- "run marketplace factory" -> marketplace_factory
- "assess this grant portfolio" -> grant_assess

Pass the user's supplied data as the shortcut payload. Never invent missing business facts.

## Direct n8n MCP
Use the separate n8n MCP server only for advanced workflow discovery, building, editing, testing, agent management or execution outside the curated shortcuts.
For direct n8n use: search first, inspect execution detail before first run, and verify the resulting execution.

Do not expose maintenance, backup or watchdog workflows as normal mobile shortcuts.
