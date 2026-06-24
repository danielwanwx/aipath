---
name: aipath
description: Use when someone wants to find their realistic AI career path, map their current background to AI roles, identify proof gaps, upgrade projects or workflows, and prepare truthful resume/interview positioning.
---

# AIPath

Diagnose how close a person is to an AI-related role based on their background, target role
or JD, and project/workflow evidence.

The target role can be AI Engineer, Applied AI Engineer, FDE, AI PM, AI Ops, AI automation
builder, AI consultant, data/product roles with AI workflows, or another concrete AI-facing
role. This Skill should not force every user into AI Engineer. It should help them understand:

- What evidence they already have.
- What evidence is missing.
- Which AI direction best fits their current background.
- How to rewrite truthfully without overclaiming.
- What project, workflow, or proof artifact to build next.

## When To Use

Use this Skill when the user says things like:

- "帮我看看这份简历能不能投 AI Engineer."
- "我想从 SDE 转 FDE，还差什么？"
- "我不是程序员，也想转 AI 相关岗位，怎么判断方向？"
- "我现在做产品/运营/数据/咨询，怎么把经历转成 AI 工作流证据？"
- "这个 JD 和我的经历匹配吗？"
- "我的 RAG/Agent 项目怎么写进简历？"
- "我有一个 AI 自动化 workflow，怎么变成可展示的项目？"
- "帮我准备这个岗位的面试问题."
- "为什么我投 AI 岗没有面试？"

## Required Input

Ask for missing fields if they are important. If the user only has partial information,
continue with clearly labeled assumptions.

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

## Output Contract

Always produce these sections in order.

### 1. Fit Snapshot

Give a score:

- `Strong fit`
- `Promising but under-evidenced`
- `Needs project proof`
- `Too early for this JD`
- `Better fit for adjacent AI role`

Also give a 0-100 readiness score.

The score should be conservative. A user with tools but no evaluation, deployment, business
workflow, or project evidence should not score high.

If the user is not a strong fit for the requested role, suggest the most realistic adjacent
AI direction instead of forcing a match.

### 2. Role Direction

Map the user to one or two realistic directions, such as:

- AI Engineer / Applied AI Engineer.
- FDE / AI solutions engineer.
- AI PM / AI product strategist.
- AI Ops / automation builder.
- Data analyst / analytics engineer with AI workflow ownership.
- AI content/workflow operator.
- Too early; build a smaller proof artifact first.

Explain why the direction fits or does not fit.

### 3. JD Signal Map

Extract 6-10 signals from the JD or target role. Example signals:

- RAG / retrieval.
- Agent workflows.
- Backend or API systems.
- Evaluation.
- Deployment.
- Data pipelines.
- Product/customer communication.
- Observability.
- Cloud/infrastructure.
- Cross-functional work.
- Workflow ownership.
- Business impact.

For each signal, mark:

- `Covered`
- `Weak`
- `Missing`

### 4. Evidence Gaps

Explain the top gaps that make the candidate less competitive.

Prefer evidence gaps over keyword gaps. Example:

- Not "missing LangChain keyword."
- Better: "No proof that you evaluated output quality or handled failure cases."

### 5. Positioning Rewrites

Rewrite 3-6 bullets, profile lines, or project/workflow descriptions.

Rules:

- Do not invent metrics.
- Do not invent production usage.
- Keep the user's real experience.
- If evidence is missing, use honest language like `prototype`, `internal tool`,
  `local evaluation`, `simulated workload`, or `planned eval set`.
- Prefer action + workflow/system + evidence + role relevance.

### 6. Project Or Workflow Upgrade Suggestions

If the user has RAG, agent, or LLM projects, upgrade them using this rubric:

- User problem.
- Data source.
- Retrieval/tool workflow.
- Evaluation.
- Failure analysis.
- Deployment.
- Observability.
- Cost/latency.
- README/demo proof.

If the user is not a software engineer, translate this into a workflow proof artifact:

- Input materials.
- Decision process.
- AI-assisted steps.
- Human review.
- Quality checks.
- Before/after example.
- Business result or learning artifact.

If the user has no AI project or workflow, suggest one small proof artifact that maps to the
target role.

### 7. Interview Question Set

Generate 10 likely interview questions:

- 4 role-specific depth questions.
- 3 project/workflow tradeoff questions.
- 2 stakeholder/customer/user-facing questions.
- 1 behavioral story question.

Give answer angles, not memorized scripts.

### 8. Seven-Day Action Plan

Give a practical 7-day plan.

Each day should have:

- One action.
- One artifact to produce.
- Why it improves interview odds.

### 9. Honest Positioning

Tell the user what they should and should not claim.

Examples:

- Can claim: "built a prototype with local eval set."
- Cannot claim: "production RAG platform" unless deployed with real usage.

### 10. Xiaohongshu-Friendly Summary

Summarize the diagnosis in a short, direct style that could become a note:

- One-line problem.
- Three gaps.
- Three next actions.
- One comment CTA.

## Quality Bar

A good answer should feel like a sharp career/project/workflow teardown from a senior AI
builder, not like a generic HR resume review.

It should leave the user with a concrete next artifact to build.

## Guardrails

- Never guarantee interviews, offers, salary, immigration outcomes, or job placement.
- Never fabricate metrics, production usage, team size, revenue, users, or model quality.
- Do not blindly stuff AI keywords into bullets.
- Do not tell a user to claim FDE experience unless there is customer-facing or deployment
  evidence.
- Do not tell non-engineering users to market themselves as AI Engineers unless they have
  real technical project evidence.
- If a user is too early for the target JD, say so kindly and give a smaller next step.
- For career advice, avoid legal, immigration, or financial claims.

## Example

Weak bullet:

> Built a chatbot using LangChain and OpenAI.

Stronger truthful bullet:

> Built a document QA prototype using FastAPI, OpenAI embeddings, and a vector database;
> added a local evaluation set and citation-failure review to compare retrieval settings
> before presenting the project as an AI Engineer portfolio demo.

Why it is stronger:

- It says what was built.
- It names evidence.
- It avoids fake production claims.
- It creates interview follow-up material.

Non-engineering example:

Weak claim:

> Used ChatGPT to improve team workflows.

Stronger truthful claim:

> Built an AI-assisted customer research workflow that turns support tickets and call notes
> into a weekly insight brief, with human review, source links, quality checks, and a decision
> log for product follow-up.

Why it is stronger:

- It names the workflow.
- It shows input, review, and output.
- It avoids pretending to be an engineering system.
- It creates a proof artifact that can be discussed in interviews.
