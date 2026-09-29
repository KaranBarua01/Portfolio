# Multidisciplinary Portfolio Redesign — Design Spec

**Date:** 2026-09-29  
**Repository:** `KaranBarua01/Portfolio`

## 1. Purpose

Redesign the portfolio so that it does not position Karan primarily as an engineer, operations specialist, analyst, salesperson, or any other narrow function.

The portfolio should present a consistent, evidence-backed pattern:

> Karan approaches difficult problems from multiple directions — research, commercial context, strategy, data, systems, product, technical execution, risk, and learning — and can move from an ambiguous problem to a working, testable solution.

The site must prove this through case studies and reasoning traces rather than relying on adjectives such as "systems thinker" or "problem solver."

## 2. Primary positioning

The main identity will be:

**Multidisciplinary problem solving across research, strategy, systems, data, product, and execution.**

The portfolio must communicate breadth without using unsupported claims such as "I can do everything" or "above average." The reader should infer unusual range from the evidence.

## 3. Design principles

1. **Proof before labels**  
   Show how problems were reframed, modeled, tested, and improved before listing capabilities.

2. **Thinking before tools**  
   Python, SQL, D1, Workers, APIs, Excel, GitHub, and Slack are execution tools, not the headline identity.

3. **Cross-domain reasoning**  
   Each major case study should show more than one lens: business, data, system, technical, research, product, or risk.

4. **No confidential disclosure**  
   Internal company/customer data, proprietary implementation details, credentials, private records, and sensitive identifiers stay out of the public site.

5. **No inflated claims**  
   Avoid unsupported performance claims or personality judgments. Use concrete examples and explain the reasoning process.

6. **Static and maintainable**  
   Keep the existing static GitHub Pages architecture. Do not introduce a framework unless the current HTML/CSS structure becomes insufficient.

## 4. Information architecture

### 4.1 Hero

Replace the current narrow headline with a broader positioning line:

**Research · Strategy · Systems · Data · Product · Execution**

The hero copy should explain that the value is the ability to move between disciplines depending on the problem while preserving one consistent problem-solving method.

Primary actions:
- View CV
- GitHub

### 4.2 Core section — How I Think

This becomes the conceptual center of the site.

Represent the working sequence:

**Understand the real problem → map the system → gather evidence → separate fact from assumption → find patterns → model rules → identify constraints → design → build → test edge cases → learn → redesign**

This section should explain that the sequence is not always linear; the work loops when new evidence changes the model.

### 4.3 Multidirectional Thinking

Add a dedicated section titled around the idea **One problem. Multiple lenses.**

The lenses should include:
- Research — what is actually happening?
- Commercial — why does it matter?
- Strategy — where should attention go?
- Data — what information represents reality?
- Systems — how are the parts connected?
- Product — what would help the user?
- Technical — what should be encoded or automated?
- Risk — what happens when assumptions fail?
- Learning — what should change after the result?

The purpose is to demonstrate that the same person can operate across these views instead of handing the problem off at every boundary.

## 5. Case studies

### 5.1 Company Research / GTM Research

This case study proves that the reasoning pattern existed before the larger software systems.

Frame the progression from simple account research toward a structured commercial decision process.

The public version may show a generalized flow such as:

**Client capability → Campaign → Industry → Sub-industry → Commodity / Part → Company → Persona → Contact → Commercial outcome**

The case study should explain that research began to consider:
- whether the company actually manufactures or consumes the relevant capability;
- make-vs-buy implications;
- evidence quality;
- exclusions and DNP logic;
- prior outcomes;
- market and sourcing context;
- whether there is a plausible commercial reason for demand now.

The key question to surface:

> Why should this company need this capability, why might the need exist now, and what evidence would prove or disprove that hypothesis?

### 5.2 Chuck — Flagship Case Study

Chuck should be the strongest proof of multidirectional problem solving.

Do not describe it only as a Slack or Cloudflare automation.

Use a progression narrative:

**Manual workflow → automation → inconsistent business meaning → explicit rules → canonical state → historical reconciliation → stable identity → database-backed processing → deduplication/update behavior → scale constraints → health gates and safe change**

The case study should show the kinds of questions that drove the design:
- Where should truth live?
- What makes two records the same?
- Which source is authoritative for which fact?
- How should later information supersede older information?
- How should historical and live records coexist?
- What happens when previously unusable data becomes usable?
- How can updates avoid repeatedly scanning a very large master dataset?
- How do platform/runtime/write limits change the architecture?

Highlight the working principle:

> Preserve what is already healthy. Find the smallest responsible layer. Change that layer without destabilizing the rest of the system.

Implementation details remain generalized because Chuck contains internal operational logic.

### 5.3 Data Architecture / Master Data Reasoning

Give the large-data architecture work its own focused section rather than burying it inside Chuck.

Public framing:

**staging → identity/index layer → targeted lookup → update/insert decision → master record**

Discuss:
- stable identity;
- source/address mapping;
- newer-information precedence;
- reusable vs unusable states;
- deduplication;
- appearances/history;
- bounded processing;
- avoiding unnecessary full-table scans.

Do not publish internal table contents or sensitive business rules.

### 5.4 PYXS — Flagship Case Study

Present PYXS as a research-intelligence system designed to understand why an opportunity may exist, not as a generic scraper.

Use the reasoning chain:

**Company identity → facilities → equipment → capabilities → applications → market context → buying signals → timing → company → relevant persona**

Also show the epistemic discipline:

**Fact → Pattern → Inference → Hypothesis → Evidence needed → Action**

Important principle:

> Unknown facts should remain unknown until evidence supports them.

The current null-preserving/no-inference architecture is a concrete implementation of that principle.

The case study can also explain the long-term learning goal: prior research, outcomes, RFQs, and signals should improve later decisions rather than disappearing after each run.

### 5.5 Intrader — Side Project

Intrader must be visually and editorially secondary.

Label it clearly as a personal side experiment used to explore:
- market-data ingestion;
- experimental design;
- validation discipline;
- interface design;
- no-lookahead testing;
- risk-aware analysis.

Do not position trading as a professional identity or make profit/performance claims.

## 6. Capabilities section

Replace the current skill-first presentation with two layers.

### Layer A — Ways of working

Use evidence-backed capabilities such as:
- problem reframing;
- research decomposition;
- systems modeling;
- commercial reasoning;
- data modeling;
- constraint-first design;
- root-cause analysis;
- product thinking;
- iterative experimentation;
- business-to-technical translation.

### Layer B — Tools used to execute

Place lower on the page:
- Python
- SQL / SQLite / Cloudflare D1
- JavaScript / Cloudflare Workers
- REST APIs / WebSockets
- Git / GitHub
- Slack workflow integrations
- Excel / CSV data pipelines
- testing / validation / QA

The wording must make clear that the tools are mechanisms, not the identity.

## 7. CV redesign

The CV must remain credible for hiring use while sharing the portfolio's broader positioning.

### Profile

Replace the current operations-heavy framing with a multidisciplinary profile centered on:
- ambiguous problem solving;
- research;
- commercial context;
- systems;
- data;
- product;
- technical execution.

### Experience

Keep the actual title **Associate Team Lead — Centre of Excellence** and employer **InsideJob**.

Rewrite bullets so they describe:
- problems identified;
- systems/processes redesigned;
- research methods developed;
- data-quality logic defined;
- operational/technical mechanisms built;
- cross-functional translation performed.

Avoid implying a formal engineering title that was not held.

### Projects

Order:
1. Chuck
2. PYXS
3. Company/GTM Research methodology
4. Intrader — side project

## 8. Visual design

Keep the existing dark visual language but strengthen hierarchy.

### Direction

- dark, minimal, professional;
- strong typography;
- more editorial case-study layout;
- fewer repetitive card grids;
- use timeline/flow structures where reasoning is sequential;
- use contrast between "problem", "question", "model", and "result";
- avoid flashy portfolio gimmicks that reduce credibility.

### Responsive behavior

The site must remain readable on desktop and mobile.

### Accessibility

- semantic headings;
- sufficient text contrast;
- visible focus states;
- meaningful link text;
- no information conveyed only by color.

## 9. Files to change

- `index.html` — major content and information-architecture rewrite
- `styles.css` — case-study, reasoning-flow, and hierarchy styles
- `resume.html` — positioning and evidence-led CV rewrite
- `README.md` — repository description and portfolio rationale

No JavaScript is required for the initial redesign.

## 10. Content boundaries

The public portfolio must not include:
- client/customer names unless already intentionally public and safe;
- internal identifiers;
- private Slack channels;
- credentials;
- private company data;
- confidential counts that reveal operations unnecessarily;
- proprietary source code from private projects;
- internal employee details.

Generalized architecture and reasoning patterns are allowed.

## 11. Acceptance criteria

The redesign is successful when:

1. The hero does not make Karan look primarily like an engineer or operations specialist.
2. A reader can understand the multidirectional reasoning model before reaching the tools section.
3. Chuck and PYXS demonstrate thinking through concrete problem evolution, not just technology stacks.
4. Company research appears as a serious capability and not a footnote.
5. Intrader is visibly secondary and labeled as a side project.
6. The CV remains truthful to formal experience while showing broader capability.
7. No confidential internal data is published.
8. The site remains static, responsive, accessible, and deployable through the existing GitHub Pages workflow.

## 12. Non-goals

This redesign will not:
- invent achievements or performance metrics;
- claim formal roles not held;
- turn the portfolio into a trading portfolio;
- publish private project repositories or internal data;
- add unnecessary frameworks, databases, or build systems;
- optimize the site for one narrow job title.

## 13. Intended reader impression

After reading the site, the intended takeaway is:

> This person can investigate an unfamiliar problem, understand the surrounding business context, structure ambiguous information, reason across multiple disciplines, design a system, build the mechanism, test it, and revise the model when reality disagrees.
