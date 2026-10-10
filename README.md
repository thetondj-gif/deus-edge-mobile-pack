# Deus Edge Mobile Pack v2

A compact mobile control plane for Google AI Edge Gallery Agent Chat.

## Core design

- **3 skills only**: Founder Command, DeusIntus.com, DeusIntus.co.uk.
- **1 MCP tool only**: `deus_mobile_command`.
- Long-tail workflows, specialists and estate access remain behind that one tool.
- Use **Gemma-4-E2B-it** on 8 GB devices.
- Keep the Agent Chat prompt short; use `AGENT-CHAT-SYSTEM-PROMPT.txt`.

## Install skills

Load these skill files from **Agent Skills → + → Load skill from URL**:

`https://raw.githubusercontent.com/thetondj-gif/deus-edge-mobile-pack/main/skills/deus-founder-command/SKILL.md`

`https://raw.githubusercontent.com/thetondj-gif/deus-edge-mobile-pack/main/skills/deus-brand-com/SKILL.md`

`https://raw.githubusercontent.com/thetondj-gif/deus-edge-mobile-pack/main/skills/deus-brand-co-uk/SKILL.md`

## MCP configuration

This public pack does not include a private MCP endpoint.

Configure your own `deus_mobile_command` MCP endpoint privately in Google AI Edge Gallery. Do not share personal Tailnet, localhost, or internal-network URLs in a public repository.

Do not keep the old six Deus helper skills enabled alongside v2; their jobs are now folded into Founder Command.

## Troubleshooting

If a GitHub Pages skill URL does not load, use the raw GitHub URLs above. They read directly from the `main` branch and do not depend on the Pages deployment.