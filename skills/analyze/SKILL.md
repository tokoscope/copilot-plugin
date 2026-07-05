# Analyze Prompt

Analyze a prompt or file for token count, estimated cost, and waste score.

## Usage

Ask Copilot to analyze any prompt or file:

```
Analyze this prompt for token usage: [paste your prompt]
```

```
How many tokens is this system prompt?
```

```
What's the waste score for this file?
```

## What you get

- **Token count** — estimated tokens using GPT tokenizer heuristics
- **Cost estimate** — per-call cost across gpt-4o, gpt-4o-mini, claude-sonnet, gemini-flash
- **Waste score** — 0-100 score flagging redundant instructions, filler phrases, and bloat
- **Compressed version** — minimum effective form of the prompt if waste score > 30%
- **Suggestions** — specific lines or phrases to cut or rewrite

## Examples

**Input:**
> Please note that it is very important that you make sure to respond to my question clearly and helpfully. As an AI, I need you to understand that what I am asking is: What is the capital of France?

**Output:**
- Tokens: ~47
- Cost on gpt-4o-mini: $0.000007
- Waste score: 78/100
- Compressed: "What is the capital of France?" (7 tokens, 85% reduction)

## Links

- Dashboard: https://app.tokoscope.com
- Docs: https://tokoscope.com/docs
- Install SDK: npm install tokoscope
