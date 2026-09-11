# chinese-claudish

> **English** | [中文（黑话版）](README.zh.md)

## The honest shape

This repository ships the load-bearing conversion nobody asked for: **plain prose in, Claude-flavoured Chinese dialect out**. Not a translation — a reframing, and a deliberate one. The pipeline is gated on a contract that does not bend: every fact, number, file path, and date survives the rewrite untouched; only the rhetoric gets the upgrade. Output reads as though the model *naturally* chose the phrasing — never as though vocabulary was welded onto otherwise unchanged prose. Parody project. Not affiliated with Anthropic.

## Two surfaces, one spine

The **semantic layer is the spine**; everything else is a thin adapter bolted onto it. The spine is fully audited: distilled from four real specimens in `corpus/`, and documented end-to-end in `specs/claudish-zh-spec.md` — the seven technique families, the six vocabulary registries, the three uniquely-Chinese devices (four-character compression, the bureaucratic-athletic register, zh-en code mixing), and the trap ledger (a suspicion must never land as a verdict; a scope must never widen). The trap ledger is load-bearing, in case that wasn't clear.

### Surface 1: the web translator (for the non-technical)

Open `index.html` and it just works. The gear in the corner is the gate: drop in any OpenAI-compatible endpoint (OpenAI / DeepSeek / Qwen / Zhipu / vLLM…), and the key stays where it belongs — localStorage, this browser, no server in the path. A **test-connection guard** probes `/models` first (zero tokens spent), and degrades to a one-token chat only when the endpoint lacks the endpoint. The advanced panel holds temperature, max tokens, a **kill-the-thinking switch** (`reasoning_effort: none` — reasoning-tier models otherwise burn the clock before answering), and the raw system prompt itself, editable, because the prompt *is* the product.

### Surface 2: agent style injection (for the machines)

Drop [`AGENTS.md`](AGENTS.md) into any project root. Codex, Claude Code, and Zed all read this file; the model loads it every turn and the dialect becomes its default voice. Global instal: `~/.codex/AGENTS.md`. Zero install, zero setup, dialect on contact.

## The ledger

```
index.html       web translator (two-pane, Google-Translate-shaped)
prompt.js        compiled system prompt (the operative form of the spine)
AGENTS.md        resident style directive for agents
specs/           the full distillation + upstream specs
corpus/          four real specimens + index
dictionary/      upstream Claudish lexicon (entries.json + validator)
README.zh.md     中文黑话版 · the dialect's mother tongue
```

## Provenance

The spine is not invented vocabulary — it's distilled from real long-horizon sessions. The tally-chain sentence ("137 项 spine 落地 + 3 死门归零 + 全套绿"), the bureaucracy register (拍板 / 终审 / 归户), the athletics register (正赛 / 出局 / 哑火), and a documented correction specimen where a human degarbled "出局" back to "排除" — the evidence chain is in the corpus, cross-referenced against the upstream lexicon. Credit where credit lands: [programasweights/claudish](https://github.com/programasweights/claudish) and [gvzdv/claudish-to-english](https://github.com/gvzdv/claudish-to-english).

MIT License.