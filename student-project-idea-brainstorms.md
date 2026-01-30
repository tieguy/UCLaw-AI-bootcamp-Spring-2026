# Student Project Idea Brainstorms

Potential capstone project ideas for the course. Choose based on your interests, career goals, and preferred engagement mode: **Evaluator** (audit/critique existing systems) or **Builder** (design/prototype new tools).

---

## Meta

Ethan Mollick, b-school prof, asks his students ["what makes you uniquely human" as a prompt for their capstones.](https://www.linkedin.com/posts/emollick_i-started-the-vibefounding-mba-class-where-activity-7417943251430567936-zD3Y)

This is a great way to think about LLMs, and life in general:

> 1) What are 2-3 industries or types of work in which you have deep experience?
> 2) What are 2-3 skills (broadly defined) where you would consider yourself world class? These are areas that have traditionally gained you notice among your peers or where you know you are particularly good.
> 3) What are 2-3 things outside of work that you LOVE and have knowledge about? This could be hobbies (you knit, you play a sport, you play Dungeons and Dragons, you volunteer at an assisted living home, you are an avid birdwatcher) or areas of particular interest (you are part of an internet community devoted to movies, you follow all the latest nutritional supplement news, you are really into modern art).

> Their startups had to build on these very human edges. If you are just using the knowledge and abilities inherent in the model, you aren't really using your human advantage.

What is your human edge?

---

## Featured Option: System Alignment Challenge

### How do we align AI tools not just with "law," but with *justice*?

This capstone tackles two core alignment problems:
1. **Micro-alignment**: The language we use to train AI shapes its "moral geometry"
2. **Macro-alignment**: The structural design of legal service delivery determines who gets justice

**Full details and specifications**: See [Issue #3](https://github.com/tieguy/UCLaw-AI-bootcamp-Spring-2026/issues/3)

### Track A: The Evaluator ("Wet Cement" Auditor)

**Focus**: Embeddings, language, and moral geometry

**Task**: Conduct a "Moral Embedding Audit" of a legal workflow (eviction notices, plea offers, contract terminations)

**Deliverables**:
- Jupyter Notebook with before/after vector analysis and visualizations
- Linguistic Policy Memo (5-8 pages) arguing why specific legal language must change
- Side-by-side AI outputs using "cold" vs "warm" terminology

**Skills**: Embeddings, vector similarity, data visualization, prompt engineering, statistical analysis

**Example projects**: Eviction notice bias audit, plea bargain language analysis, contract termination dignity study

### Track B: The Builder ("Alliance" Architect)

**Focus**: Service design, access, and regulatory strategy

**Task**: Prototype a "Community Justice Node"—AI tool for non-lawyer settings (library, union hall, tenant organization)

**Deliverables**:
- Working prototype with documentation (GitHub repo)
- Service design blueprint mapping human/AI handoffs
- Regulatory strategy memo (5-8 pages) defending against UPL claims
- 5-minute demo video

**Skills**: LLM API integration, prompt engineering, workflow design, UX for non-technical users, regulatory analysis

**Example projects**: Freelancer legal cooperative, tenant defense toolkit, small claims navigator

### Hybrid Option: Full Stack Alignment Architect

Build the "Alliance" tool (Track B), then run the "Wet Cement" audit (Track A) on its own internal prompts to certify it as "Justice Aligned."

**Additional deliverable**: Alignment Certification Report proving the tool's language choices align with stated values

**Why this option**: Technically rigorous (embeddings, agent design), legally sophisticated (UPL, access to justice), portfolio-ready proof of capability

---

## Practice-Oriented Scenarios

Choose an engagement mode for any scenario:

### Evaluator Mode
Audit existing AI tools or workflows, document capabilities/limitations/failure modes, recommend whether to adopt

### Builder Mode
Design and prototype a custom AI workflow or tool for the practice context, with implementation and risk mitigation plan

---

### Small Firm Practice

**Context**: 5-attorney plaintiff's employment firm (40-60 active cases). Currently: Clio + Westlaw.

**Evaluator**: Test 2-3 legal AI tools on actual intake emails and demand letter drafting. Document what works, what fails, cost-benefit analysis.

**Builder**: Design custom intake triage workflow or demand letter generation system. Prototype with quality control checkpoints.

**Key issues**: Cost vs. volume, privilege protection, time to learn/maintain, vendor lock-in

---

### In-House Legal Operations

**Context**: First legal ops hire at 50-person startup drowning in vendor NDAs and procurement contracts.

**Evaluator**: Compare contract management platforms (with AI) vs. ALSPs vs. general-purpose LLMs. Build vs. buy vs. outsource decision.

**Builder**: Prototype internal NDA review workflow with playbook encoding company positions, risk flagging, redline suggestions.

**Key issues**: Scalability, integration with existing systems, internal expertise, handoff protocols

---

### Access-to-Justice Tool

**Context**: Legal aid organization considering AI deployment for underserved populations.

**Evaluator**: Rigorously test an existing A2J tool (e.g., eviction defense, benefits eligibility). Document UPL boundaries, accuracy on edge cases, privacy risks.

**Builder**: Design community-accessible tool for specific legal need. Define clear human escalation triggers. Develop regulatory defense strategy.

**Key issues**: UPL boundaries, privacy for vulnerable populations, accuracy requirements, digital divide, liability exposure

---

### Litigation Discovery

**Context**: Mid-size firm evaluating AI-assisted document review.

**Evaluator**: Compare TAR/CAL platforms vs. general LLM approaches. Test on sample document set, measure accuracy, assess proportionality and privilege protection.

**Builder**: Design hybrid human/AI review workflow. Prototype privilege log generation or key document identification system.

**Key issues**: Proportionality, privilege, competence obligations, cost-benefit, client billing implications

---

### Solo/Small Practice Automation

**Context**: Solo practitioner (family law, estates, etc.) with limited budget, high volume.

**Evaluator**: Test general-purpose LLM subscriptions vs. legal-specific tools. Document what's worth paying for on a limited budget.

**Builder**: Design simple automation for most repetitive task (client intake, standard forms, status updates). Focus on sustainability and learning curve.

**Key issues**: Budget constraints, time to learn vs. time saved, client service quality, ethical obligations on limited resources

---

### Appellate Practice

**Context**: Appellate clinic or small appellate practice evaluating AI integration.

**Evaluator**: Test AI tools for record review, research verification, citation checking. Document when AI helps vs. hinders appellate-quality work.

**Builder**: Design workflow for one appellate task (issue spotting from record, research verification, cite-checking). Define quality thresholds.

**Key issues**: Accuracy standards for appellate work, relationship to oral argument prep, judicial expectations, record-intensive vs. legal-intensive appeals

---

## Alternative Approaches

### Deep Ethics Dive
Pick an emerging ethics issue and analyze in depth:
- Privilege in multi-tenant AI systems
- Conflicts of interest in shared legal AI tools
- Defining "competence" for AI-augmented practice
- Informed consent for AI use in client matters

**Deliverable**: Analysis memo with proposed ethical framework or rule modifications

### Tool Comparison Study
Rigorously evaluate 3+ tools on identical legal task. Document capabilities, limitations, failure modes, costs.

**Deliverable**: Comparison matrix, test results, purchase recommendation with risk assessment

### Workflow Design Sprint
Design novel AI-augmented workflow for repetitive legal task, build prototype, test with real examples, document results.

**Deliverable**: Working prototype, design documentation, evaluation report, implementation roadmap

---

## Evaluation Criteria

Strong projects demonstrate:

- **Rigor**: Nuanced analysis, not "AI good/bad"
- **Professional responsibility**: Ethics integrated throughout, not afterthought
- **Realism**: Honest cost-benefit assessment, not vendor marketing
- **Failure awareness**: What could go wrong and how to mitigate
- **Implementation thinking**: Not just "should we" but "how would we"

**"This doesn't work safely" is a valid and valuable conclusion if well-supported.**

---

## Technical Depth Options

- **Analysis-focused**: Evaluation, comparison, decision framework (requires legal research, tool testing, interview skills)
- **Build-light**: Simple workflows using existing tools, prompt engineering (requires API basics, workflow design)
- **Build-heavy**: Custom prototypes with embeddings, agents, complex workflows (requires coding, LLM APIs, technical architecture)

All depth levels are valid. Match to your technical comfort and learning goals.

---

## Getting Started

1. **Choose engagement mode**: Evaluator or Builder? (Or hybrid for ambitious projects)
2. **Select scenario**: What practice context interests you?
3. **Scope appropriately**: 3-week timeline from assignment to presentation
4. **Research landscape**: What exists? What's possible? What are the constraints?
5. **Define success criteria**: What would "done well" look like?

We'll discuss project selection and scope in Session 5 when the capstone is formally assigned.

---

## Resources

**For Evaluator tracks**:
- Tool trial access (coordinate with instructors)
- Practitioner interview connections
- Evaluation frameworks and rubrics

**For Builder tracks**:
- LLM API access (OpenAI, Anthropic, etc.)
- Sample legal text and datasets
- Technical tutorials and starter code
- Office hours for debugging and design feedback

**For System Alignment Challenge**:
- Full specifications in [Issue #3](https://github.com/tieguy/UCLaw-AI-bootcamp-Spring-2026/issues/3)
- Embeddings tutorials and baseline datasets
- UPL case law and regulatory strategy resources
- Community organization contacts for user research
