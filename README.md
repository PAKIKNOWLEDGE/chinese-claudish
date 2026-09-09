# chinese-claudish

**人话 → 中文黑话**：把大白话改写成 Claude / Claude Code 在中文语境下的特征文风——
修辞打磨、对比密集、结构隐喻、流程术语，带体制腔与竞技腔，四字格压缩，中英混排。

> 恶搞项目，与 Anthropic 无关。灵感来自
> [programasweights/claudish](https://github.com/programasweights/claudish) 与
> [gvzdv/claudish-to-english](https://github.com/gvzdv/claudish-to-english)。

黑话长这样：

> 人话：*发布要先通过全部自动化测试，然后由负责人批准后才能上线。*
>
> 黑话：**发布走双闸：测试门禁先绿，负责人拍板才放行。**

## 用法一：网页翻译器（给不会配的人）

打开 `index.html` 即用。右上角 ⚙ 填入你自己的 OpenAI 兼容端点（OpenAI / DeepSeek /
通义 / 智谱 / vLLM…），左栏打人话，右栏出黑话。浏览器直连云端模型，密钥只存本地
localStorage，不经过任何服务器。

- 「测试连接」按钮：先打 `GET /models`（零 token）验证 URL + Key，端点不支持就自动
  降级为一次 `max_tokens=1` 的最小对话。
- 高级面板可调采样参数和系统提示词，翻译质量主要靠提示词，改它就够了。

## 用法二：Agent 风格注入（让模型直接"学会"说黑话）

把 [`AGENTS.md`](AGENTS.md) 拷进某个项目根目录——Codex、Claude Code、Zed 都读这份
文件，模型每轮加载上下文，开口自动变黑话。想全局生效放 `~/.codex/AGENTS.md`。

## 语义层（这是本仓库的核心资产）

「黑话」不是随机堆词，是对真实语料的蒸馏。完整规格见
[`specs/claudish-zh-spec.md`](specs/claudish-zh-spec.md)：七类技法、六类特征词表、
三大独有装置（四字格压缩 / 体制竞技腔 / 中英混排）、与英文词典的映射表、以及语料
证实的陷阱清单（怀疑不得升级为断言、语义范围不得扩大等）。

- `prompt.js` — 蒸馏结果编译成的 system prompt（网页默认用它）
- `AGENTS.md` — 同一语义层编译成的 agent 常驻风格指令
- `dictionary/` — 英文原版词典与 schema（字段契约），供中文词典建档沿用

## 语料

`corpus/` 四份真实样本：长程任务中的黑话原稿、黑话现象观察（元语料）、CLAUDE.md
diff（含「出局 → 排除」的纠偏样本）、交付汇报腔样本。索引见
[`corpus/README.md`](corpus/README.md)。

## 目录

```
├── index.html       # 谷歌翻译式单页：人话 → 黑话
├── prompt.js        # 编译好的 system prompt（网页默认）
├── AGENTS.md        # agent 常驻风格指令（拷进项目即生效）
├── specs/           # 语义层规格：claudish-zh-spec + 英文原版两份 spec
├── corpus/          # 蒸馏用真实语料
├── dictionary/      # 英文原版 Claudish 词典（entries.json + 校验器）
└── NOTE.txt         # 素材来源与中文改造清单
```

MIT License。