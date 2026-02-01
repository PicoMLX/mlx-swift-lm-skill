# MLX-Swift-LM Skill

This repo packages a skill for agentic coding tools (Claude Code, Codex, Droid, etc.) to help with the MLX-Swift-LM library. The skill provides usage guidance, best practices, and reference notes for local LLM/VLM inference on Apple Silicon.

Source library: https://github.com/ml-explore/mlx-swift-lm/

## What this skill covers
- Local LLM and VLM inference with MLX-Swift-LM
- Streaming generation and tool calling
- LoRA and adapter training flows
- Embeddings and RAG-friendly patterns
- Concurrency, cache, and tokenizer usage

## Repo layout
```
mlx-swift-lm/skill.md          # Skill definition, triggers, and overview
mlx-swift-lm/references/       # Topic-specific deep dives
README.md                      # This file
LICENSE
```

References included:
- `references/model-container.md`
- `references/kv-cache.md`
- `references/tokenizer-chat.md`
- `references/concurrency.md`
- `references/tool-calling.md`
- `references/supported-models.md`
- `references/lora-adapters.md`
- `references/training.md`
- `references/embeddings.md`

## Install (generic)
1. Copy or symlink the `mlx-swift-lm` folder into your tool's skills directory.
2. Restart or refresh your tool so it discovers the new skill.

Common locations:
- Codex CLI: `$CODEX_HOME/skills` (default: `~/.codex/skills`)
- Claude Code: default `~/.claude/skills`
- Droid: default `~/.factory/skills`

## Use the skill
Skill name: `swift-mlx-lm`

You can invoke it directly, or rely on triggers like:
`mlx`, `mlx-swift`, `mlx-lm`, `apple silicon llm`, `local llm swift`, `vision language model swift`, `lora training swift`

Example prompts:
- "Use the swift-mlx-lm skill to add streaming generation to my Swift app."
- "With the MLX-Swift-LM skill, show how to run Qwen2-VL with an image."
- "Use swift-mlx-lm to explain LoRA adapter loading for MLX-Swift-LM."

## Update
Pull the repo and re-sync the `mlx-swift-lm` folder in your skills directory.

## Contributing
Edit `mlx-swift-lm/skill.md` for the main skill instructions and add new topic docs under `mlx-swift-lm/references/`.
