# Ideas for Future Iterations

This document captures enhancements and alternatives considered during Spring 2026 planning but deferred due to time, complexity, or being first-time-through. Consider these for future offerings.

---

## Practitioner Involvement

**Spring 2026 decision**: Instructor-led sessions only, no guest practitioners.

**For future consideration**: Guest speakers could reinforce specific sessions:

- **Law Firm CTO/Innovation Director** — Session 3 (practice operations, vendor evaluation, build vs. buy)
  - Could share real vendor evaluation frameworks
  - Discuss what actually works vs. vendor promises

- **Litigator** (large or mid-size firm) — Session 4 (discovery, research, privilege)
  - Real talk about AI in document review
  - Practical privilege considerations with AI tools
  - Motion practice and research verification

- **In-House/Transactional Counsel** — Session 4 (contract review, drafting, templates)
  - Luis could fill this role, or bring in another in-house perspective
  - Playbook development in practice
  - Managing legal tech stack

- **Ethics/Risk Counsel** — Session 6 (ethics, competence, conflicts)
  - Bar perspectives on AI competence
  - Real ethics opinions and disciplinary cases
  - Managing client confidentiality with cloud tools

**Implementation notes**:
- Guest speakers are supplements, not prerequisites
- Course works without them (proven Spring 2026)
- If pursuing, start outreach 3-4 months before semester
- Have backup plan if practitioners cancel

---

## Pedagogical Enhancements

### Deeper Technical Foundation

**What we did**: "Intuition without math" approach (Part 3 of Session 1, later deferred)

**Alternative for future**: More substantial technical grounding
- How transformers actually work (conceptual level)
- Training vs. inference
- Why certain architectures matter for legal work
- Understanding model capabilities from architecture

**Resources to explore**:
- Owen Astrachan (Duke) — computational thinking materials for non-CS students
- Coursera AI/ML intro courses (Zoe's original proposal referenced these)
- Anthropic's "AI Safety Fundamentals" curriculum

**Trade-off**: Deeper understanding vs. overwhelming students who just want practical skills

---

### Multi-Agent Coordination as Explicit Topic

**What we did**: Multi-agent concepts mentioned briefly in Session 5, not emphasized

**Alternative for future**: Dedicated session or extended coverage on:
- Orchestrating multiple specialized AI agents
- When single-agent vs. multi-agent makes sense
- Managing handoffs and verification between agents
- Real-world multi-agent systems in legal practice

**Requires**:
- More advanced student baseline (or earlier theoretical foundation)
- Concrete legal examples of multi-agent workflows
- Possibly a dedicated assignment

**Trade-off**: Advanced capability vs. overwhelming beginners still learning single-tool use

---

### Project Sequencing: Swap Projects 3 & 4?

**Current order**:
- Project 3 (Session 4-5): Design a workflow
- Project 4 (Session 5-6): Strategic build/buy/commission decision

**Alternative order**:
- Project 3 (Session 4-5): Strategic decision (evaluative)
- Project 4 (Session 5-6): Workflow design (generative, capstone demo)

**Arguments for swapping**:
- Strategic thinking logically precedes detailed design
- Students evaluate landscape before committing effort
- Capstone-as-demo is more engaging than decision memo presentation
- Mirrors real-world: evaluate options → pick one → execute

**Arguments against**:
- Students need to *try* building to understand build/buy tradeoffs
- Current order: exploratory design, then integrative strategic thinking
- "Here's what I learned from building" is powerful

**For future**: Test the swap and see which produces better learning outcomes

---

### Peer Review Integration

**What we did**: Instructor feedback on projects

**Alternative for future**: Build peer review into workflow
- Mirrors real practice (multiple eyes on work product)
- Teaches constructive critique
- Surfaces different approaches to same problem

**Possible implementations**:
- Project 2 or 3: peer review as required step before submission
- Anonymous peer feedback using rubrics
- In-class peer workshops for Project 4 (already partially there)

**Requires**:
- Clear rubrics and review guidelines
- Class time for review process
- Managing uneven peer feedback quality

---

## Materials and Resources

### Sourcing More Sophisticated Assignment Materials

**For Project 2** (Playbook Encoding):
- **Data room index** for due diligence exercise
  - Check SEC filings / Delaware Chancery appraisal cases for exposed data rooms
  - Academic transactional clinic simulations
  - Create synthetic (less realistic but more controlled)

- **Deposition fact pattern** for litigation prep exercise
  - NITA case files (may require licensing)
  - Public depositions from high-profile cases (Enron, Theranos)
  - Zoe's clinic sanitized examples

**For Project 3/4** (Workflow Design):
- **Discovery documents** for motion to compel workflow
  - Need realistic request/response/meet-and-confer set
  - Could synthesize or pull from public cases

- **Inbound sales contracts** for negotiation workflow
  - Luis/Tal can source (sanitized company examples)
  - Real "customer paper" with problematic terms

---

### Curated Reading List

**What we did**: Minimal readings (superprompt for Session 1, possibilities.md placeholder)

**For future**: Optional deeper readings for motivated students
- Theoretical foundations (how LLMs work)
- Ethics and professional responsibility cases
- Legal innovation and practice transformation
- Specific tool documentation and best practices
- Academic research on AI in legal practice

**Start with**:
- Anthropic's Soul Doc or summary (already in possibilities.md)
- CA State Bar AI guidance
- ABA Formal Opinions on technology competence
- Selected articles from legal tech journals

---

## Tools and Infrastructure

### Expanded Tool Access

**What we had**: General-purpose LLMs (Claude, ChatGPT)

**For future consideration**:

**Legal-specific tools** (request from school or vendors):
- **Legal research**: CoCounsel, Westlaw AI, Lexis+ AI, Vincent AI
- **Contract review**: Spellbook, Harvey, Ironclad AI
- **Practice management**: Clio with AI features
- **Document review**: Relativity (for discovery scenarios)

**Decision point**: Standardize on 2-3 tools vs. let students choose from approved list?

**Trade-offs**:
- More tools = broader exposure, fragmented class discussion
- Fewer tools = shared experience, deeper mastery, easier support

---

### Course Infrastructure

**For future**:
- Dedicated collaboration platform (Slack, Discord, etc.)
- Structured submission system
- Shared resource repository
- Tool usage tracking/analytics (if available)

---

## Format and Structure

### Compressed Bootcamp Format

**What we did**: 6 sessions spread over semester (Jan-Apr)

**Alternative explored**: Compressed 4-6 day intensive bootcamp
- Daily or every-other-day sessions
- Immersive experience with less context-switching
- Projects completed in real-time during bootcamp week

**Trade-offs**:
- Intensity and focus vs. time for experimentation between sessions
- Scheduling difficulty vs. sustained engagement
- Student capacity (other coursework) vs. deep immersion

**For future**: Possible January term or summer intensive version?

---

### Formal Capstone Presentations

**What we did**: Project 4 presentations in Session 6 (format TBD)

**Enhancement for future**:
- More structured demo format if projects are swapped
- External judges or reviewers?
- Public showcase (invite broader law school community)
- Recorded presentations for portfolio building

---

## Assessment and Scaffolding

### Progressive Scaffolding

**Question for future**: Should early projects have more structure (templates, detailed rubrics) and later projects less?

**Possible approach**:
- Project 1: Detailed evaluation framework provided
- Project 2: Template provided, students fill in
- Project 3: High-level requirements only
- Project 4: Open-ended with constraints

**Trade-off**: Support vs. independence, training wheels vs. learning to fail

---

### Failure-Friendly Framing

**For future**: Explicit mechanisms to reinforce "this doesn't work" as valid outcome
- Rubrics that reward rigorous negative findings
- Showcase projects that discovered failures
- Reflection prompts on what failed and why
- Class discussion of interesting failures

---

## Curriculum Refresh Process

**For future iterations**: Systematic approach to keeping current

**Possible approach**:
- Post-semester review with students (what tools/techniques changed)
- Quarterly scan of legal AI landscape
- Monitoring bar guidance and ethics opinions
- Staying connected with practitioners using these tools
- Budget time for significant updates between offerings

**Reality**: AI legal tools will change faster than curriculum. Teaching judgment and evaluation frameworks matters more than teaching specific tools.

---

## Cross-Cutting Decisions Still Open

- **Project 1 track structure**: Single mandatory assignment (A2J evaluation) vs. multiple career-aligned tracks?
- **Tool standardization**: Require specific tools or allow student choice?
- **Capstone format**: Written decision memo vs. workflow demo vs. both?

---

## Notes for Next Planning Cycle

- Start practitioner outreach 3-4 months early (if pursuing)
- Confirm school tool access at least 6 weeks before start
- Owen Astrachan contact for computational thinking materials
- Review and update this document after each offering with what actually worked
