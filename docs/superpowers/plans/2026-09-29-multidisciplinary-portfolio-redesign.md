# Multidisciplinary Portfolio Redesign Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Rewrite the public Portfolio so it presents Karan as a multidisciplinary problem-solver whose value comes from connecting research, commercial reasoning, strategy, systems, data, product, and execution.

**Architecture:** Preserve the existing static GitHub Pages site and rewrite the current HTML/CSS in place. The new site will use evidence-led case studies and reasoning flows instead of skill-first cards, with Chuck and PYXS as the main case studies, company/GTM research as a major proof point, data architecture as a focused reasoning example, and Intrader as a small side project.

**Tech Stack:** Static HTML5, CSS3, GitHub Pages.

**Spec:** `docs/superpowers/specs/2026-09-29-multidisciplinary-portfolio-design.md`

## Global Constraints

- Keep the existing static GitHub Pages architecture.
- Do not introduce a JavaScript framework or build system.
- Do not publish confidential company/customer data, credentials, internal identifiers, private Slack channels, or proprietary source code.
- Do not invent achievements, metrics, titles, or claims.
- Keep the actual formal title **Associate Team Lead — Centre of Excellence** and employer **InsideJob**.
- Intrader must remain visually and editorially secondary as a personal side project.
- Tools must appear as execution mechanisms, not as the primary professional identity.
- The site must remain responsive and accessible.
- The visual direction remains dark, minimal, professional, and editorial rather than flashy.

## Review Focus

1. **Narrow-role regression:** hero/profile copy must not reduce the positioning to engineering, operations, RevOps, or data alone.
2. **Unsupported superiority claims:** no copy should claim exceptional intelligence, "above average," or "can do everything"; breadth must be demonstrated through evidence.
3. **Confidentiality leakage:** case studies must remain generalized and must not expose private customer/company records, internal identifiers, or proprietary operational details.
4. **Intrader prominence:** side-project treatment must remain secondary to Chuck, PYXS, company research, and data/system reasoning.
5. **Mobile readability:** long case-study flows and lens grids must collapse cleanly without horizontal scrolling or illegible text.

---

### Task 1: Rewrite the Portfolio Information Architecture and Core Copy

**Files:**
- Modify: `index.html`

**Interfaces:**
- Consumes: Existing static site structure and links to `resume.html`, GitHub, and `styles.css`.
- Produces: Semantic section/class structure consumed by Task 2 styling: `.hero`, `.hero-proof`, `.thinking-flow`, `.lens-grid`, `.case-study`, `.case-flow`, `.principle`, `.side-project`, `.tool-grid`.

- [ ] **Step 1: Replace the narrow hero positioning**

Set the eyebrow to:
`Research · Strategy · Systems · Data · Product · Execution`

Use hero copy that states that Karan works across disciplines and moves from unclear problems to evidence, models, decisions, systems, and execution without claiming a single narrow professional identity.

- [ ] **Step 2: Add the core reasoning model**

Create a "How I Think" section containing this sequence:

`Understand the real problem → Map the system → Gather evidence → Separate fact from assumption → Find patterns → Model rules → Identify constraints → Design → Build → Test edge cases → Learn → Redesign`

Add a short note that the sequence loops when new evidence changes the model.

- [ ] **Step 3: Add the multidirectional lens section**

Create "One problem. Multiple lenses." with nine lenses:
Research, Commercial, Strategy, Data, Systems, Product, Technical, Risk, Learning.

Each lens gets a single question-style description matching the design spec.

- [ ] **Step 4: Add Company/GTM Research as a major case study**

Use the generalized flow:
`Client capability → Campaign → Industry → Sub-industry → Commodity / Part → Company → Persona → Contact → Commercial outcome`

Include the key reasoning question:
`Why should this company need this capability, why might the need exist now, and what evidence would prove or disprove that hypothesis?`

Keep client/company examples generalized.

- [ ] **Step 5: Add Chuck as the flagship case study**

Use the progression:
`Manual workflow → Automation → Explicit business rules → Canonical state → Historical reconciliation → Stable identity → Database-backed processing → Targeted updates → Scale constraints → Health gates`

Include question prompts about truth, identity, source authority, superseding information, historical/live coexistence, recoverable unusable data, large-dataset updates, and platform limits.

Include the principle:
`Preserve what is already healthy. Find the smallest responsible layer. Change that layer without destabilizing the rest of the system.`

- [ ] **Step 6: Add Data Architecture as a focused proof section**

Use the public architecture flow:
`Staging → Identity / index layer → Targeted lookup → Update / insert decision → Master record`

Discuss stable identity, newer-information precedence, reusable/unusable states, deduplication, appearances/history, bounded processing, and avoiding unnecessary full-table scans.

- [ ] **Step 7: Add PYXS as the second flagship case study**

Use the reasoning chain:
`Company identity → Facilities → Equipment → Capabilities → Applications → Market context → Buying signals → Timing → Company → Relevant persona`

Also show:
`Fact → Pattern → Inference → Hypothesis → Evidence needed → Action`

Include the principle:
`Unknown facts should remain unknown until evidence supports them.`

- [ ] **Step 8: Add capabilities and tools with the correct hierarchy**

First show ways of working:
problem reframing, research decomposition, systems modeling, commercial reasoning, data modeling, constraint-first design, root-cause analysis, product thinking, iterative experimentation, business-to-technical translation.

Then show tools separately under a heading such as "Tools I use to execute ideas."

- [ ] **Step 9: Demote Intrader**

Create one compact side-project section describing Intrader as a personal experiment for market-data ingestion, experimental design, validation discipline, interface design, and no-lookahead testing.

Do not make profit/performance claims.

- [ ] **Step 10: Verify semantic content**

Check:
- exactly one `h1`;
- heading hierarchy is ordered;
- links to `resume.html` and GitHub still work;
- no confidential names/identifiers are present;
- hero does not contain the old `GTM Systems · Automation · Data Operations` positioning.

- [ ] **Step 11: Commit**

```bash
git add index.html
git commit -m "Rewrite portfolio around multidisciplinary problem solving"
```

---

### Task 2: Redesign the Visual Hierarchy for Evidence-Led Case Studies

**Files:**
- Modify: `styles.css`

**Interfaces:**
- Consumes: Class names introduced in Task 1.
- Produces: Responsive, accessible layout for the new hero, thinking flow, lens grid, case studies, principles, tools, and side project.

- [ ] **Step 1: Preserve and refine the dark visual system**

Keep the existing dark palette and typography base, but improve contrast, spacing, and hierarchy for longer editorial sections.

- [ ] **Step 2: Style the hero as broad capability, not role-card-first**

Reduce the visual weight of the current role card. Add a concise proof/positioning panel that supports the main statement without making job title the dominant identity.

- [ ] **Step 3: Style the thinking flow**

Create a responsive flow using flex/grid chips or numbered stages. It must wrap naturally on smaller screens and must not depend on horizontal scrolling.

- [ ] **Step 4: Style the lens grid**

Use a 3-column desktop grid, 2-column tablet grid where appropriate, and 1-column mobile layout.

- [ ] **Step 5: Style case studies as editorial narratives**

Create clear visual treatment for:
- case study eyebrow/title;
- problem framing;
- progression flow;
- "questions I asked" block;
- principle/callout;
- supporting explanation.

Chuck and PYXS should have stronger visual weight than the side project.

- [ ] **Step 6: Style Intrader as secondary**

Use reduced size/contrast and compact spacing so it is clearly a side experiment.

- [ ] **Step 7: Add accessibility details**

Add visible `:focus-visible` states, maintain sufficient contrast, and ensure link/button states are visible without relying only on color.

- [ ] **Step 8: Verify responsive rules**

At widths below 850px:
- all multi-column grids collapse cleanly;
- no horizontal overflow;
- hero stacks vertically;
- case flows wrap;
- large headings remain within viewport width.

- [ ] **Step 9: Commit**

```bash
git add styles.css
git commit -m "Add editorial case study styling"
```

---

### Task 3: Rewrite the CV Around Multidisciplinary Problem Solving

**Files:**
- Modify: `resume.html`

**Interfaces:**
- Consumes: Positioning and evidence model from the spec and Task 1.
- Produces: Print-friendly CV that remains truthful to formal experience while demonstrating broader capability.

- [ ] **Step 1: Replace the title line**

Remove `GTM Systems · Automation · Data Operations` as the primary identity.

Use:
`Multidisciplinary Problem Solving · Research · Strategy · Systems · Data · Product`

- [ ] **Step 2: Rewrite the profile**

Describe the ability to move from ambiguous business questions through research, commercial context, systems/data modeling, process/product design, and technical implementation.

Do not claim a formal engineering role.

- [ ] **Step 3: Rewrite the InsideJob experience bullets**

Keep:
`Associate Team Lead — Centre of Excellence`

Rewrite bullets to emphasize:
- structured target/company research;
- translating research into repeatable decision frameworks;
- redesigning operational workflows;
- defining data-quality and canonical-state rules;
- building/steering automation and internal systems;
- connecting business users, process semantics, data, and implementation.

- [ ] **Step 4: Reorder projects**

Order:
1. Chuck
2. PYXS
3. Company / GTM Research Methodology
4. Intrader — Side Project

- [ ] **Step 5: Replace generic problem-solving lists with evidence-led capabilities**

Keep the CV concise enough for print while emphasizing problem reframing, research decomposition, systems modeling, commercial reasoning, constraint-first design, data modeling, product thinking, experimentation, and business-to-technical translation.

- [ ] **Step 6: Keep tools compact**

Present tools in one concise section below capabilities rather than as the dominant qualification.

- [ ] **Step 7: Verify print behavior**

Ensure existing print CSS still fits the revised content and that no section is cut off awkwardly because of oversized blocks.

- [ ] **Step 8: Commit**

```bash
git add resume.html
git commit -m "Reframe CV around multidisciplinary capability"
```

---

### Task 4: Align the Repository README and Final Verification

**Files:**
- Modify: `README.md`

**Interfaces:**
- Consumes: Final positioning from Tasks 1–3.
- Produces: Repository README that accurately describes the purpose of the public portfolio.

- [ ] **Step 1: Rewrite the opening profile**

Describe the portfolio as evidence of multidisciplinary problem solving across research, strategy, systems, data, product, and execution.

- [ ] **Step 2: Rewrite selected work summaries**

Order and describe:
- Chuck — flagship internal workflow/data/system reasoning case study;
- PYXS — manufacturing research-intelligence case study;
- Company/GTM research methodology;
- Intrader — side experiment.

Do not expose confidential implementation details.

- [ ] **Step 3: Reframe the stack**

Rename the stack section to indicate these are tools used to execute ideas rather than the professional identity.

- [ ] **Step 4: Verify content consistency across all files**

Confirm:
- hero/profile positioning is consistent in `index.html`, `resume.html`, and `README.md`;
- Intrader is secondary everywhere;
- Chuck and PYXS are the main system case studies;
- company research is represented as a serious capability;
- no confidential details were added;
- all project links are valid.

- [ ] **Step 5: Verify the published static structure**

Confirm the repository still contains:
- `index.html`
- `resume.html`
- `styles.css`
- existing GitHub Pages workflow

No build step or framework should be required.

- [ ] **Step 6: Commit**

```bash
git add README.md
git commit -m "Align portfolio README with multidisciplinary positioning"
```

---

## Self-Review

- **Spec coverage:** All design-spec sections map to Tasks 1–4: positioning, thinking model, multidirectional lenses, company research, Chuck, data architecture, PYXS, side-project Intrader, tools hierarchy, CV, visual system, confidentiality, responsive behavior, and static architecture.
- **Step scan:** Each step changes one coherent aspect of one file and has a checkable result.
- **Type/interface consistency:** Class names introduced in Task 1 are explicitly the styling interface consumed by Task 2. No JavaScript interfaces are introduced.
- **Review Focus:** The five highest-risk regressions are explicitly covered by content and responsive verification steps.
- **Proportion:** The plan is implementation-specific but remains shorter than a code transcript; no HTML/CSS bodies are embedded.
