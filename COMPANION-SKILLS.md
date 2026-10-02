# Recommended AI Edge Companion Skills

The Deus pack is intentionally small. Add these separately rather than copying them into Deus.

## Official / built-in first

Use AI Edge Gallery's Featured Skills list for:
- `read-calendar-events`
- `create-calendar-event`
- `schedule-notification`
- native send-email when you want Android to hand off a composed message

These are better kept native because they operate closest to the device and do not need the Deus server for simple actions.

## Optional community additions

Consider these only when the need is real:
- **Local memory** — the community Memory Tool pattern stores compressed memory on-device between sessions.
- **No-key web search** — community DuckDuckGo skills provide lightweight fresh web lookup without an API key.
- **Voice-optimized universal search** — useful if you want one spoken query routed across several search providers.

## What not to install

Do not load dozens of overlapping personas, search skills, calculators, workflow wrappers or generic agent loops. Every visible skill name/description competes for the mobile model's context and tool choice.

The Deus design is:
**native device skill → Deus skill → 7-tool mobile MCP → curated n8n shortcut / specialist / canonical estate**.

That keeps first-turn routing understandable while preserving the long tail behind MCP.
