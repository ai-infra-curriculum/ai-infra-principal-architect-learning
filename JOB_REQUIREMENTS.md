# Job Requirements — Principal AI Infrastructure Architect

**Cycle**: 2026-06
**Role**: Principal AI Infrastructure Architect (level 60)
**Window**: postings observed 2026-03-18 → 2026-06-16 (last 90 days)
**Sample**: 25 in-window, in-scope postings (2 additional stale postings retained for context, not counted in frequency)
**Bottom line**: Hold steady. Every requirement appearing in ≥30% of postings is already covered by an existing module or project. No additions proposed this cycle.

The role at this altitude is genuinely scarce. Of the ~70 postings inspected, most "Principal AI Architect" titles are senior IC engineer roles and were excluded. The 25 in-scope postings come from financial services (8), consulting/SI (6), tech vendors (5), healthcare (3), telecom (2), and one each from retail and industrial — a mix that matches the cohort's target market. See `.aicg/job-requirements.json` for the full normalized dataset and posting-level citations.

## How to read this document

- Requirements are grouped by theme and ordered by posting frequency (descending).
- Each requirement names the **lowest-level role** that owns its primary coverage (the ownership rule). When this role needs extra depth or leadership context, the local module is listed too.
- For requirements not covered anywhere in the curriculum, an external resource is listed instead. None this cycle.
- Frequency is the share of in-scope postings that explicitly cite the requirement in the verbatim posting text.

## Group 1 — Architectural strategy & reference architecture

These are the core executive-architect responsibilities. All cleanly covered.

| Requirement | Freq | Primary coverage |
|---|---|---|
| Own enterprise AI reference architecture | 68% | [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md); [mod-601-org-wide-architecture](lessons/mod-601-org-wide-architecture/) |
| Multi-year AI/architecture roadmap (3–5 years) | 56% | [mod-603-multi-year-investment](lessons/mod-603-multi-year-investment/); [project-02-technology-roadmap](projects/project-02-technology-roadmap/README.md) |
| Multi-cloud / hybrid cloud reference architecture | 44% | [mod-601-org-wide-architecture](lessons/mod-601-org-wide-architecture/); [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) (§4: multi-cloud trade-off) |
| Enterprise architecture frameworks (TOGAF / Zachman / ArchiMate) | 36% | [mod-601-org-wide-architecture](lessons/mod-601-org-wide-architecture/) |
| Reusable patterns / platform-as-product operating model | 28% | [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) (§7 operating model, D8 RACI) |

**Evidence highlights**: Molina ("enterprise-wide AI strategy, architecture, and roadmap"), Caterpillar ("technical leader and trusted advisor on AI solution design"), Scotiabank ("12+ years…at least 5 years as the architecture authority"), Truist Bank ("primary accountability for defining and executing an AI-first, cloud-first enterprise architecture strategy"), Costco ("Shape AI/ML strategy and define reference architectures").

## Group 2 — Governance, standards & ARB

The principal architect typically chairs (or co-chairs) the architecture review board and owns the standards program. Fully covered.

| Requirement | Freq | Primary coverage |
|---|---|---|
| AI governance framework (policies, standards, exception process) | 56% | [project-03-governance-framework](projects/project-03-governance-framework/README.md) |
| ARB / design-authority governance | 32% | [mod-601-org-wide-architecture](lessons/mod-601-org-wide-architecture/); [project-03-governance-framework](projects/project-03-governance-framework/README.md) |
| Responsible AI / ethical AI / bias-mitigation standards | 40% | [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) (§5 MRM + EU AI Act); [project-03-governance-framework](projects/project-03-governance-framework/README.md) |
| Model risk management (SR 11-7, OCC 2011-12, OSFI E-23) | 20% | [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) (regulated FS scenario) |
| Regulated-industry compliance (HIPAA, GDPR, SOC2, DORA, FINTRAC) | 28% | [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) (regulated multinational scenario) |

**Evidence highlights**: Slalom ("Define and implement AI governance frameworks, including model risk management, safety, and compliance"), Cognizant ("AI Governance, Responsible AI, Compliance: Define and enforce ethical AI principles, model risk management, and explainability standards"), Celonis ("12+ years in Enterprise Architecture or a CTO-level role"), Costco ("Establish governance frameworks and standards").

## Group 3 — Platform capabilities (gen-AI, MLOps, agentic)

Generative AI is now the dominant platform capability cited at this level. Covered by the Enterprise Platform project, which already includes a gen-AI gateway design as a graded deliverable.

| Requirement | Freq | Primary coverage |
|---|---|---|
| Generative AI / LLM platform architecture (gateway, RAG, eval) | 52% | [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) (§4.4 gen-AI gateway design question) |
| Agentic AI architecture (multi-agent, orchestration, MCP, HITL guardrails) | 48% | [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) (§4.4 gen-AI gateway); [project-02-technology-roadmap](projects/project-02-technology-roadmap/README.md) (emerging-tech radar) |
| MLOps / LLMOps governance at platform level | 32% | [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) (D5 governance + MRM control catalogue) |

**Note on agentic**: this was the closest-to-genuine-gap requirement at 48% frequency. Postings cite specific frameworks (LangGraph, AutoGen, CrewAI), MCP integration, agent lifecycle management, and HITL controls. The principal-architect curriculum treats these inside the gen-AI gateway design and the technology-radar exercise; deeper hands-on coverage lives in the lower-level Agentic AI tracks (`ai-infra-agentic-systems-architect-learning` at level 48, `ai-infra-senior-agentic-ai-engineer-learning` at level 40). Per the ownership rule, principal architects should reference those tracks for depth and use the existing gen-AI gateway design exercise here. No new module proposed — the requirement is covered at the appropriate altitude.

## Group 4 — Stakeholder & executive influence

Covered by the stakeholder coalition module.

| Requirement | Freq | Primary coverage |
|---|---|---|
| Executive influence / C-suite advisory | 56% | [mod-604-stakeholder-coalition](lessons/mod-604-stakeholder-coalition/); [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) (D9 board pack) |
| Cross-organizational architecture alignment | (implicit in 100%) | [mod-601-org-wide-architecture](lessons/mod-601-org-wide-architecture/); [mod-604-stakeholder-coalition](lessons/mod-604-stakeholder-coalition/) |

**Evidence highlights**: Thoughtworks ("acting as a strategic AI advisor to C-suite and senior technical stakeholders"), Fidelity SVP AI Architecture ("define and implement enterprise-wide core and common AI architecture and strategy"), 3Cloud ("Lead executive and architectural design sessions").

## Group 5 — Investment, FinOps & vendor strategy

Covered.

| Requirement | Freq | Primary coverage |
|---|---|---|
| FinOps for AI / cost-aware architecture | 16% | [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) (D6 FinOps & TCO model) |
| Vendor / partner-tool strategy (Bedrock, Azure AI Foundry, Vertex) | 16% | [project-02-technology-roadmap](projects/project-02-technology-roadmap/README.md) (technology radar / build-vs-buy) |
| Multi-year capital planning | (implicit in 56% roadmap citations) | [mod-603-multi-year-investment](lessons/mod-603-multi-year-investment/) |

## Group 6 — Modernization, M&A and thought leadership

Each is covered by a dedicated project, even though the frequency is low — these are the kind of requirements that show up in only ~1 in 25 postings but are characteristic of the role when they do.

| Requirement | Freq | Primary coverage |
|---|---|---|
| Brownfield modernization / strangler-fig migration | (implicit in roadmap + reference-architecture asks) | [mod-605-tech-debt-modernization](lessons/mod-605-tech-debt-modernization/); [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) (§6 migration of 600+ models off 23 stacks) |
| M&A technical due diligence | 4% | [project-04-ma-integration](projects/project-04-ma-integration/README.md) |
| Thought leadership / conference / whitepaper / patents | 16% | [project-05-thought-leadership](projects/project-05-thought-leadership/README.md) |
| Standards-body / foundation engagement (CNCF, LF AI, MLCommons) | 0% (this window) | [mod-602-industry-standards](lessons/mod-602-industry-standards/) |

## Requirements covered at lower-level roles (linked, not duplicated)

The principal architect needs to be conversant — not hands-on — with these. Coverage stays at the lowest level per the ownership rule.

| Requirement | Owning role | Why not principal-architect-owned |
|---|---|---|
| AI/ML security threat modeling (model extraction, prompt injection, supply chain) | `ai-infra-security-learning` (level 35) | Principal architects set the standard via [project-03-governance-framework](projects/project-03-governance-framework/README.md); deep technical content owned at security level |
| Agentic frameworks hands-on (LangGraph, AutoGen, CrewAI, MCP) | `ai-infra-agentic-systems-architect-learning` (level 48); `ai-infra-senior-agentic-ai-engineer-learning` (level 40) | Principal architects make platform-level choices; the implementation patterns are taught one level down |
| GPU capacity planning / scheduler tuning | `ai-infra-performance-learning` (level 35) | Principal architects reference the FinOps and capacity plan; engineering depth is owned elsewhere |
| Feature store / vector DB / lakehouse implementation | `ai-infra-ml-platform-learning` (level 30) | Principal architects evaluate; implementation is platform-engineer territory |
| Production MLOps pipelines | `ai-infra-mlops-learning` (level 30) | Principal architects set governance; pipeline construction is MLOps-owned |
| 10+ years architecture experience (general gating criterion) | N/A (admissions criterion) | Already enforced as a prerequisite in the README |

## Continuity-bias verdict

- Zero requirements clear the gate of `(freq ≥ 30%) AND (≥ 3 distinct postings) AND (not covered anywhere in the curriculum)`.
- The one near-miss (agentic AI architecture, 48%, 5+ citations) fails the third condition: it is already addressed in `project-01-enterprise-platform` (gen-AI gateway design) and the lower-level Agentic AI tracks. No new module or exercise warranted.
- Proposed additions in `.aicg/curriculum-plan-delta.json`: **none** (empty `modules`, `exercises`, and `projects` arrays).

## Cycle-over-cycle note

This is the first cycle for which `JOB_REQUIREMENTS.md` has existed in this repo. Subsequent cycles should diff against this baseline. If the agentic-AI frequency climbs from 48% toward 70%+ and the lower-level Agentic tracks don't grow to absorb principal-altitude framing (multi-agent governance at enterprise scale, agent-platform reference architecture, fleet-level autonomy controls), a `mod-606-agentic-platform-architecture` becomes defensible. Not this cycle.
