---
name: deus-n8n-shortcuts
description: Voice-friendly shortcuts to the founder's useful n8n workflows. Use for apps, funnels, research, outreach, content, creative, marketplace, grants and automation.
metadata:
  homepage: https://thetondj-gif.github.io/deus-edge-mobile-pack/
---
# Deus n8n Shortcuts

Use the connected n8n MCP server for workflow discovery and execution.

## Rule
Call `search_workflows` first when the workflow state is uncertain. Check `availableInMCP`.
Use `get_workflow_details` with detailLevel=execution before first execution to learn trigger name/input shape.
Use `execute_workflow` in production mode for published workflows; pass the exact webhook trigger name and body for webhook workflows.
After starting, use execution-status tooling when the result matters.

## Founder shortcuts
- "build an app" -> deusOutcomeFoundryBuild01 or deusAppBuilder01
- "make/render an image" -> deusCreativeRouter01
- "turn this config into content" -> deusConfigContentHype01
- "research this decision" -> deusPersonalResearchDecisionBrief01
- "turn this idea into an offer/funnel" -> deusPersonalIdeaOfferFunnel01
- "make outreach for this opportunity" -> deusPersonalOpportunityOutreachPack01
- "run marketplace factory" -> deusMarketplaceFactory01
- "commission YouTube from signals" -> deusYouTubeSignalCommissioning01
- "scan Reddit leads" -> deusRedditIntel01
- "assess this grant portfolio" -> deusGrantPortfolioAssess01

Do not expose maintenance/watchdog/backup workflows as normal user shortcuts.
If direct execution is unavailable, route the job through the Founder MCP to the automation specialist rather than pretending it ran.
