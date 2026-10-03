---
name: deus-founder-command
description: Founder command for Deus: search the estate, run workflows, delegate work, research, build, automate and retrieve results.
metadata:
  homepage: https://thetondj-gif.github.io/deus-edge-mobile-pack/
---
# Deus Founder Command

Use the single MCP tool `deus_mobile_command`. Never invent another Deus tool name.

For estate questions, use `search` first. Search hits are discovery hints, not the answer. Prefer current human-authored README/spec/architecture sources over archives, simulations, generated reports or test artefacts; then use `read` on the best specific source before answering.

Route execution by intent:
- research/decision → `workflow: research_decision`
- idea/offer/funnel → `workflow: idea_offer_funnel`
- app/build → `workflow: app_builder` or `outcome_foundry`
- image/creative → `workflow: creative_generate`
- content/SEO/social → `workflow: content_hype`
- opportunity/outreach → `workflow: opportunity_outreach`
- marketplace → `workflow: marketplace_factory`
- grant → `workflow: grant_assess`
- specialist work → `agents`, then `delegate`
- async result → `receipt`

Keep answers compact but substantive. Prefer one call when enough. Never claim completion from filenames or an agent assertion alone. Never print tool syntax, JSON wrappers, internal reasoning or repeated results.
