# chinese-claudish（中文黑话）

> **English（Claudish 版）** | **中文（黑话版）**

## 整体形状

这仓库交付的是一个没人要、但已经落地的转换：**人话进 → Claude 腔中文出**。不是翻译，是重构，而且是刻意的重构。管线契约硬得像铁，不弯：事实、数字、路径、日期逐字幸存，被升级的只有修辞。输出像模型自然说出的黑话——绝不是往人话上焊词。恶搞项目。与 Anthropic 无关。

## 两条表面，一根脊柱

**语义层是脊柱**，其余全是挂在脊柱上的薄适配器。脊柱已终审：蒸馏自 `corpus/` 四份真实语料，全协议落在 `specs/claudish-zh-spec.md`——七类技法、六类词表、三大独有装置（四字格压缩 / 体制竞技腔 / 中英混排）、以及陷阱台账（怀疑不得升级为裁决、语义范围不得扩大）。陷阱台账是承重的，这句话本身也是承重的。

### 表面一：网页翻译器（给不会配的）

打开 `index.html`，它就已经就位。右上角齿轮是门禁：填任意 OpenAI 兼容端点（OpenAI / DeepSeek / 通义 / 智谱 / vLLM…），密钥驻留它该待的地方——本浏览器 localStorage，路径上零服务器。**测试连接**先打 `/models`（零 token），端点没实现才降级为一次 token 最小对话。高级面板：temperature、max tokens、**关思考开关**（`reasoning_effort: none`——推理模型不然先烧半天钟才开口）、以及可编辑的原生 system prompt——prompt 即产品。

### 表面二：Agent 风格注入（给机器）

把 [`AGENTS.md`](AGENTS.md) 丢进任意项目根目录。Codex、Claude Code、Zed 全认这份文件；模型每轮加载，黑话成为默认嗓音。全局安装：`~/.codex/AGENTS.md`。零安装、零配置、一触即染。

## 台账

```
index.html      网页翻译器（双栏，谷歌翻译形状）
prompt.js       编译好的 system prompt（脊柱的可操作形态）
AGENTS.md       agent 常驻风格指令
specs/          蒸馏全文 + 英文原版 spec
corpus/         四份真实语料 + 索引
dictionary/     英文原版 Claudish 词典（entries.json + 校验器）
README.md       English · the dialect's export model
```

## 来路

脊柱不是发明词，是蒸馏自真实长程会话的沉淀：拉链句签名句式（"137 项 spine 落地 + 3 死门归零 + 全套绿"）、体制腔（拍板 / 终审 / 归户）、竞技腔（正赛 / 出局 / 哑火）、以及一份被人类纠偏的标本（"出局"被改回"排除"）——证据链在语料里，与上游词典交叉引用。致敬落位：[programasweights/claudish](https://github.com/programasweights/claudish) 与 [gvzdv/claudish-to-english](https://github.com/gvzdv/claudish-to-english)。

MIT License。