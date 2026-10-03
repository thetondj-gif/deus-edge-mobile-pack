# AI Edge Agent Chat compatibility

## Required model for tools

Use **Gemma-4-E2B-it** or **Gemma-4-E4B-it** in Google AI Edge Gallery Agent Chat.

For an 8 GB Android device, use **Gemma-4-E2B-it**.

Do **not** use Qwen2.5, DeepSeek-Qwen, or another imported/custom model for the Deus MCP Agent Chat route unless you have independently verified its LiteRT tool-calling format. Google currently lists Qwen2.5 for normal chat and prompt lab, not Agent Chat, while Gemma 4 E2B/E4B are explicitly registered for Agent Chat.

Imported models may still appear in Agent Chat because Gallery currently registers imported LLMs there generically. Visibility in the picker therefore does not prove compatible function calling.

## System prompt

Use the compact prompt in `AGENT-CHAT-SYSTEM-PROMPT.txt`. It preserves Gallery's required placeholders (`___SKILLS___` and `___TOOLS___`) and runtime functions (`load_skill` and `runMcpTool`) while removing unnecessary prompt weight.

Do not use a Qwen/OpenAI/Claude tool-call template. Model-native strings such as `<|tool_call>`, `run_mcp_tool`, Python-style `print(result)`, or raw JSON tool wrappers are a compatibility failure, not a valid MCP result.

## Deus MCP

Use:

`https://anthons-mac-studio.tail8ff43e.ts.net/mobile-mcp`

The mobile profile now exposes **one MCP tool only**: `deus_mobile_command`. It handles search, read, workflows, specialists, receipts and model status behind one schema and caps result size for AI Edge's tighter context.

## Healthy behaviour

A healthy turn looks like:

1. Agent Chat silently selects `runMcpTool` or `load_skill`.
2. Gallery executes the runtime tool.
3. The Deus server audit receives exactly one MCP call.
4. The model receives the tool result.
5. The final answer is normal prose.

If you see repeated `print(result)`, raw `<|tool_call>` tokens, or the server audit shows no call, change the Agent Chat model before changing Deus routing.
