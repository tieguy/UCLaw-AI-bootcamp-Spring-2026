# Assignment Brainstorm

Working document to validate course structure through concrete assignment design.

## Project 1: Tool Evaluation

**Core task**: Simulate a task you might face in your first year of practice. Use at least two AI tools, then verify the output against primary sources.

**Framing**: "Your supervising partner asks you to take a first pass at [task]. You have access to AI tools. Use them—but remember, your name is on the work product."

### Students choose based on career interest:

**Transactional / Contracts track**
Review a vendor agreement or NDA with embedded issues (one-sided indemnity, problematic IP assignment, missing limitation of liability). Use two or more tools to identify issues. Then verify: pull the relevant UCC provisions or case law that support your redlines.

**Litigation track**
Research a focused legal question (e.g., "Under California law, can a commercial landlord require a tenant to waive jury trial rights?"). Use two or more tools. Then verify: confirm every cited case exists, check that holdings are accurately described, identify any gaps.

**Client-facing / Access to justice track**
Process a realistic intake inquiry (messy, emotional, multiple potential claims). Use two or more tools to identify potential claims, flag missing information, and draft a follow-up. Then verify: are the legal theories actually viable? Did the tools miss obvious issues?

**Deliverable**: 1-2 page reflection covering:
- What each tool caught, missed, or got wrong
- How you verified the output
- How confident you'd be presenting this to a supervisor
- What you'd do differently next time

---

## Project 2: Playbook Encoding

**Core task**: Take an existing human checklist and make it AI-executable.

### Option A: Ken Adams Lite
Provide 10-15 rules from Ken Adams' *Manual of Style for Contract Drafting* (e.g., "avoid 'shall' for obligations on parties other than the subject," "use 'states' not 'provides' when referring to what a contract says"). Students encode these as prompts or instructions that an LLM can apply to a sample contract.

**Test it**: Run their encoded instructions against a deliberately flawed contract. Does the AI catch what Ken Adams would catch?

*Source materials*: Ken Adams' book is published and citable; we can excerpt rules. Sample flawed contracts can be synthetic.

### Option B: Due Diligence Checklist
Provide a standard M&A due diligence checklist (corporate records, material contracts, litigation, IP, etc.). Students translate it into instructions an AI can use to review a mock data room index.

**The gap revealed**: The checklist says "review all material contracts"—but what makes a contract "material"? Students discover what's implicit in human checklists.

*Source materials — NEED TO FIND*:
- Are there data rooms exposed through litigation? (SEC filings sometimes include data room indices in merger litigation; Delaware Chancery appraisal cases?)
- Academic simulations? (Possible: transactional lawyering clinics at other schools may have created synthetic ones)
- Could we create a synthetic data room index? (Less realistic but controllable)

### Option C: Deposition Prep Checklist
Source a litigation deposition prep checklist. Students encode it so an AI can help prepare for deposing a specific witness (provide a case fact pattern).

*Source materials — NEED TO FIND*:
- NITA or similar publishers have case files for trial advocacy courses—could we license one?
- Public case files from high-profile litigation? (Enron, Theranos depositions are partially public)
- Zoe's clinic may have sanitized examples from appellate work?

---

## Project 3: Workflow Design

**Core task**: Design a new AI-augmented process from scratch for a repetitive legal task.

### Option A: First-Draft Motion to Compel
Design a workflow that takes: (1) discovery requests served, (2) responses received, (3) meet-and-confer correspondence → and produces a first draft motion to compel with specific deficiencies called out.

**Considerations**: What does the human review at each step? Where are the hallucination risks? What verification is needed?

### Option B: Inbound Sales Contract Negotiation
Design a workflow for reviewing and negotiating inbound sales contracts (customer paper). Given a customer's contract and your company's standard positions, the workflow should: identify deviations from standard, flag high-risk terms, suggest redlines, and draft negotiation talking points.

**Considerations**: How do you encode "company standard positions"? What's the handoff to the human negotiator? How do you handle novel terms the playbook doesn't anticipate?

*Source materials*: Luis/Tal can source realistic (sanitized) inbound contracts and company position guides.

### Option C: Open Source License Analysis
Design a workflow for analyzing a codebase's open source dependencies and license obligations. The workflow should: identify dependencies, map to licenses, flag copyleft or problematic licenses, and surface attribution requirements.

**Considerations**: How do you handle license ambiguity (e.g., dual-licensed packages)? What's the verification step? How do you present risk to a non-technical stakeholder?

*Source materials*: Luis and Tal can advise; public GitHub repos provide endless realistic examples.

### Option D: Legal Research Memo Pipeline
Design a multi-step workflow: issue → initial research → verify citations → organize by relevance → draft memo.

**Considerations**: Where should a human intervene? What are the handoff points? How do you build in citation verification?

*Note*: This option overlaps somewhat with Project 1's research track—might be better suited for students who didn't choose that track initially.

---

## Project 4: Strategic Decision

**Core task**: Given a complex workflow, decide whether to use existing tool, create custom playbook, or commission software. Justify considering costs, capabilities, and ethics.

### Option A: Small Firm Scenario
You're a 5-attorney plaintiff's employment firm. You handle 40-60 active matters, mostly single-plaintiff discrimination and wage/hour. You currently use Clio for practice management and Westlaw for research. A partner asks you to evaluate whether the firm should:
- Subscribe to a legal AI tool ($500-2000/month)
- Build custom Claude/GPT playbooks for intake and demand letters
- Keep doing things manually

**Deliverable**: 2-3 page memo with recommendation and reasoning. Consider: cost, capability, privilege risks, time investment, what happens when the tool breaks.

### Option B: In-House Dilemma
You're the first legal ops hire at a 50-person startup. GC asks you to figure out how to handle the flood of vendor NDAs and procurement contracts. Options:
- Adopt a contract management platform with AI review
- Build internal playbooks using enterprise Claude/GPT
- Outsource to an ALSP with AI capabilities
- Some hybrid

**Deliverable**: Decision memo addressing build/buy/outsource tradeoffs.

### Option C: Litigation Support Build-Out
Mid-size litigation firm is considering investing in AI-assisted document review for discovery. Evaluate:
- TAR/CAL platforms (Relativity, etc.)
- General-purpose LLM approaches
- Hybrid human/AI workflows

**Deliverable**: Recommendation with ethical considerations (privilege, competence, proportionality).


## Cross-Cutting Questions

### Project 3/4 Order — Should We Swap?

Current order:
- **Project 3** (Session 4-5): Design a workflow
- **Project 4** (Session 5-6): Strategic build/buy/commission decision

Swapped order:
- **Project 3** (Session 4-5): Strategic decision (evaluative)
- **Project 4** (Session 5-6): Workflow design (generative, capstone demo)

**Arguments for swapping**:
- Strategic thinking ("should we build this?") is logically prior to detailed design ("how do we build this?")
- Students understand the landscape of options before committing effort to one approach
- Capstone becomes a *demonstration* of something built, which is more engaging than defending a decision memo
- Mirrors real-world sequence: evaluate options → pick one → execute

**Arguments against swapping**:
- Students need to have *tried* building a workflow to really understand the build/buy tradeoff
- Current order lets Project 3 be exploratory ("design this") and Project 4 be integrative ("now that you've tried it, what would you recommend?")

**Syllabus impact if swapped**:
- Session 4 would introduce Strategic Decision (currently Project 4 content)
- Session 5 would introduce Workflow Design (currently Project 3 content), with emphasis on multi-step/multi-agent coordination
- Session 6 capstone would feature workflow demos rather than decision presentations

This is a moderate rework—mostly reordering content rather than creating new content. The main change is that Session 5 (Building Robust AI Workflows) would need to do more heavy lifting on workflow design instruction, since it would be introducing the capstone project rather than building on Project 3.

**Tentative recommendation**: Swap them. The capstone-as-demo is more compelling, and strategic framing before detailed work makes pedagogical sense.

### Other Open Questions

1. **Scaffolding**: Should we provide more structure for early projects (templates, rubrics) and less for later ones?

2. **Sourcing materials**: Summary of needs:
   - Project 1: Contracts with embedded issues (can be synthetic), intake emails (Zoe's clinic?), research questions (can create)
   - Project 2: Ken Adams excerpts (published), data room index (need to find), deposition fact pattern (NITA or public cases)
   - Project 3/4: Inbound sales contracts (Luis/Tal), open source repos (public), discovery docs (need to find or synthesize)

3. **Peer review**: Should any projects include peer feedback as part of the workflow (mirroring real practice)?

4. **Failure-friendly framing**: How do we make clear that discovering "this doesn't work" is a valid and valuable outcome?

5. **Career track flexibility**: Project 1 now explicitly offers tracks. Should later projects also offer career-aligned options, or should everyone converge on shared experiences?

## Tools to Request from School

We should request access to tools that appear across multiple assignments. Candidates:

**General-purpose LLMs** (definitely need)
- Claude (Pro or Team)
- ChatGPT (Plus or Team)
- Possibly Gemini or Copilot for comparison

**Legal research**
- Westlaw AI / Lexis+ AI features (likely already have institutional access)
- CoCounsel (Thomson Reuters) — would need to request
- Vincent AI or similar

**Contract review**
- Spellbook
- Harvey (may be hard to get academic access)
- Ironclad AI

**Practice management / workflow**
- Clio (has AI features now)
- Other practice management with AI integration

**Document review / discovery**
- Relativity (for Project 3/4 discovery scenarios)

*Decision needed*: Do we standardize on 2-3 tools everyone uses, or let students pick from an approved list?

