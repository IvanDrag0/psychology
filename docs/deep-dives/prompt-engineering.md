# Prompt Engineering Fundamentals

**Prerequisites**: Week 1 guide | **Type**: Deep Dive (Optional)

---

## What Prompt Engineering Actually Is

Prompt engineering is not about finding magic words that unlock hidden capabilities. It is structured communication — telling an AI system exactly what you need, in a format it can act on reliably.

If you have ever written a good survey instrument, you already understand the core skill. A well-designed questionnaire item has a clear stem, specifies the construct being measured, avoids double-barreled questions, and provides an unambiguous response format. A well-engineered prompt does the same thing: it provides context, specifies the task precisely, constrains the output, and anticipates where the model might go off track.

The difference between a vague prompt and a well-engineered one is the difference between "Tell me about body image" and a structured interview protocol with defined constructs, specific probes, and a coding scheme. Both use language. One produces usable data.

> **Key Takeaway**: Prompt engineering is methodological design applied to AI interaction. You already have the underlying skill — this page teaches you the format.

---

## Anatomy of a Good Prompt

Every effective prompt contains some combination of five components. Not every prompt needs all five, but knowing the full toolkit lets you add structure as needed. Each component has a direct analogy to something you already do in psychology research.

### 1. Role Assignment

**What it does**: Tells the AI who it is and what expertise to draw on.

**Psychology analogy**: This is like giving a research assistant their role definition before they start coding data. "You are coding for appearance-related content in mother-daughter interaction transcripts" is fundamentally different from "read these transcripts and tell me what you notice."

**Example**:

> You are a research methods consultant specializing in applied machine learning for clinical psychology. You have expertise in predictive modeling, text analysis, and study design for behavioral health research.

**Why it works**: LLMs generate text by predicting what would plausibly come next in a given context. When you assign a role, you steer the model toward the knowledge domain and communication register most useful for your task. A "methods consultant" response will look different from a "friendly tutor" response, even for the same question.

### 2. Context

**What it does**: Provides the background information the AI needs to give a relevant response.

**Psychology analogy**: This is the introduction section of a research protocol — everything a new team member needs to know before they can do their job. Without it, they are working blind.

**Example**:

> I am a psychology PhD with expertise in adolescent development and body image research. I use R for data analysis and have no Python experience. I am preparing for tenure-track job interviews at programs that value computational methods.

**Why it works**: The same question — "How should I analyze open-ended survey responses?" — has different answers depending on whether the person asking is a computer science PhD with Python fluency or a psychology researcher who works in R. Context lets the AI calibrate its response to your actual situation.

### 3. Task

**What it does**: States exactly what you want the AI to do.

**Psychology analogy**: This is the instructions section of a coding manual — the specific procedure, stated precisely enough that two different coders would do the same thing.

**Example**:

> Explain what cross-validation is and why it matters. Use an analogy to a psychology method I already know. Then give me a concrete example using body dissatisfaction data with a binary outcome (clinical vs. non-clinical).

**Why it works**: Vague tasks produce vague outputs. "Tell me about cross-validation" gives you a generic textbook summary. A specific task — with a defined audience, a requested format, and a concrete application — produces something you can actually use.

### 4. Constraints

**What it does**: Sets boundaries on what the response should and should not include.

**Psychology analogy**: These are your inclusion/exclusion criteria. Just as you would not include participants outside your age range, you do not want the AI venturing into territory that is not helpful.

**Example**:

> Do not assume I know Python. Do not use mathematical notation unless you also provide a plain-English explanation. Keep the total response under 500 words. If a concept requires deep technical background, say so and tell me what I would need to learn first.

**Why it works**: Without constraints, LLMs default to their most general response pattern. Constraints narrow the output space to what is actually useful for you. They are especially important for avoiding technical jargon, managing response length, and keeping the model honest about the limits of a simplified explanation.

### 5. Output Format

**What it does**: Specifies the structure of the response you want.

**Psychology analogy**: This is the response format on a structured assessment — if you want a Likert scale, you do not hand someone a blank page and hope they produce one.

**Example**:

> Format your response as:
> 1. One-sentence definition
> 2. Psychology analogy
> 3. Body image research example
> 4. Three key terms I should know for interviews

**Why it works**: Specifying output format makes responses consistent, scannable, and directly usable. This is especially valuable when you are asking the AI to do the same task across multiple inputs — coding 20 transcripts, summarizing 10 papers, or generating interview prep for 5 different questions.

---

## Common Patterns

Once you understand the five components, you can combine them into patterns that solve recurring problems. Here are the four most useful patterns for psychology researchers.

### Role Assignment Pattern

Assign a specific persona to shape the tone, depth, and perspective of the response.

> You are an experienced clinical psychologist who also has a strong quantitative methods background. Explain [concept] in a way that a developmental psychologist new to computational methods would understand.

**When to use it**: Whenever you need the response calibrated to a specific audience or expertise level.

### Few-Shot Example Pattern

Provide 2-5 examples of the input-output pair you want, then ask the model to continue the pattern.

> Here are three examples of how I want social media posts classified:
>
> Post: "Finally learning to love my body as it is" → Category: body-positive
> Post: "I wish I could lose 10 more pounds before summer" → Category: body-negative
> Post: "Just had coffee with friends" → Category: neutral
>
> Now classify the following post: [new text]

**When to use it**: Classification tasks, coding tasks, or any time you want consistent formatting. Few-shot prompting is the single most important technique for research applications because it operationalizes your constructs through examples rather than relying on the LLM's default understanding of your categories.

### Chain-of-Thought Pattern

Ask the model to show its reasoning step by step before giving a final answer.

> Before giving your final classification, think through the following:
> 1. What appearance-related content, if any, is present in this speaking turn?
> 2. Is the content explicit or implied?
> 3. Which code(s) from the codebook best match this content?
> 4. Final code(s) with one-sentence rationale.

**When to use it**: When accuracy matters more than speed. Chain-of-thought prompting reduces errors on tasks that require multi-step reasoning. It also makes the model's logic auditable — you can see where it went wrong and adjust accordingly.

### Structured Output Pattern

Request a specific format — a table, a numbered list, JSON, or a template — so the output is directly usable.

> Return your analysis as a markdown table with these columns:
> | Speaking Turn | Code(s) | Confidence (High/Medium/Low) | Rationale |

**When to use it**: Any time you need to compare, aggregate, or import the outputs into another tool. Structured output is essential for research-grade use of LLMs because it makes inter-rater reliability analysis possible.

---

## Iterative Refinement

Your first prompt will rarely be your best prompt. Prompt engineering is an iterative process — closer to piloting a survey instrument than to writing a final draft.

### The Revision Loop

1. **Write** your initial prompt using the five components above.
2. **Test** it on a few representative inputs.
3. **Evaluate** the outputs. Where do they match your expectations? Where do they diverge?
4. **Diagnose** the mismatches. Is the task underspecified? Are the constraints too loose? Does the model need examples?
5. **Revise** the specific component that is causing the problem.
6. **Re-test** on the same inputs to confirm improvement, then test on new inputs.

### Common Refinement Moves

| Problem | Likely Cause | Fix |
|---------|-------------|-----|
| Response is too generic | Task is underspecified | Add concrete details and examples to the task |
| Response is too technical | Missing constraints | Add "Do not assume [X] knowledge" |
| Response format varies across inputs | No output format specified | Add explicit format instructions |
| Model misinterprets your categories | Relying on zero-shot | Switch to few-shot with labeled examples |
| Response is too long | No length constraint | Add word or paragraph limits |
| Model hedges excessively | No confidence framing | Add "Be direct. State what is known and what is uncertain." |

### The Survey Instrument Analogy

Think of prompt refinement the same way you think about piloting a questionnaire:

- **Cognitive interviewing** → Reading the AI's output carefully to understand how it interpreted your instructions
- **Item revision** → Rewriting ambiguous parts of your prompt based on what the output revealed
- **Pilot testing** → Running the revised prompt on a small sample before scaling up
- **Standardization** → Locking in the final prompt and using it consistently across all inputs

The goal is the same: a standardized instrument that produces reliable, interpretable results across repeated administrations.

---

## Practical Tips for Daily Use

You do not need a research-grade prompt for everyday tasks. Here are templates for the most common uses throughout this course and your career development.

### Learning a New Concept

> I'm a psychology researcher with strong stats skills but no formal AI/ML training. Explain [concept] using an analogy to a psychology research method I already know. Then give me one concrete example using [your research area] data. Keep it under 300 words.

### Brainstorming Research Connections

> I study [your topic] using [your methods]. Generate 5 specific ways that [AI/ML technique] could extend or strengthen this research. For each idea, briefly explain what data I would need and whether it's feasible for someone whose primary language is R. Flag any ideas that would require a computational collaborator.

### Writing Assistance

> I am drafting a [research statement / grant aim / cover letter paragraph] that positions my work in [your area] as connected to AI/ML methods. Here is my draft: [paste draft]. Revise it to sound confident but honest about my current skill level. Do not overclaim — I am building toward computational work, not already doing it. Keep the same overall structure and length.

### Interview Prep

> I have a tenure-track interview at a program that values computational methods. The committee might ask: "[interview question]." Draft a 2-3 sentence response that accurately represents my background: I have conceptual fluency in AI/ML, hands-on experience with ML in R using tidymodels, and I am actively building toward a computational collaboration. I do not want to overclaim.

---

## The AI Tutor Prompt: A Worked Example

The [AI Tutor Prompt](../ai-tutor.md) that accompanies this course is itself a worked example of prompt engineering. Here is how each section maps to the components described above.

| Prompt Section | Component | What It Does |
|---------------|-----------|-------------|
| "You are an AI/ML tutor specifically designed for psychology PhD students..." | **Role Assignment** | Defines the persona and expertise the model should draw on |
| "Your learner has the following background: PhD in Psychology, research specialization in..." | **Context** | Tells the model exactly who it is talking to, so it can calibrate vocabulary and examples |
| "Use psychology analogies first. Never assume computer science knowledge." | **Constraints** | Prevents the model from defaulting to CS-native explanations |
| Response Frameworks ("What is [concept]?" → 5-step structure) | **Output Format** | Ensures consistent, structured responses for each question type |
| Key Knowledge Base (papers, R packages, terminology) | **Context** (grounding) | Anchors the model's responses in specific, accurate references |
| Curriculum Awareness (Week 1-4 descriptions) | **Context** (progressive disclosure) | Lets the model adjust its response depth based on where you are in the course |

Notice that the tutor prompt uses all five components, and each one is doing specific work. The role assignment is not decorative — it shapes every response. The constraints are not suggestions — they prevent the most common failure mode (lapsing into CS jargon). The output formats are not optional — they ensure you get responses you can actually learn from.

This is what prompt engineering looks like in practice: not tricks, but deliberate design choices that shape reliable outputs.

---

## What This Does Not Cover

This page covers the fundamentals — enough to use AI tools effectively for learning, brainstorming, writing, and career development. It does not cover research-grade prompt engineering: designing prompts for systematic coding, classification at scale, or data augmentation.

For that, see [LLMs as Research Tools](llms-as-research-tools.md), which covers:

- Qualitative coding with LLMs, including inter-rater reliability
- Zero-shot and few-shot classification for research data
- Research-grade prompt design with reproducibility requirements
- Reporting standards for LLM-assisted research

The line between "everyday prompt engineering" and "research-grade prompt engineering" is rigor. Everyday prompts need to be useful. Research prompts need to be reproducible, validated, and documented to a standard that reviewers will accept.

---

*Related modules: [LLMs as Research Tools](llms-as-research-tools.md) for research-grade prompting and LLM-assisted coding. [AI Tutor Prompt](../ai-tutor.md) for a worked example you can use immediately.*
