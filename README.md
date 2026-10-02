# Deus Edge Mobile Pack

A mobile-first founder/brand operating pack for Google AI Edge Gallery.

## What this does

The local on-device model stays the conversational front end. Skills load only when relevant. Heavy work routes through the private Deus Founder MCP, Agent DM specialists, or the existing n8n estate.

This keeps the phone's tool context small while exposing a much larger capability estate behind a few deliberate interfaces.

## Pack

- **deus-founder-command** — estate search, project context and specialist delegation.
- **deus-brand-com** — dedicated deusintus.com consumer brand director.
- **deus-brand-co-uk** — dedicated deusintus.co.uk / UK-market operator.
- **deus-n8n-shortcuts** — voice-friendly access to the useful founder workflows.
- **deus-google-workspace** — Calendar/Gmail native-first, deeper Workspace automation through Deus.
- **deus-research-intel** — internal + live research and evidence.
- **deus-build-launch** — app/site/funnel/MVP execution.
- **deus-content-engine** — content/SEO/social/YouTube from real evidence.
- **deus-opportunity-revenue** — leads, grants, tenders, outreach and marketplace signals.

## Install on AI Edge Gallery

Open **Agent Skills → + → Load skill from URL** and use a skill folder URL such as:

`https://thetondj-gif.github.io/deus-edge-mobile-pack/skills/deus-founder-command`

Repeat only for the skills you actually want active. Google AI Edge Gallery has a tight mobile context window; a focused pack is more reliable than hundreds of visible tools.

## Agent Chat compatibility

Use **Gemma-4-E2B-it** or **Gemma-4-E4B-it** for Agent Chat. On an 8 GB device use E2B. Do not assume an imported/custom model is tool-call compatible merely because Gallery lets it appear under Agent Chat. Keep Gallery's default Agent Chat system prompt. See `AI-EDGE-COMPATIBILITY.md`.

## MCP

Use the private Founder MCP as the main tool plane. Add n8n MCP only when you want direct workflow building/execution from the phone, and disable unneeded n8n tools per session.

No credentials are stored in this repository.

## Design principles

- local inference first
- skills for intent/routing
- MCP for live tools/actions
- n8n for deterministic workflows
- specialists for deep work
- verify outputs, don't trust completion assertions
- reuse existing capabilities before building new ones
