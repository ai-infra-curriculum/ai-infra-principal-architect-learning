# Job Requirements — Principal AI Infrastructure Architect

**Cycle**: 2026-10
**Role**: Principal AI Infrastructure Architect (level 60)
**Window**: postings observed 2026-07-13 → 2026-10-11 (last 90 days)
**Sample**: 25 in-scope postings (10 carry-forward-open/refreshed from the 2026-09 baseline + 15 net-new; 16 prior-cycle postings closed/aged-out this cycle and retained for context only; 3 prior-cycle postings access-blocked and excluded from frequency counts; 24 excluded as IC-engineer / customer-facing / out-of-window despite Principal title)
**Bottom line**: **Fourth consecutive hold-steady cycle.** Every requirement appearing in ≥30% of postings is already covered by an existing module or project. No additions proposed. One notable watchlist event: **MCP (Model Context Protocol) explicit at platform level crossed the 15% principal-altitude bullet trigger set in 2026-09** (0% → 16%, 4 of 25 postings — GE Vernova, CVS Health/Aetna, DIRECTV, Raymond James Financial). Per the 2026-09 watchlist action, this triggers a bullet refinement inside `project-01-enterprise-platform` §4 (gen-AI gateway) in a subsequent lesson-authoring run, **not** a new module, exercise, or project this cycle — MCP is a protocol owned deep at level 48 and the 30% delta gate is not met. Agentic AI architecture climbed modestly (50% → 60%) but remains fully covered by existing content; NIST AI RMF / ISO 42001 explicit citations stayed at the floor (4% / 4%); regulated-industry compliance sample share stayed in the 60s%.

Sector distribution: financial services 10, healthcare/payer/life-sciences 5, consulting/SI 0, tech vendor / device 3, aerospace/defense 2, industrial/manufacturing 1, sovereign-cloud vendor 1, retail-CPG-services 0, insurance 0, travel/retail-tech 1, telco/media 1, tax/compliance SaaS 1. Geographic distribution: US ~76%, EMEA ~16%, Canada ~8%, APAC ~0%. See `.aicg/job-requirements.json` for the full normalized dataset, cycle-over-cycle deltas, and posting-level citations.

## How to read this document

- Requirements are grouped by theme and ordered by posting frequency (descending).
- Each requirement names the **lowest-level role** that owns its primary coverage (the ownership rule). Where this role adds architectural or leadership framing on top, the local module is listed too.
- For requirements not covered anywhere in the curriculum, an external resource would be listed instead. None this cycle.
- Frequency is the share of in-scope postings that explicitly cite the requirement in the verbatim posting text.
- Deltas (▲/▼) compare to the 2026-09 baseline. Absence of an arrow means ±2pp or less.

## Group 1 — Architectural strategy & reference architecture

Core executive-architect responsibilities. All cleanly covered.

| Requirement | Freq (Δ) | Primary coverage |
|---|---|---|
| Own enterprise AI reference architecture | 96% ▲ | [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md); [mod-601-org-wide-architecture](lessons/mod-601-org-wide-architecture/) |
| Multi-year AI/architecture roadmap (3–5 years) | 48% ▲ | [mod-603-multi-year-investment](lessons/mod-603-multi-year-investment/); [project-02-technology-roadmap](projects/project-02-technology-roadmap/README.md) |
| Enterprise architecture frameworks (TOGAF / Zachman / ArchiMate / FEAF) | 32% ▼ | [mod-601-org-wide-architecture](lessons/mod-601-org-wide-architecture/) |
| Multi-cloud / hybrid cloud reference architecture | 32% | [mod-601-org-wide-architecture](lessons/mod-601-org-wide-architecture/); [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) (§4: multi-cloud trade-off) |
| Reusable patterns / platform-as-product operating model | 28% | [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) (§7 operating model, D8 RACI) |

**Note on the 92% → 96% ref-architecture climb**: Still a sample-composition artifact rather than a market signal. Every surviving/refreshed and net-new posting at principal altitude this cycle is accountable for enterprise AI reference architecture — the handful of exceptions (e.g., Centific Edge-AI/IoT) are nominally scoped-down but still author ADRs and reference designs. Coverage unchanged.

**Note on multi-year roadmap climb (42% → 48%)**: Net-new postings explicitly name multi-year framing more consistently this cycle — GE Vernova ("define multi-year AI data architecture roadmap"), GSK ("multi-year enterprise architecture strategy"), AstraZeneca ("strategic investment priorities"), CACI USSS ("AI Strategy & 3-Year Roadmap"), Ford Credit ("multi-year strategy, target states"). Fully covered.

**Evidence highlights (net-new this cycle)**: CVS Health Principal AI Architect — Aetna Technology ("senior individual contributor accountable for AI architecture across Aetna Technology, setting the technical direction for how AI capabilities are built, served, orchestrated, and governed"), Raymond James Financial Principal Enterprise Data & AI Architect ("principal enterprise architect for enterprise data platforms, AI/ML platforms and capabilities, agentic data access, semantic enablement"), GE Vernova Principal AI Data Architect ("define multi-year AI data architecture roadmap… lead architecture reviews across domains"), Avalara Principal Architect — Enterprise AI ("shapes how Avalara adopts AI across the enterprise by turning new AI capabilities and validated pilots into scalable architecture standards, reusable patterns, decision frameworks, and governance guardrails"), DIRECTV Principal AI Architect ("defines, designs, and evolves enterprise-grade Generative AI and AI-driven architectures aligned with DIRECTV's strategic business objectives").

## Group 2 — Governance, standards & ARB

The principal architect typically chairs (or co-chairs) the architecture review board and owns the standards program. Fully covered.

| Requirement | Freq (Δ) | Primary coverage |
|---|---|---|
| AI governance framework (policies, standards, exception process) | 80% ▲ | [project-03-governance-framework](projects/project-03-governance-framework/README.md) |
| Regulated-industry compliance (HIPAA, GDPR, SOC2, OSFI, FINTRAC, SR 11-7, FedRAMP, FISMA, GxP, NIST SP 800-171, CMMC) | 64% | [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) (regulated multinational scenario) |
| Responsible AI / ethical AI / bias-mitigation standards | 48% ▲ | [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) (§5 MRM + EU AI Act); [project-03-governance-framework](projects/project-03-governance-framework/README.md) |
| ARB / design-authority governance | 20% | [mod-601-org-wide-architecture](lessons/mod-601-org-wide-architecture/); [project-03-governance-framework](projects/project-03-governance-framework/README.md) |
| Model risk management (SR 11-7, OSFI E-23, OCC 2011-12) | 16% | [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) (regulated FS scenario) |
| **NIST AI RMF (explicit)** | **4%** | Covered generically in [project-03-governance-framework](projects/project-03-governance-framework/README.md). <!-- needs-research: Second cycle at 4%. Only Wells Fargo r-555203 remains the single explicit citation (unverified direct fetch; cross-indexed via Wells Fargo job search). Not climbing. If it climbs to ≥30% next cycle, propose an exercise inside project-03 mapping the control catalogue to NIST AI RMF Govern/Map/Measure/Manage functions. Not module-worthy. --> |
| **ISO/IEC 42001 (explicit)** | **4%** | Covered generically in [project-03-governance-framework](projects/project-03-governance-framework/README.md). Same story — Wells Fargo r-555203 remains the single explicit citation. |

**AI governance framework climb (58% → 80%)**: Real, and strongest signal of the cycle. Net-new postings consistently describe governance ownership as a first-class responsibility — Avalara ("governance guardrails for AI-enabled solutions"), CVS Health ("author AI standards as automated gates and paved-road defaults, not as a review queue"), GE Vernova ("establish enterprise governance, security, privacy, and quality standards"), GSK ("pragmatic, agile architecture governance balancing innovation with security and compliance"), Sarepta Director AI Architecture & Governance (governance in the title). This is now definitionally in-scope — all 20 postings that cite it are already landed by `project-03-governance-framework` which already pairs policy, standards, and exception process. **No content change needed.**

**Regulated-industry compliance (62% → 64%)**: Steady. The regulated-FS skew holds (Scotiabank, BMO, Wells Fargo GenAI+Agentic, Raymond James, First Citizens, Huntington, TIAA, Truist) and is now joined by life-sciences (AstraZeneca, GSK, Sarepta — GxP, pharma R&D), healthcare (Molina, CVS/Aetna, Elevance — HIPAA/PHI), defense (CACI USSS — FedRAMP/FISMA/Zero Trust; Sierra Nevada; Centific — NIST SP 800-171/CMMC). Fully covered by project-01 §5 multi-regime regulated scenario.

**Note on NIST AI RMF / ISO 42001**: Flat at 4% / 4% — not climbing per the 2026-09 watchlist's "weakening" assessment. Wells Fargo r-555203 (Principal AI Architect, Enterprise Functions Technology) continues to be the lone explicit citation and is unverified via direct fetch this cycle; carried forward as `unverified-but-indexed`. Watchlist retained at the same priority — do NOT propose content on this signal.

**Evidence highlights**: Wells Fargo Principal Architect — GenAI and Agentic AI r-560817 ("define architectural direction for enterprise AI platform, including model platforms, AI gateways, agent orchestration frameworks, guardrails and safety controls, LLMOps and MLOps capabilities, AI observability and monitoring"), Scotiabank Chief AI Architect ("defines Scotiabank's enterprise AI solution architecture including canonical reference architectures, solution patterns, and integration blueprints that govern how GenAI, agentic AI, and ML capabilities are assembled and deployed across business lines"), CACI AI Enterprise Architect USSS ("develop AI Governance Charter & Operating Framework; AI Strategy & 3-Year Roadmap; FedRAMP, FISMA, Zero Trust"), BMO Principal Architect AI Platform ("deep grounding in Responsible AI, AI/data governance, privacy, and evaluation/guardrail design; OSFI and OCC regulatory experience"), Sarepta Director AI Architecture & Governance ("defining and governing enterprise-scale AI and Generative AI architectures… governance frameworks required to deliver AI outcomes safely and at scale").

## Group 3 — Platform capabilities (gen-AI, MLOps, agentic, MCP)

Generative AI, agentic AI, and MLOps at the platform level remain the dominant capabilities cited. All cleanly covered. **MCP crossed the 15% watchlist bullet trigger this cycle** — see note below.

| Requirement | Freq (Δ) | Primary coverage |
|---|---|---|
| Agentic AI architecture (multi-agent, orchestration, A2A, HITL guardrails) | 60% ▲ | [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) (§4.4 gen-AI gateway); [project-02-technology-roadmap](projects/project-02-technology-roadmap/README.md) (emerging-tech radar); deeper hands-on coverage at `ai-infra-agentic-systems-architect-learning` (level 48) and `ai-infra-senior-agentic-ai-engineer-learning` (level 40) |
| Generative AI / LLM platform architecture (gateway, RAG, eval) | 60% ▲ | [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) (§4.4 gen-AI gateway design question) |
| **Model Context Protocol (MCP) explicit at platform level** | **16% ▲▲** | Owned deep at `ai-infra-agentic-systems-architect-learning` (level 48). Principal-architect altitude framing: [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) (§4 gen-AI gateway — currently references "multi-agent orchestration" generically). <!-- needs-research: MCP climbed 0% -> 16% this cycle (4 of 25 postings: GE Vernova "MCP Servers and MCP Registries", CVS Health "MCP adopted by exception", DIRECTV "Model Context Protocol (MCP), multi-agent systems, and agent-to-agent orchestration frameworks", Raymond James "MCP-based tooling"). This CROSSES the 2026-09 cycle's 15% principal-altitude bullet trigger. The trigger action is a bullet refinement inside project-01 §4 adding MCP (protocol, auth patterns, registry/governance) alongside the existing gateway/orchestration bullets — handled by a subsequent lesson-authoring run, NOT this cycle's delta. Deep MCP implementation ownership stays at level 48. Do NOT propose a new module, exercise, or project. --> |
| MLOps / LLMOps governance at platform level | 16% ▲ | Owned at `ai-infra-mlops-learning` (level 30); principal architects add governance framing via [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) (D5 governance + MRM control catalogue) |

**Note on agentic AI climb (50% → 60%)**: Partial reversal of last cycle's decline. Net-new postings this cycle are more consistently agentic-forward: CVS Health ("define the agentic architecture: agent orchestration as the enforced contract, domain agents scoped by journey"), DIRECTV ("defines advanced AI architectures including Model Context Protocol (MCP), multi-agent systems, and agent-to-agent orchestration frameworks"), Raymond James ("agent design patterns and reference architectures"), Elevance ("agentic AI… emerging AI architecture patterns"), First Citizens ("centralized enterprise AI platform… agent orchestration"), Priceline ("multi-agent frameworks like LangChain/LangGraph"), GE Vernova ("agentic workflows"), Ford Credit ("agentic systems design: models, retrieval, tools, memory, orchestration, permissions"). This is still well below the 70% threshold set in 2026-06 for opening `mod-606-agentic-platform-architecture`. The 2026-09 watchlist also required that lower-level Agentic tracks (levels 40/48) still fail to cover principal-altitude framing — that condition is NOT re-validated this cycle. Coverage unchanged. **No new module or exercise proposed.**

**Note on MCP climb (0% → 16%)**: *This is the headline watchlist event of the cycle.* The 2026-09 cycle flagged MCP as a first-time watch item at 0% principal altitude, with the explicit trigger: "If MCP appears in ≥15% of principal-altitude in-scope postings, add it as a bullet inside `project-01-enterprise-platform` (§4 gen-AI gateway). Do NOT propose a new module — MCP is a protocol, owned deep at level 48." MCP cleared that trigger this cycle at exactly 4 of 25 (16%): GE Vernova, CVS/Aetna, DIRECTV, Raymond James. These are all principal-altitude internal-ARB roles at named employers across four distinct sectors (industrial, healthcare, media, FS/wealth). The trigger action is a bullet-level content refinement inside project-01 §4 to be executed by a subsequent lesson-authoring run, **not** a curriculum-plan delta entry. The 30% delta gate for a new module/exercise/project is NOT met, and MCP implementation depth remains owned at level 48 per the ownership rule. **Do not confuse the 15% watchlist bullet trigger with the 30% delta gate — the delta remains empty.**

**Note on MLOps/LLMOps slight rebound (12% → 16%)**: Priceline, Pronix, Ford Credit, Avalara all explicit; still well below prior cycle's 31% peak. Real MLOps ownership stays at level 30.

## Group 4 — Stakeholder & executive influence

Covered by the stakeholder coalition module.

| Requirement | Freq (Δ) | Primary coverage |
|---|---|---|
| Executive influence / C-suite advisory | 64% ▼ | [mod-604-stakeholder-coalition](lessons/mod-604-stakeholder-coalition/); [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) (D9 board pack) |
| Cross-organizational architecture alignment | (implicit in ~100%) | [mod-601-org-wide-architecture](lessons/mod-601-org-wide-architecture/); [mod-604-stakeholder-coalition](lessons/mod-604-stakeholder-coalition/) |

**Evidence highlights (net-new this cycle)**: AstraZeneca Chief Enterprise Architect ("C-suite influence capabilities… strategic leadership"), GSK VP Chief Enterprise Architect ("advise senior leaders on translating complex enterprise challenges into actionable architecture roadmaps"), Ford Credit Principal AI Architect ("ability to communicate technical trade-offs to executives and engineers"), CVS Health Principal AI Architect ("translate trade-offs for senior leaders"), Avalara Principal Architect ("reports to VP of Enterprise AI Transformation… influences teams across the organization without direct people management"), Sarepta Director AI Architecture & Governance ("senior technical leadership role").

**Note on the 69% → 64% drift**: Within noise; still ≫30% and fully covered. The slight dip reflects that a handful of new postings (GE Vernova, Avalara, Lenovo, Centific) frame influence as hands-on authority rather than C-suite advisory, and are correspondingly cross-counted in Group 1 only. Coverage unchanged.

**Title-cluster observation**: "Chief AI Architect" / "Chief Enterprise Architect" titles dominated again (Scotiabank, AstraZeneca, GSK VP Chief EA, TIAA Chief EA, Truist Divisional Chief Architect), with "Executive Director AI Architecture" (HARMAN carry-forward) and "Head of AI Architecture" (Lenovo) rounding out the exec cluster. One new framing — "Director, AI Architecture & Governance" (Sarepta, posted 2026-09-22) — makes governance explicit in the title. `mod-604-stakeholder-coalition`'s executive-influence framing already lands at this title cluster; no refresh needed.

## Group 5 — Investment, FinOps & vendor strategy

Covered.

| Requirement | Freq (Δ) | Primary coverage |
|---|---|---|
| Vendor / partner-tool strategy (Bedrock, Azure AI Foundry, Vertex, SageMaker, Anthropic, OpenAI, Google Gemini) | 24% ▲ | [project-02-technology-roadmap](projects/project-02-technology-roadmap/README.md) (technology radar / build-vs-buy) |
| FinOps for AI / cost-aware architecture | 16% ▲ | [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) (D6 FinOps & TCO model) |
| Multi-year capital planning | (implicit in 48% roadmap citations) | [mod-603-multi-year-investment](lessons/mod-603-multi-year-investment/) |

## Group 6 — Modernization, M&A and thought leadership

Each is covered by a dedicated project, even though the frequency is low — these are the kind of requirements that show up in only ~1 in 25 postings but are characteristic of the role when they do.

| Requirement | Freq (Δ) | Primary coverage |
|---|---|---|
| Brownfield modernization / strangler-fig migration | (implicit in roadmap + ref-arch asks) | [mod-605-tech-debt-modernization](lessons/mod-605-tech-debt-modernization/); [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) (§6 migration of 600+ models off 23 stacks) |
| M&A technical due diligence | 0% | [project-04-ma-integration](projects/project-04-ma-integration/README.md) |
| Thought leadership / conference / whitepaper / patents | 0% | [project-05-thought-leadership](projects/project-05-thought-leadership/README.md) |
| Standards-body / foundation engagement (CNCF, LF AI, MLCommons) | 0% (this window) | [mod-602-industry-standards](lessons/mod-602-industry-standards/) |

**Note**: Zero-frequency ≠ removal candidate. These are role-characteristic requirements that surface when they surface (M&A due diligence when the employer is mid-transaction; thought leadership when the employer wants a public-face architect). Removals require a separate proposal per the packet rules.

## Group 7 — First-time low-frequency and downgraded signals (watch)

Below the 30% not-covered threshold. Retained here as a running record; MCP is the only mover this cycle and triggers a `project-01 §4` bullet refinement (handled downstream of this packet, not via delta).

| Requirement | Freq (Δ) | Primary coverage / rationale |
|---|---|---|
| **Model Context Protocol (MCP) explicit** | **16% ▲▲** | **Crossed the 2026-09 cycle's 15% principal-altitude bullet trigger.** 4 postings: GE Vernova (MCP Servers + Registries), CVS/Aetna (MCP as integration exception), DIRECTV (MCP + A2A), Raymond James (MCP-based tooling preferred). Trigger action: bullet refinement inside [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) §4 adding MCP alongside existing gateway/orchestration bullets, routed to the subsequent lesson-authoring run. MCP implementation depth stays at `ai-infra-agentic-systems-architect-learning` (level 48) per the ownership rule. The 30% delta gate for module/exercise/project is NOT met. |
| NIST AI RMF (explicit) | 4% | Flat. Wells Fargo r-555203 remains the single explicit citation (indexed, direct URL 404). Covered generically in [project-03-governance-framework](projects/project-03-governance-framework/README.md). |
| ISO/IEC 42001 (explicit) | 4% | Flat. Same story. Covered generically in [project-03-governance-framework](projects/project-03-governance-framework/README.md). |
| OWASP LLM Top 10 (explicit) | 4% | Flat. Wells Fargo r-555203 remains the single citation. Owned at `ai-infra-security-learning` (level 35). |
| Sovereign cloud (standalone) | 4% | Bull/Atos p34 refreshed 2026-08-23. Standalone signal preserved but not climbing. Embedded in [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md)'s regulated-multinational scenario. |
| EU AI Act (standalone, not embedded) | 0% ▼ | Flat at zero; implicit under "regulated multinational" scenario coverage in [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) (§5 MRM + EU AI Act). |
| NIST SP 800-171 / CMMC (defense / FedRAMP cousin) | 8% ▲ | First-time explicit mentions this cycle (Centific "NIST SP 800-171 compliance, pathway toward CMMC Level 2 and Level 3"; CACI USSS "FedRAMP, FISMA, Zero Trust Architecture"). Covered inside [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md)'s regulated multinational scenario via FedRAMP/FISMA; defense-track specifics are owned at `ai-infra-security-learning` (level 35). Watch for climb. |
| Agent-to-agent (A2A) orchestration (explicit) | 8% ▲ | DIRECTV "agent-to-agent orchestration frameworks" + agentic-forward FS postings imply A2A. Owned deep at `ai-infra-agentic-systems-architect-learning` (level 48). Principal-altitude framing is in [project-01-enterprise-platform](projects/project-01-enterprise-platform/README.md) §4; same bullet-refinement path as MCP. |

## Requirements covered at lower-level roles (linked, not duplicated)

The principal architect needs to be conversant — not hands-on — with these. Coverage stays at the lowest level per the ownership rule.

| Requirement | Owning role | Why not principal-architect-owned |
|---|---|---|
| AI/ML security threat modeling (model extraction, prompt injection, supply chain, OWASP LLM Top 10) | `ai-infra-security-learning` (level 35) | Principal architects set the standard via [project-03-governance-framework](projects/project-03-governance-framework/README.md); deep technical content owned at security level |
| Agentic frameworks hands-on (LangGraph, AutoGen, CrewAI, Google ADK, **MCP implementation**) | `ai-infra-agentic-systems-architect-learning` (level 48); `ai-infra-senior-agentic-ai-engineer-learning` (level 40) | Principal architects make platform-level choices and set MCP adoption policy; the implementation patterns are taught one level down |
| GPU capacity planning / scheduler tuning | `ai-infra-performance-learning` (level 35) | Principal architects reference the FinOps and capacity plan; engineering depth is owned elsewhere |
| Feature store / vector DB / lakehouse implementation | `ai-infra-ml-platform-learning` (level 30) | Principal architects evaluate; implementation is platform-engineer territory |
| Production MLOps pipelines | `ai-infra-mlops-learning` (level 30) | Principal architects set governance; pipeline construction is MLOps-owned |
| 10+ years architecture experience (general gating criterion) | N/A (admissions criterion) | Already enforced as a prerequisite in the README |

## Continuity-bias verdict

- Zero requirements clear the gate of `(freq ≥ 30%) AND (≥ 3 distinct postings) AND (not covered anywhere in the curriculum)`.
- The 30%+ requirements — ref-architecture ownership (96%), AI governance framework (80%), regulated-industry compliance (64%), executive influence (64%), agentic AI (60%), gen-AI/LLM platform (60%), multi-year roadmap (48%), responsible AI (48%), TOGAF (32%), multi-cloud (32%) — are each explicitly covered by existing modules or projects.
- The **MCP climb (0% → 16%)** is this cycle's only mover but is a *watchlist bullet trigger*, not a *delta gate*. The 2026-09 cycle set the explicit remediation path: bullet refinement inside project-01 §4 in a subsequent lesson-authoring run. MCP is a protocol owned deep at level 48; principal-architect altitude framing is adoption policy and reference-architecture integration, not framework implementation. **Do not propose a new module, exercise, or project.**
- Agentic AI reversed last cycle's dip (50% → 60%) but remains below the 70% module-opening threshold; the lower-level Agentic tracks (levels 40/48) still cover principal-altitude framing adequately.
- NIST AI RMF / ISO/IEC 42001 / OWASP LLM Top 10 / EU AI Act standalone remain flat at 4% / 4% / 4% / 0%. No action.
- First-time explicit signals this cycle: NIST SP 800-171 / CMMC (8%) via Centific + CACI; A2A orchestration (8%) via DIRECTV. Both below any bullet trigger; both covered through existing content (project-01 regulated scenario and project-01 §4 respectively). Watch for climb.
- Proposed additions in `.aicg/curriculum-plan-delta.json`: **none** (empty `modules`, `exercises`, and `projects` arrays).

## Cycle-over-cycle diff (2026-09 → 2026-10)

**Climbers**:

- **AI governance framework: 58% → 80%** (+22pp). Real signal — net-new postings consistently foreground governance as a first-class responsibility (Avalara, CVS Health, GE Vernova, GSK, Sarepta). Fully covered by project-03.
- **Model Context Protocol (MCP) explicit: 0% → 16%** (+16pp). Headline watchlist event — crosses the 2026-09 cycle's 15% principal-altitude bullet trigger. Not a delta item; project-01 §4 bullet refinement routed to lesson authoring.
- **Agentic AI architecture: 50% → 60%** (+10pp). Partial reversal of last cycle's dip. Below the 70% module trigger. Covered.
- **Agent-to-agent (A2A) orchestration: 0% → 8%** (+8pp). First-time explicit (DIRECTV). Covered via project-01 §4 and level 48.
- **NIST SP 800-171 / CMMC: 0% → 8%** (+8pp). First-time explicit (Centific, CACI USSS). Covered via project-01 regulated scenario and level 35 security.
- **FinOps for AI: 8% → 16%** (+8pp). CVS/Aetna "unit economics as a design constraint" + Priceline "cost awareness" + Molina AI FinOps. Covered.
- **Responsible AI / ethical AI: 35% → 48%** (+13pp). Language returned ("guardrails and responsible AI controls" appears explicitly in CVS, BMO, Avalara, DIRECTV, Raymond James, GSK). Fully covered.
- **Multi-year AI/architecture roadmap: 42% → 48%** (+6pp). Multi-year framing is more explicit this cycle (GE Vernova, GSK, AstraZeneca, Ford Credit, CACI). Covered.
- **Multi-cloud / hybrid cloud architecture: 27% → 32%** (+5pp). Modest climb — BMO AWS/Azure, Priceline cloud-native, CVS AWS-primary + multicloud, Raymond James multi-platform. Covered.

**Decliners**:

- **Executive influence / C-suite advisory: 69% → 64%** (-5pp). Within noise. Still ≫30% and covered.
- **Enterprise AI reference architecture ownership: 92% → 96%** (+4pp — kept in climbers context, within noise). Sample-filter artifact.
- **TOGAF / enterprise architecture frameworks: 35% → 32%** (-3pp). Within noise. Covered.

**Flat (±2pp)**:

- NIST AI RMF, ISO/IEC 42001, OWASP LLM Top 10, EU AI Act standalone, sovereign cloud, model risk management, MLOps/LLMOps (slight uptick 12% → 16%), ARB/design-authority governance (15% → 20% — within noise), vendor/partner strategy (19% → 24%).

**Closed / aged-out prior-cycle postings** (retained for context in `.aicg/job-requirements.json` under `postings_closed_since_prior_cycle`):

- Prior carry-forwards aged out of window or verified closed this cycle: p09 Cognizant Bangalore (posted 2026-06-04, outside window), p13 Fidelity SVP (URL 404 persists), p15 3Cloud (Sept 14 2026 deadline past), p19 NTT, p21 AIG, p22 CDW (all older than window), p26 Wells Fargo SaaS r-555203 (direct 404 persists; indexed-but-unverified), p27 Vanguard (URL 404), p30 Elevance Distinguished Engineer (Sept 30 2026 deadline past — likely replaced by Elevance Enterprise Architect Executive this cycle), p36 US Bank Chief Architect (prior-cycle 410 persists), p40 Baldwin, p43 Cigna, p44 Empower, p45 Clinisys, p46 Celanese, p47 Acosta (all older than window).
- Already-closed prior-cycle context-only postings (unchanged): p03 Cisco, p06 UHG Optum, p07 Celonis, p08 Costco, p10 Slalom, p12 Citi, p14 BECU, p18 Sentara, p23 Wells Fargo Reconciliation, p25 Thoughtworks, p28 BlackRock, p29 IQVIA, p31 SAP Tokyo, p32 Deloitte, p35 Humana.

**Access-blocked without corroboration** (excluded from frequency counts): p11 Caylent, p17 Vonage, p20 Salesforce.

## Watchlist for the 2026-11 cycle

1. **Model Context Protocol (MCP) explicit at platform level** — crossed the 15% watchlist bullet trigger this cycle (0% → 16%). **Trigger action**: route a bullet refinement inside `project-01-enterprise-platform` §4 (gen-AI gateway design) to the next lesson-authoring run, adding MCP alongside the existing gateway/orchestration bullets. Deep MCP implementation stays at level 48. Watch for continued climb: if MCP reaches ≥30% next cycle AND principal-altitude postings start naming MCP registry governance, MCP server auth patterns, or MCP policy enforcement at fleet scale that is not yet covered at level 48, propose an *exercise* inside `mod-601-org-wide-architecture` on MCP adoption policy. Do NOT open a new module.
2. **Agentic AI architecture** — climbed 50% → 60% this cycle, partial reversal of last cycle's dip. Watchlist retained at the same threshold: 70% frequency AND re-validated gap at levels 40/48 are both required before opening `mod-606-agentic-platform-architecture`. Neither condition is met.
3. **Agent-to-agent (A2A) orchestration explicit** — first-time 8% this cycle (DIRECTV). Companion signal to MCP. Likely bundled under the same project-01 §4 bullet refinement; track whether it emerges as a standalone citation (vs. always paired with MCP).
4. **AI governance framework (80%)** — the single most-cited requirement this cycle after ref-architecture ownership. Watch whether this holds as the regulated-FS/healthcare/life-sciences skew in the sample normalizes. If an in-depth governance capability (e.g., AI MRM control catalogue reference implementation; EU AI Act Annex III mapping; US AI Executive Order compliance; agentic AI governance primitives) emerges in ≥30% of postings and is NOT already in project-03, propose an exercise.
5. **NIST AI RMF + ISO/IEC 42001 explicit citations** — both still flat at 4%. Watchlist retained at "weakening". If either reaches ≥30% next cycle, propose an exercise inside `project-03-governance-framework` mapping its control catalogue to the respective framework's functions/clauses. Not module-worthy.
6. **NIST SP 800-171 / CMMC** — first-time 8% this cycle (Centific, CACI USSS). Watch whether defense-sector postings expand. If this reaches ≥15% principal-altitude, extend `project-01-enterprise-platform`'s regulated multinational scenario with a defense/CMMC sub-question. Do NOT open a new module.
7. **Sovereign cloud (Bull/Atos p34) and EU AI Act standalone** — unchanged. Same trigger thresholds as 2026-09.
8. **AI governance framework super-climb (58% → 80%)** — sample-composition sensitive. Watch whether this holds when tech-vendor and retail postings return. Content unchanged either way.
9. **"Director, AI Architecture & Governance" title framing** (Sarepta new this cycle) — joins the 2026-09 title cluster of "Chief Architect — AI Platform" (US Bank, aged out) and "Executive Director, AI Architecture" (HARMAN carry-forward). Governance-in-title is a mild framing shift. `mod-604-stakeholder-coalition` already lands at this title cluster; no refresh needed yet.
10. **Verification debt** — Wells Fargo r-555203 remains indexed-but-unverified across two cycles now (direct URL 404; prior cycle cross-indexed via search). If it is not direct-verifiable in the 2026-11 cycle, downgrade its citations (NIST AI RMF, ISO 42001, OWASP LLM Top 10) to context-only and recompute watchlist frequencies.
