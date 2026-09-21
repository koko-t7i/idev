# mou

把模糊的想法谈成明确的需求和实施计划。

## 它会做什么

- 维护一份清单，记着哪些已定、哪些待定、哪些不做，每轮只贴新增的；
- 把五件事问完：目标与动机、范围、边界条件、验收标准、约束；
- 把"快""好用"换成能验收的标准；
- 需求谈拢后先读你的代码，再定这功能写在哪、怎么接进去；
- 写出需求文档和实施计划。

## 怎么用

```text
/mou 我想给项目加一个插件系统
$mou 按 docs/plugin-research.md 的调研结果，聊聊插件系统要做成什么样
```

## 流程

1. **谈需求** — 这个阶段不定技术方案，把五件事谈到边界和验收标准都清楚；
2. **确认** — mou 把整份清单重贴一遍，你点头后进下一步；
3. **谈实施计划** — 先读项目代码，再敲定这功能新开模块还是加在现有模块上、数据
   怎么存、对外什么接口、动哪些文件、分几步做、出问题怎么退；
4. **写文档** — 你同意后写出两份文件。

## 产出

默认写到 `/tmp/mou/<slug>/`，也可以指定路径：

- `requirements.md` — 需求文档；
- `plan.md` — 实施计划。

## 安装

```bash
ln -s /path/to/mou ~/.grok/skills/mou      # Grok
ln -s /path/to/mou ~/.claude/skills/mou    # Claude Code
ln -s /path/to/mou ~/.codex/skills/mou     # Codex
```

装完重启会话。

## 目录结构

```text
mou/
├── SKILL.md
├── README.md
├── references/
│   ├── dialogue-playbook.md      # 对话手法
│   ├── requirements-template.md  # 需求文档模板
│   └── plan-template.md          # 实施计划模板
└── agents/
    └── openai.yaml
```

## License

MIT
