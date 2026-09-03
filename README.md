<div align="center">

# Writer Nuwa · 作家写作系统蒸馏器

<p align="center">
  <img src="assets/hero.gif" alt="nuwa-skill Hero Animation" />
  <br/>
  <sub>动画由 <a href="https://github.com/alchaincyf/huashu-design">huashu-design</a> skill 制作</sub>
</p>

> 输入一个作家名字，蒸馏他/她如何写，而不只是写过什么。

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Agent Skills](https://img.shields.io/badge/Agent%20Skills-Standard-green)](https://agentskills.io)
[![skills.sh](https://img.shields.io/badge/skills.sh-Compatible-blue)](https://skills.sh)
[![Multi-Runtime](https://img.shields.io/badge/Runtime-Claude%20Code%20·%20Codex%20·%20Cursor%20·%20OpenClaw%20·%20Hermes-blueviolet)](#安装)

<br>

**Writer Nuwa 将作家的作品、写作谈与批评材料，转化为可分析、可验证、可执行的写作系统。**

Writer Nuwa 基于 NUWA-Skill 的人物蒸馏方法，
## Writer Nuwa 提炼什么

Writer Nuwa 从作品语料中提炼写作系统，而不是人物观点或角色扮演：

| 系统层 | 内容 |
|---|---|
| **Writing Models** | 可复现的文本组织机制 |
| **Writing Heuristics** | 按情境触发的写作与修改规则 |
| **Linguistic DNA** | 词汇、句法、节奏、标点、修辞与语用 |
| **Narrative DNA** | 视角、距离、信息控制、时间、场景与结构 |
| **Imagery System** | 意象、空间、身体、感官与主题语义场 |
| **Emotional Mechanics** | 情绪如何由文本操作生成 |
| **Anti-patterns** | 不应复制的表面模仿与风格陷阱 |
| **Honest Boundaries** | 语料、体裁、翻译和置信度限制 |

🧪 **Writer Fidelity Scorecard**：使用 [references/fidelity-scorecard.md](references/fidelity-scorecard.md) 进行 100 分制验证，低于 70 分不发布。

```
用户      ❯ OpenAI和Anthropic谁的方向是对的？

乔布斯    ❯ 你问错了。这不是一场关于方向的竞赛。
            这是一场关于品味的竞赛。

            OpenAI像1985年的微软。什么都做，什么都要赢。
            这种策略能赢市场份额。Bill Gates就是这么赢的。
            问题是——当你什么都做的时候，你不可能每件事都做到
            insanely great。

            Anthropic更像早期的Apple。聚焦。
            Focus means saying no to a hundred good ideas.

            ## Writer Nuwa 提炼什么

            Writer Nuwa 从作品语料中提炼写作系统，而不是人物观点或角色扮演：

            | 系统层 | 内容 |
            |---|---|
            | **Writing Models** | 可复现的文本组织机制 |
            | **Writing Heuristics** | 按情境触发的写作与修改规则 |
            | **Linguistic DNA** | 词汇、句法、节奏、标点、修辞与语用 |
            | **Narrative DNA** | 视角、距离、信息控制、时间、场景与结构 |
            | **Imagery System** | 意象、空间、身体、感官与主题语义场 |
            | **Emotional Mechanics** | 情绪如何由文本操作生成 |
            | **Anti-patterns** | 不应复制的表面模仿与风格陷阱 |
            | **Honest Boundaries** | 语料、体裁、翻译和置信度限制 |

            🧪 **Writer Fidelity Scorecard**：使用 [references/fidelity-scorecard.md](references/fidelity-scorecard.md) 进行 100 分制验证，低于 70 分不发布。

```text
蒸馏鲁迅的写作系统

生成一个 Hemingway Writer Skill

分析张爱玲的小说写作机制

创建一个契诃夫短篇小说 Writer Skill
```

## Output

每次蒸馏通常生成：

```text
writer-author/
├── SKILL.md
├── FIDELITY.md
└── references/
  └── research/
    ├── 01-corpus.md
    ├── 02-linguistic-dna.md
    ├── 03-narrative-dna.md
    ├── 04-rhetoric-imagery.md
    ├── 05-poetics-criticism.md
    └── 06-period-contrast.md
```

  ## Writer Nuwa 提炼什么

  Writer Nuwa 从作品语料中提炼写作系统，而不是人物观点或角色扮演：

  | 系统层 | 内容 |
  |---|---|
  | **Writing Models** | 可复现的文本组织机制 |
  | **Writing Heuristics** | 按情境触发的写作与修改规则 |
  | **Linguistic DNA** | 词汇、句法、节奏、标点、修辞与语用 |
  | **Narrative DNA** | 视角、距离、信息控制、时间、场景与结构 |
  | **Imagery System** | 意象、空间、身体、感官与主题语义场 |
  | **Emotional Mechanics** | 情绪如何由文本操作生成 |
  | **Anti-patterns** | 不应复制的表面模仿与风格陷阱 |
  | **Honest Boundaries** | 语料、体裁、翻译和置信度限制 |

  🧪 **Writer Fidelity Scorecard**：使用 [references/fidelity-scorecard.md](references/fidelity-scorecard.md) 进行 100 分制验证，低于 70 分不发布。
### 人物Skill

| 人物 | 领域 | 独立仓库 | 一键安装（跨 runtime） |
|------|------|---------|---------|
| 🔥 **Paul Graham** | 创业/写作/产品/人生哲学 | [paul-graham-skill](https://github.com/alchaincyf/paul-graham-skill) | `npx skills add alchaincyf/paul-graham-skill` |
| 🔥 **张一鸣** | 产品/组织/全球化/人才 | [zhang-yiming-skill](https://github.com/alchaincyf/zhang-yiming-skill) | `npx skills add alchaincyf/zhang-yiming-skill` |
| 🔥 **Karpathy** | AI/工程/教育/开源 | [karpathy-skill](https://github.com/alchaincyf/karpathy-skill) | `npx skills add alchaincyf/karpathy-skill` |
| 🔥 **Ilya Sutskever** | AI安全/scaling/研究品味 | [ilya-sutskever-skill](https://github.com/alchaincyf/ilya-sutskever-skill) | `npx skills add alchaincyf/ilya-sutskever-skill` |
| 🔥 **MrBeast** | 内容创造/YouTube方法论 | [mrbeast-skill](https://github.com/alchaincyf/mrbeast-skill) | `npx skills add alchaincyf/mrbeast-skill` |
| 🔥 **特朗普** | 谈判/权力/传播/行为预判 | [trump-skill](https://github.com/alchaincyf/trump-skill) | `npx skills add alchaincyf/trump-skill` |
| ⭐ **乔布斯** | 产品/设计/战略 | [steve-jobs-skill](https://github.com/alchaincyf/steve-jobs-skill) | `npx skills add alchaincyf/steve-jobs-skill` |
| **马斯克** | 工程/成本/第一性原理 | [elon-musk-skill](https://github.com/alchaincyf/elon-musk-skill) | `npx skills add alchaincyf/elon-musk-skill` |
| **芒格** | 投资/多元思维/逆向思考 | [munger-skill](https://github.com/alchaincyf/munger-skill) | `npx skills add alchaincyf/munger-skill` |
| **费曼** | 学习/教学/科学思维 | [feynman-skill](https://github.com/alchaincyf/feynman-skill) | `npx skills add alchaincyf/feynman-skill` |
| **纳瓦尔** | 财富/杠杆/人生哲学 | [naval-skill](https://github.com/alchaincyf/naval-skill) | `npx skills add alchaincyf/naval-skill` |
| **塔勒布** | 风险/反脆弱/不确定性 | [taleb-skill](https://github.com/alchaincyf/taleb-skill) | `npx skills add alchaincyf/taleb-skill` |
| **张雪峰** | 教育选择/职业规划/阶层流动 | [zhangxuefeng-skill](https://github.com/alchaincyf/zhangxuefeng-skill) | `npx skills add alchaincyf/zhangxuefeng-skill` |
| **孙宇晨** | 营销/注意力经济/叙事操控 | [仓库内examples/](examples/sun-yuchen-perspective/) | 复制 `examples/sun-yuchen-perspective/` 到skills目录 |

### 主题Skill

| 主题 | 领域 | 独立仓库 | 一键安装（跨 runtime） |
|------|------|---------|---------|
| **X导师** | X/Twitter运营全栈 | [x-mentor-skill](https://github.com/alchaincyf/x-mentor-skill) | `npx skills add alchaincyf/x-mentor-skill` |

人物Skill蒸馏一个人的思维方式；主题Skill蒸馏一个领域的方法论。每个仓库都包含完整的调研数据和效果示例对话。

🧪 **保真度评分卡**：15个官方Skill已全部通过独立双agent盲测（立场一致性/风格辨识度/边缘诚实度/来源透明度/结构完整度，方法论见 [references/fidelity-scorecard.md](references/fidelity-scorecard.md)），**全员A级（≥85分）**。各分数：MrBeast/纳瓦尔/塔勒布/乔布斯/Karpathy/Paul Graham/张雪峰 97 · 芒格/费曼/X导师 96 · 特朗普 95 · Ilya 94 · 张一鸣 93 · 孙宇晨 91 · 马斯克 89。完整评分卡见各skill目录内的 `FIDELITY.md`。

想蒸馏不在列表里的人或主题？安装女娲，说「蒸馏一个XXX」就行。

---

## 贡献与社区

女娲的生态由社区一起长大，但走两条不同的路：

- **`SKILL.md` 是核心资产，不接受外部PR改动**。发现方法论的bug或改进点→开issue讨论，被采纳的想法由维护者实现并在commit中致谢（先例见PR #59）
- **社区蒸馏的人物skill走 [COMMUNITY.md](COMMUNITY.md) 索引**：放你自己的仓库（star归你），跑一遍[保真度评分卡](references/fidelity-scorecard.md)拿到B级以上，提一行PR即可收录

完整规则见 [CONTRIBUTING.md](CONTRIBUTING.md)。社区已有的合集、多人格编排和主题应用，见 [COMMUNITY.md](COMMUNITY.md)。

---

## 达尔文.skill：让所有Skill持续进化

<div align="center">

<a href="https://github.com/alchaincyf/darwin-skill">
<img src="https://raw.githubusercontent.com/alchaincyf/darwin-skill/master/assets/banner.svg" alt="达尔文.skill" width="600">
</a>

</div>

女娲造Skill，**[达尔文](https://github.com/alchaincyf/darwin-skill)** 让Skill进化。

受 Karpathy autoresearch 启发，达尔文.skill 用自主实验循环批量优化所有Skill：8维度评估、棘轮机制（只保留改进，自动回滚退步）、独立子agent评分。女娲的 Phase 5 双Agent精炼就内置了达尔文的评估体系，这也是女娲生成的Skill质量高的原因之一。

```bash
npx skills add alchaincyf/darwin-skill
```

---

## How It Works

Writer Nuwa 将作家的写作特征从语料中提取出来，经过规则化、构建和验证，最终生成可运行的 Writer Skill：

```text
Author + Scope
  ↓
Corpus Building
  ↓
6 Parallel Writer Research Agents
  ↓
Writing Models
Writing Heuristics
Linguistic DNA
Narrative DNA
Imagery System
  ↓
Writer SKILL.md
  ↓
Fidelity Validation
  ↓
Dual Reviewer Refinement
```

### Phase 1: Corpus and Writer Research

确认作者与分析范围，建立作品语料库，并由 6 个并行 Writer Research Agent 分析作品、写作时期、语言、叙事、意象和文学批评材料。

### Phase 2: Writing Feature Extraction

把文本观察转换为可验证、可执行的写作系统，包括 `Writing Models`、`Writing Heuristics`、`Linguistic DNA`、`Narrative DNA`、`Imagery System` 和 `Anti-patterns`。任何“很克制”“很冷峻”之类的文学形容，都必须经过 Observation → Evidence → Mechanism → Trigger → Operation → Failure Condition 的转换，不能直接入库。

核心提炼链：

```text
作品证据
→ Writing Models
→ Writing Heuristics
→ Linguistic DNA
→ Narrative DNA
→ Imagery System
```

### Phase 3: Writer Skill Construction

将提炼结果组装为 Writer `SKILL.md`，包含写作哲学、写作模型、启发式规则、语言与叙事 DNA、意象系统、情绪机制、反模仿边界、写作协议和诚实边界。

### Phase 4: Fidelity Validation

通过已知段落重构、未知题材、风格消融、反漫画化、对照、模仿、识别和应用测试，检查 Skill 学到的是写作机制，而不是原作的表面词汇或固定意象。

### Phase 5: Dual Reviewer Refinement

由两个独立 Reviewer 复核：`Literary Fidelity Critic` 判断“这是真的吗”，`Generative Writing Engineer` 判断“这能运行吗”。只有证据真实且规则可执行，才进入最终交付。

### 五阶段概览

#### Phase 1 — Research

六个 Agent：

1. `Corpus Analyst`
2. `Linguistic Analyst`
3. `Narratology Analyst`
4. `Rhetoric & Imagery Analyst`
5. `Poetics & Criticism Analyst`
6. `Period & Contrast Analyst`

#### Phase 2 — Distillation

生成：

- 3–7 个 `Writing Models`
- `Writing Heuristics`
- `Linguistic DNA`
- `Narrative DNA`
- `Imagery System`
- `Anti-patterns`
- `Boundaries`

#### Phase 3 — Skill Assembly

生成最终 Writer `SKILL.md`。

#### Phase 4 — Fidelity Validation

使用 `reconstruction`、`unseen topic`、`ablation`、`anti-caricature`、`contrast` 测试。

#### Phase 5 — Refinement

两个独立 Reviewer：

- `Literary Fidelity Critic`
- `Generative Writing Engineer`

完整方法论在 `references/writer-extraction-framework.md`。

---

## 仓库结构

```
writer-nuwa-skill/
├── SKILL.md                      # Writer Nuwa 机器执行规范
├── references/
│   ├── extraction-framework.md   # Writer 提炼方法论
│   ├── fidelity-scorecard.md     # Writer 保真评分卡
│   └── writer-skill-template.md  # Writer Skill 模板
├── examples/                     # Writer Skill 示例规范
│   └── README.md
└── examples-legacy/              # 旧人物 Skill，仅供历史参考
```

调研过程全透明。每个 example 都包含完整的研究文件，你可以看到作品语料如何被收集、筛选，并转换为可执行的写作规则。

---

## 背后的故事

Writer Nuwa 延续 NUWA-Skill 的研究与验证方法，但将分析对象从人物的公开观点转为作家的作品语料、写作时期、批评材料与创作机制。

这里的目标不是生成一个“像作者”的声音，而是把作者如何组织文本、调度语言、控制信息和使用意象，转换为可验证、可迁移的 Writer Skill。

---

## 关于作者

**花叔 Huashu** — AI Native Coder，独立开发者，代表作：小猫补光灯（AppStore 付费榜 Top1）

| 平台 | 链接 |
|------|------|
| 🌐 官网 | [bookai.top](https://bookai.top) · [huasheng.ai](https://www.huasheng.ai) |
| 𝕏 Twitter | [@AlchainHust](https://x.com/AlchainHust) |
| 📺 B站 | [花叔](https://space.bilibili.com/14097567) |
| ▶️ YouTube | [@Alchain](https://www.youtube.com/@Alchain) |
| 📕 小红书 | [花叔](https://www.xiaohongshu.com/user/profile/5abc6f17e8ac2b109179dfdf) |
| 💬 公众号 | 微信搜「花叔」或扫码关注 ↓ |

<img src="wechat-qrcode.jpg" alt="公众号二维码" width="360">

## Credits

Writer Nuwa is a derivative project based on
[NUWA-Skill](https://github.com/alchaincyf/nuwa-skill).

Original NUWA methodology:
Huashu / alchaincyf.

This fork adapts cognitive distillation into
writer-system distillation.

## 许可证

MIT — 随便用，随便改，随便造。

---

<div align="center">

**Writer Nuwa** 蒸馏作家如何写。<br><br>
*HOW THEY WRITE, not WHAT THEY WROTE.*

<br>

MIT License © [花叔 Huashu](https://github.com/alchaincyf)

</div>

---

<div align="center">
<sub>作者的其他项目 · also by 花叔</sub>

[![FanBox · Coding Agent 的驾驶舱](https://raw.githubusercontent.com/alchaincyf/fanbox/master/assets/promo-banner.jpg)](https://github.com/alchaincyf/fanbox)

</div>

---

## English

> *"Learn how a writer writes, not just what they wrote."*

**Writer Nuwa** is a derivative project based on [NUWA-Skill](https://github.com/alchaincyf/nuwa-skill). It adapts cognitive distillation into writer-system distillation: extracting how an author organizes language, narrative, imagery, and revision decisions.

Writer Nuwa is an [Agent Skill](https://agentskills.io) that turns an author's corpus into a runnable Writer `SKILL.md`. It works in Claude Code, Codex, Cursor, OpenClaw, Hermes Agent, CodeBuddy, Workbuddy, Gemini CLI, OpenCode, and 50+ skills-compatible runtimes.

It extracts:

- Writing Models
- Writing Heuristics
- Linguistic DNA
- Narrative DNA
- Imagery System
- Emotional Mechanics
- Anti-patterns
- Honest Boundaries

**How it works**: Author + scope → corpus building → 6 parallel Writer Research Agents → writing-system distillation → Writer `SKILL.md` → fidelity validation → dual reviewer refinement.

The system prioritizes high-level mechanisms over direct quotation or surface imitation. For living authors, use it primarily for style analysis, writing education, and non-high-fidelity creative guidance. For translated literature, distinguish the author's original-language features from the translator's language features.

**Install** (cross-runtime, auto-detects your agent): `npx skills add overwegfernandz80-hub/writer-nuwa-skill`

See the Chinese README above for live examples and methodology.
