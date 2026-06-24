# AIPath RED Skill

一个用于判断 AI 转型路径的 RED Skill。

**AIPath** 不是简历模板，也不是求职承诺。它会根据你的背景、目标岗位/JD、项目或工作流证据，帮你判断：

- 你更适合哪类 AI 方向。
- 目标岗位真正看哪些信号。
- 你现在缺的是关键词，还是可被追问的证据。
- 你的项目或工作流下一步该补什么。
- 哪些经历可以诚实地写，哪些还不能 claim。

## Who It Is For

这个 Skill 不只适合 SDE。

适合这些人先做一次诊断：

- SDE / Backend / Data Engineer: 判断是否适合 AI Engineer、Applied AI Engineer、FDE。
- Product / Ops / Analyst / Consultant: 判断是否适合 AI PM、AI Ops、automation builder、AI workflow owner。
- Students / career switchers: 找到更现实的 first proof artifact，而不是直接硬冲很重的 JD。

## How To Use

### 小红书用户最快使用方式

1. 打开 [`SKILL.md`](./SKILL.md)。
2. 复制全部内容。
3. 粘贴到 Claude Code / OpenClaw 这类 Agent。
4. 再粘贴这句话：

```text
请使用 AIPath 帮我做一次 AI 转型路径诊断。先按模板向我收集信息；如果信息不完整，也请基于假设继续，并标清楚假设。
```

5. 按 [`中文输入模板`](./templates/input_template_zh.md) 填你的背景、目标岗位/JD、项目或工作流。

如果你只想先快速看方向，可以加一句：

```text
先给我 short diagnosis，不要超过 500 字；如果我觉得有用，再展开完整报告。
```

### General Usage

把 [`SKILL.md`](./SKILL.md) 复制到支持 Skill / Agent workflow 的工具中使用，例如 Claude Code 或 OpenClaw。

如果你的工具支持安装 Skill，可以把这个目录作为 Skill source。  
如果你的工具暂时不支持安装，直接复制 `SKILL.md` 的内容给 Agent，然后输入：

```text
Use this Skill to diagnose my AI transition fit. Ask me for the required input first.
```

然后按模板填写：

```text
1. Target role or JD:
2. Current background summary:
3. Work experience or workflow examples:
4. Project descriptions or AI workflow ideas:
5. Current AI/LLM stack:
6. Deployment or production evidence:
7. Evaluation or metrics evidence:
8. Target company type:
9. Timeline:
10. Biggest concern:
```

## Output

Skill 会按这个结构输出：

1. Fit Snapshot
2. Role Direction
3. JD Signal Map
4. Evidence Gaps
5. Positioning Rewrites
6. Project Or Workflow Upgrade Suggestions
7. Interview Question Set
8. Seven-Day Action Plan
9. Honest Positioning
10. Xiaohongshu-Friendly Summary

## Sample

- [Sample input](./sample_inputs/sde_to_ai_engineer.json)
- [Sample output](./sample_outputs/sde_to_ai_engineer_output.md)
- [中文输入模板](./templates/input_template_zh.md)
- [中文启动提示词](./templates/starter_prompt_zh.md)

## Xiaohongshu

小红书备用文案：

- [Post body](./xiaohongshu/post_body.txt)
- [First comment](./xiaohongshu/first_comment.txt)

如果小红书 RED Skill 组件无法挂载，可以先在评论区放这个 GitHub 链接作为 fallback。
