# Session 1: Foundations

## Going Beyond Chat

Jan 23 · Luis & Zoe

---
# You will be part of the first wave of AI-enabled lawyers.

LV: 

this is a clinic, not a lecture. We’re here to experiment. “This doesn’t work” is a valid outcome. Your intuitions are good and valid.

---
# Intros: Zoe + Luis
Introduce ourselves briefly—perspectives from in-house/transactional and appellate clinic work.

---

# Intros: You

## What have you already tried with AI?
## What worked? What didn’t?

Z:

Round-robin: all students introduce themselves and respond to these cues. Note that some students will have done a lot, some almost nothing. Both are fine. (Even abstaining is fine, though seems unlikely!)

---

# Part 1

## What Lawyers Actually Do With AI

L: 

We’re assuming you’ve all chatted with an LLM. Today we’re going beyond that—what does it look like when AI becomes a tool, not just a conversation?

---

# Chat vs. Tool

	- "One-shot" prompts vs. structured workflows
	- Producing work vs. checking work
	- Asking questions vs. creating methodology

L:

If you take away only one thing from this class, it might be this: there is a big difference between telling a chat bot “write me a memo” and building habits and processes that you can _trust_.

Frankly, this is not stuff any lawyer has perfect intuition for yet - one way to think about this class is what it will take to make you comfortable articulating this difference and knowing when to do which.

TODO: use the fact-checking prompt as an example?

---

# Demo: The chat-structure gap

L: 

Pick a simple legal task. Show naive prompting first—get the plausible-but-wrong answer. Then show a more structured approach. Let students see failure modes in real time.

---

# Real examples from practice

L+Z each share 2-3 examples from their actual work.

TODO: list the examples for pre-discussion between Z and L.

---

# Discussion

## Think of a task from clinic, internship, or class.

## Where did you spend time on something repetitive?

## Where did a second set of eyes catch mistakes?

Z: 

TODO: I like the gist of this exercise, but worry that 

TODO Proposal: Think-pair-share format: 1 minute to think, 2 minutes with a neighbor, then a few pairs share out. We’re planting seeds for what’s “automatable” vs. what needs human judgment.

---

# Part 2

## Dissecting a “Superprompt”

L: 

We just saw the gap between naive prompting and something more structured. Now let’s look at what “more structured” can look like—someone else’s solution to a similar problem.

---

# Deep Background

## Mike Caulfield’s fact-checking prompt

A lengthy instruction set that transforms an LLM from “confident bullshitter” into “self-critical research assistant.”

L introduces. Caulfield is a digital literacy researcher. This prompt is freely available at checkplease.neocities.org. We’re going to look at *why* it works.

---

# What problems is it solving?

- LLMs don’t distinguish strong from weak evidence
- “Is this true?” gets confident answers, not rigorous analysis
- Users need to see the work, not just conclusions

L explains. This is the same problem you’ll face in legal work—you need to verify, not just accept.

TODO: mention that "don't distinguish strong from weak evidence" is something Z will go into in more detail as we discuss probability?

---

# How it works

- Forces the LLM to show its work
- Makes it argue against itself
- Encodes expert methodology as instructions

Zoe takes over. Walk through key sections: evidence type taxonomy, confidence ratings, the “preview four searches, critique how they might bias results” move. This is computational thinking in action.

---

# The key insight

## The gap between “what experts do” and “what we’d naively ask AI to do” is where the interesting work lives.

Zoe emphasizes. This is the theme of the whole course. Expert knowledge is often tacit—making it explicit and executable is the skill we’re building.

---

# Discussion

## What would an IRAC version of this look like?

## What steps would you encode for memo writing?

## Where would you force the AI to argue against itself?

Zoe facilitates. Think-pair-share. For students on journals: what would a cite-checking prompt look like? What’s your actual process for verification?

---

# Part 3

## How This Stuff Actually Works

Luis transitions. We’ve seen what structured prompting looks like. Now let’s build some intuition for *why* LLMs behave the way they do—so you can predict when they’ll help and when they’ll fail.

---

# Intuition, not math

You don’t need to understand the engineering.

You do need mental models for when to trust the output.

Luis frames this section. We’re going for “useful intuition,” not technical depth. If you want to go deeper, there are resources—but this isn’t required.

---

# What’s a language model doing?

## Prediction, not reasoning.

Luis explains. The model is predicting “what text comes next” based on patterns. It’s not “thinking through” the problem the way you would. This is why plausible-sounding wrong answers are so common.

---

# Why hallucination?

## Plausible > True

Luis continues. The model optimizes for “sounds right,” not “is right.” It has no separate fact-checking module. This is a feature of the architecture, not a bug to be fixed.

---

# “Knows” vs. “Retrieves”

## RAG vs. pure reasoning

Zoe explains. Some systems retrieve from verified databases, some reason from training data. Huge difference for legal work. The Deep Background prompt works partly by forcing retrieval behavior.

---

# Why context matters

## “Just ask it” often isn’t enough.

Zoe continues. What you put in the prompt shapes what comes out. Structured prompts work because they shape the context. This is why we’re spending a whole course on it.

---

# Discussion

## Given how these systems work:

## What legal tasks would they be good at?

## What would they be bad at?

Luis facilitates. Quick poll or think-pair-share. Draw out: pattern-matching tasks vs. novel reasoning, drafting vs. verification, high-volume vs. high-stakes.

---

# Part 4

## The Competence Obligation

Zoe transitions. Everything we’ve discussed isn’t optional. There’s a professional responsibility dimension here.

---

# CA Rule 1.1

## “…the duty to keep abreast of changes in the law and its practice, including the benefits and risks associated with relevant technology.”

Zoe reads and unpacks. This language was added deliberately. It’s not just “you can use tech”—it’s “you must understand what you’re using.”

---

# What does competence mean when tools change monthly?

Zoe continues. The State Bar’s AI guidance is a starting point, not an answer. The tools will change faster than guidance can keep up. That’s why we’re teaching judgment, not just tool operation.

---

# Discussion

## Is using AI malpractice?

## Is *not* using AI malpractice?

## Where’s the line—and who decides?

Luis facilitates. This is genuinely unsettled. Draw out the tension. No right answer yet, but students need to be thinking about it.

---

# Part 5

## Project 1: Tool Evaluation

Luis transitions. Time to get hands-on. You’re going to evaluate AI tools the way you’d evaluate them in practice—rigorously, skeptically, with your name on the work.

---

# The framing

## Your supervising partner asks you to take a first pass at a task.

## You have access to AI tools. Use them.

## But remember: your name is on the work product.

Luis explains. This is the real scenario. You’re not just “playing with AI”—you’re assessing whether and how to use it professionally.

---

# Choose your track

- A: Access-to-Justice Tool Evaluation
- B: Transactional / Contracts
- C: Litigation / Research
- D: Client-facing / Intake

Luis walks through options briefly. Pick based on career interest. All tracks teach the same core skill; the domain differs.

---

# Evaluation framework

- Accuracy & reliability
- Security & privacy
- Ethical boundaries (UPL, privilege)
- Methodology (RAG vs. reasoning)

Zoe walks through. These aren’t just “nice to check”—they’re what competent use requires. Your deliverable will address each.

---

# “This doesn’t work” is a valid outcome.

Luis emphasizes. We’re not asking you to prove the tools are good. We’re asking you to find out. Discovering failure modes is valuable.

---

# Hands-on time

Pick your track. Start exploring tools.

We’re here to help.

Luis and Zoe circulate. Help with tool access, answer questions, troubleshoot. Students should leave having started, not just having heard about the assignment.

---

# Wrap-up

---

# Logistics

- Tool access: [details TBD]
- Collaboration: encouraged
- Questions: [contact info]

Luis covers logistics quickly.

---

# Next session

## Project 1 due

## We’ll debrief and start breaking down legal processes into executable steps.

Zoe previews Session 2. The debrief will be a real discussion of what worked and what didn’t—come ready to share.

---

# Pass/fail means: experiment freely.

Luis closes. The grading structure is deliberate. Take risks. Try things. Learning from failure is the point.

---

# Questions?

Both instructors available.