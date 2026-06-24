# AIPath 中文启动提示词

如果你的工具不能直接安装 Skill，就先复制 `SKILL.md` 的全部内容给 Agent，然后再粘贴下面这段：

```text
请使用刚才的 AIPath Skill 帮我做一次 AI 转型路径诊断。

请先问我要以下信息：
1. 目标岗位或 JD
2. 当前背景
3. 工作经历或 workflow 例子
4. 项目描述或 AI workflow 想法
5. 当前 AI/LLM stack
6. 部署或 production 证据
7. 评估或指标证据
8. 目标公司类型
9. 时间线
10. 最大担心点

如果我信息不完整，也请继续诊断，但要标清楚你的假设。
先输出 short diagnosis，不超过 500 字；如果我需要，再展开完整报告。
```

如果你已经有 JD 和背景，可以直接用 [`input_template_zh.md`](./input_template_zh.md)。
