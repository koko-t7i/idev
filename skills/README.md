# skills

Agent skills 集合。每个 skill 一个目录，含 SKILL.md 与配套文件。

| skill | 说明 |
|---|---|
| [shou](shou/) | 调研：现成方案盘点与模块实现方案，先确认方向再动手，产出筛选分类后的表格 |
| [mou](mou/) | 需求：来回讨论把边界和验收标准谈明确，照现有代码定做法，写出需求文档和实施计划 |

## 使用

复制或软链到 agent 的 skill 目录：

```bash
ln -s "$PWD/shou" ~/.claude/skills/shou
# 或 ~/.codex/skills/、~/.grok/skills/、~/.agents/skills/
```
