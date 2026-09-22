# skills

Agent skills 集合。每个 skill 一个目录，含 SKILL.md 与配套文件。

| skill | 说明 |
|---|---|
| [talk](talk/) | 先聊清楚，必要时查清楚，最后收敛成能接着规划或实现的结论 |

## 使用

软链到共用的 skill 目录：

```bash
ln -s "$PWD/talk" ~/.agents/skills/talk
```

内容只留仓库这一份，链接指过去，改仓库即生效。客户端只读自己目录时，照同样方式再加一条软链。
