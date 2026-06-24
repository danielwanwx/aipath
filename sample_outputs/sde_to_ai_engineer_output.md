# AIPath Report

## Input Snapshot

- Target role: AI Engineer / Forward Deployed Engineer
- Target company type: AI startup or B2B SaaS company
- Timeline: Wants to apply in 3-4 weeks
- Biggest concern: Resume looks like normal backend SDE, not AI Engineer.

Background summary:

> Backend SDE with 4 years of experience building APIs and internal tools. Recently built a PDF Q&A RAG demo and experimented with LangChain, OpenAI, and vector databases.

Target JD:

> Build and deploy LLM-powered workflows for enterprise customers. Work across backend systems, retrieval pipelines, evaluation, observability, and customer-facing implementation. Strong Python, API design, cloud deployment, and communication skills required.

## 1. Fit Snapshot

Fit: **Needs project proof**

Readiness score: **51/100**

Interpretation: you have a real backend foundation and an AI project seed, but your current
profile still reads more like a backend SDE who experimented with LLM tools than an AI
Engineer/FDE candidate who can defend evaluation, deployment, and customer-facing tradeoffs.

## 2. Role Direction

Best current direction: AI Engineer / Applied AI Engineer, with FDE as a stretch direction after adding customer-facing and deployment proof.

This sample is still closest to the engineering lane because the user already has backend,
API, and RAG evidence. A non-engineering user would not be forced into this lane; the Skill
would map them toward AI PM, AI Ops, automation builder, or a smaller proof artifact first.

## 3. JD Signal Map

| Signal | Status |
| --- | --- |
| Backend/API systems | Covered |
| RAG/retrieval | Covered |
| Evaluation | Weak |
| Deployment | Weak |
| Observability | Missing |
| Customer/FDE communication | Covered |
| Data pipeline | Covered |
| LLM workflow | Covered |

## 4. Evidence Gaps

- Your backend experience is useful, but the AI narrative is concentrated in one local demo.
- The RAG project lacks evaluation evidence, so it is hard to prove quality improvement.
- There is no AI deployment story yet, even though the JD asks for deployed customer workflows.
- Observability is missing: no logs, metrics, trace IDs, token usage, or failure taxonomy.
- FDE/customer-facing evidence is present only indirectly through product/support collaboration.
- The resume needs stronger bridge language: backend systems -> LLM workflow reliability -> customer implementation.

## 5. Positioning Rewrites

Original:

> Built REST APIs for internal workflow tools using Python and Postgres.

Rewrite:

> Built Python/Postgres APIs for internal workflow tools, strengthening the backend foundation needed for AI workflow deployment, data access patterns, and customer-facing implementation work.

Original:

> Improved backend job reliability and reduced manual operations for support teams.

Rewrite:

> Improved backend job reliability for support workflows by reducing manual operational steps, creating a stronger story for FDE-style automation and workflow implementation.

Original:

> A local RAG app where users upload PDFs and ask questions.

Rewrite:

> Built a local document QA prototype with FastAPI, Next.js, OpenAI API, Chroma, LangChain; next step is adding a saved evaluation set, citation-failure logging, and retrieval-setting comparison before positioning it as an AI Engineer portfolio project.

## 6. Project Or Workflow Upgrade Suggestions

Upgrade the `PDF Course Notes Q&A` project in this order:

1. Define one user workflow: education team searches course notes with cited answers.
2. Add a 30-question eval set: lookup, synthesis, ambiguity, refusal, and citation checks.
3. Log retrieved chunks, answer status, citation presence, latency, and token usage.
4. Compare three retrieval settings: chunk size, overlap, and top-k.
5. Add a README section explaining failure cases and tradeoffs.
6. Deploy a small demo or record a reproducible local demo with setup instructions.
7. Write one FDE scenario: onboarding a new customer's document set and validating quality.

## 7. Interview Question Set

Technical depth:

- How does your retrieval pipeline work from document ingestion to answer generation?
- How would you evaluate whether retrieval quality improved?
- What happens when the model has weak or conflicting context?
- How would you control latency and token cost?

System/project tradeoff:

- Why did you choose this vector store and retrieval strategy?
- What would need to change before a customer could use this?
- How would you debug a bad answer reported by a user?

FDE/customer-facing:

- What questions would you ask before deploying this for an enterprise customer?
- How would you explain the system's limitations to a non-technical stakeholder?

Behavioral:

- Tell me about a time you turned an ambiguous workflow problem into a shipped system.

## 8. Seven-Day Action Plan

| Day | Action | Artifact | Why It Helps |
| --- | --- | --- | --- |
| 1 | Rewrite target resume headline and summary | AI Engineer/FDE positioning summary | Makes the transition story legible |
| 2 | Create 30 eval questions for the RAG project | `eval/questions.jsonl` | Adds quality evidence |
| 3 | Add retrieval/citation logging | Failure log sample | Creates debugging story |
| 4 | Compare chunk/top-k settings | Small eval table | Shows engineering tradeoff |
| 5 | Rewrite README around problem/eval/failures | Portfolio README | Makes the project reviewable |
| 6 | Write 90-second project story | Interview script | Improves live interview clarity |
| 7 | Apply to 5 roles and track JD gaps | Application tracker | Converts diagnosis into action |

## 9. Honest Positioning

Can claim:

- Backend SDE with workflow automation experience.
- Built a local RAG/document QA prototype.
- Actively adding evaluation and failure-analysis artifacts.
- Strong fit for roles needing backend + AI workflow implementation.

Should not claim yet:

- Production AI platform.
- Real customer deployment for the RAG app.
- Measured retrieval accuracy unless the eval set is actually run.
- FDE experience unless the story is tied to real stakeholder/customer-facing work.

## 10. Xiaohongshu-Friendly Summary

你不是完全不匹配 AI Engineer。

你现在的问题是：后端基础有了，AI 项目也有苗头，但证据链还不够。

最该补的 3 件事：

1. 给 RAG 项目加 eval set。
2. 把简历从工具名改成系统和 tradeoff。
3. 准备一段能解释用户场景、失败案例和下一步部署的面试故事。

评论区发 `JD`，我可以放一份输入模板。
