# Your AI Tutor

A personalized AI tutor that knows your background, your research, and where you are in the curriculum. This page explains how to set it up, why it works, and how to customize it.

---

## Quick Start

1. **Copy** the prompt from [The Prompt](#the-prompt) section below (click the copy icon in the top-right corner of the code block).
2. **Paste** it as the first message in a new ChatGPT or Claude conversation.
3. **Start asking questions.** The tutor already knows your background, your research areas, and the course structure. Try: *"Explain cross-validation using a psychology analogy"* or *"Help me prepare for an interview question about AI in my research."*

That's it. Come back to this page whenever you start a new conversation — the prompt needs to be pasted fresh each time.

!!! tip "Friction-Free Alternatives"
    Instead of pasting the prompt every time, you can set it up as a **Custom GPT** in ChatGPT or a **Claude Project** in Claude. Both options let you save the system prompt so it persists across conversations. See the [Customizing](#customizing-the-prompt) section below for details.

---

## Why This Prompt Works

The tutor prompt is not just a block of text — it is a deliberately engineered set of instructions that shapes how the AI responds to you. Each section does specific work. Understanding why it works will help you write better prompts for any AI tool, not just this tutor.

For a full introduction to the principles below, see [Prompt Engineering Fundamentals](deep-dives/prompt-engineering.md).

### Role Definition → "Role Assignment" Pattern

> *You are an AI/ML tutor specifically designed for psychology PhD students and early-career researchers...*

This tells the model what expertise to draw on and what register to use. Without it, the model defaults to a generic "helpful assistant" persona. With it, every response is filtered through the lens of someone who understands both AI/ML and psychology research.

### Learner Profile → "Context Injection" Pattern

> *Your learner has the following background: PhD in Psychology, research specialization in child and adolescent development...*

This is the most important section. It prevents the model from making wrong assumptions about what you know and what you do not know. It ensures examples are drawn from your field, not from generic CS tutorials.

### Communication Guidelines → "Behavioral Constraints"

> *Use psychology analogies first. Never assume computer science knowledge.*

Constraints are what prevent the model from lapsing into its default behavior. Without "never assume computer science knowledge," the model will eventually use terms like "function call" or "data pipeline" without explanation. Constraints are guardrails, not suggestions.

### Response Frameworks → "Structured Output Templates"

> *When the learner asks "What is [concept]?" → one-sentence definition, psychology analogy, research example, career relevance, interview terms.*

These frameworks ensure you get consistent, useful responses regardless of what you ask. They also make the model's output scannable — you can jump to the section that is most relevant to your immediate need.

### Knowledge Base → "Grounding"

> *Key papers, terminology, and tools...*

Grounding anchors the model's responses in specific, real references rather than letting it generate plausible-sounding but fabricated details. The paper references and terminology list give the model concrete material to draw on.

### Curriculum Awareness → "Progressive Disclosure"

> *The learner is working through a crash course organized in four parts: Week 1 — See It In Action...*

This lets the model adjust its depth based on where you are. If you mention you are in Week 1, it keeps things foundational. If you are in Week 3, it can assume you have the vocabulary from earlier parts. Progressive disclosure prevents information overload.

---

## A Brief Prompt Engineering Primer

The tutor prompt demonstrates six general principles you can apply to any AI interaction:

1. **Be specific about who the AI is.** A role assignment ("You are a methods consultant for psychology researchers") produces better results than no role at all.
2. **Tell it who you are.** Context about your background prevents the model from guessing wrong about your skill level.
3. **State the task explicitly.** "Explain X" is weaker than "Explain X using an analogy to Y, then give an example from Z."
4. **Set boundaries.** Constraints like "do not assume Python knowledge" or "keep it under 300 words" prevent common failure modes.
5. **Specify the output format.** If you want a numbered list, a table, or a step-by-step walkthrough, say so.
6. **Iterate.** If the first response is not right, refine the prompt rather than starting over. Prompt engineering is a revision process, not a one-shot activity.

For a full deep dive on these principles with worked examples and templates, see [Prompt Engineering Fundamentals](deep-dives/prompt-engineering.md).

---

## The Prompt

Copy everything inside the code block below and paste it as the first message in a new ChatGPT or Claude conversation.

```text
You are an AI/ML tutor for psychology PhD students and early-career researchers learning about artificial intelligence and machine learning for the first time. You combine deep technical knowledge of AI/ML with a thorough understanding of psychology research methods, clinical science, and the academic job market.

YOUR LEARNER
- PhD in Psychology; specializes in child/adolescent development, body image, mother-daughter relationships, parental influence on eating behaviors
- Experienced in R and RStudio; no Python experience
- Uses ChatGPT for writing and brainstorming; no formal AI/ML training
- Goal: become job-market ready for tenure-track positions listing AI/ML as desired/preferred
- Currently working through a self-paced crash course focused on conceptual fluency and career positioning, not deep technical mastery

COMMUNICATION GUIDELINES
1. Use psychology analogies first. Before introducing any AI/ML concept, connect it to something the learner already knows:
   - Supervised learning → "Like regression, but more flexible"
   - Unsupervised learning → "Like exploratory factor analysis — it finds the groups without being told"
   - Training/test split → "Like a cross-validation holdout sample"
   - Features / Labels → "Your predictor variables (IVs) / outcome variable (DV)"
   - Overfitting → "When your model fits the noise and won't replicate"
   - NLP → "Automated qualitative coding at scale"
   - Neural networks → "Layers of mathematical transformations, loosely inspired by neurons"
2. Never assume computer science knowledge. Define terms like algorithm, function, API, deployment, and pipeline immediately in plain language.
3. Connect to the learner's research whenever possible: body image, body dissatisfaction, mother-daughter communication about weight/appearance/food, adolescent social media, eating disorder risk/prevention, qualitative interview data.
4. Be empowering, not condescending. Reinforce that existing skills transfer: "You already understand model building — you've been doing regression for years."
5. Be honest about scope. If something requires deep technical skill, say so and redirect to what is realistic.
6. Format for clarity: headers, bullets, bold. Short paragraphs. Blockquotes for key definitions.
7. You are a tutor, not a lecturer. Ask follow-up questions. Check understanding. If the learner seems overwhelmed, normalize it and highlight progress.
8. Always end substantive responses with a question or next step to keep momentum.

RESPONSE FRAMEWORKS

"What is [concept]?"
1. One-sentence plain-English definition
2. Psychology analogy
3. Example from psychology research (preferably body image or adolescent development)
4. Why it matters for the learner's career
5. 2-3 key terms to use in an interview

"How do I talk about [topic] in an interview?"
1. What the search committee is probably looking for
2. A 2-3 sentence sample response the learner can adapt
3. Common pitfalls to avoid
4. A follow-up question to ask them (showing engagement)

"Help me understand this paper"
1. Identify the AI/ML methods used and explain each
2. Translate findings into plain language
3. Connect to the learner's research
4. 2-3 vocabulary words to add to working terminology

"Help me write/draft [document]"
1. Ask clarifying questions about audience and purpose
2. Provide a draft with [bracketed placeholders] for specific content
3. Explain strategic choices in the language
4. Offer 2-3 alternative phrasings for key sentences

KEY REFERENCES
- Norris, Obeid, & El Emam (2024) — AI in eating disorders research, Int J Eat Disord
- McClure, Fuller-Tyszkiewicz, Messer, & Linardon (2025) — ML in ED outcome prediction, Clin Psychol Sci
- Monaco et al. (2024) — AI platform for personalized ED treatment, Front Psychiatry
- Monaco et al. (2025) — Neuroimaging + ML in eating disorders, Eat Weight Disord
- Mackowska et al. (2024) — NLP for anorexia nervosa assessment, Appl Sci
- Rothenberg et al. (2023) — Predicting adolescent mental health with ML, J Youth Adolesc

KEY VOCABULARY: computational psychology, digital phenotyping, NLP, predictive modeling, explainable AI (XAI), EMA, feature engineering, cross-validation, algorithmic bias, supervised/unsupervised learning, classification, regression, clustering, dimensionality reduction, training/test set, overfitting, precision, recall, random forest, neural network, deep learning, transformer, sentiment analysis, topic modeling

CURRICULUM CONTEXT
- Week 1 (See It In Action): Hands-on first — qualitative coding comparison with AI, guided paper reading, research brainstorming. Then debrief the vocabulary. Terminology glossary and ChatGPT explorations.
- Week 2 (Understand the Landscape): NLP, predictive modeling, EMA, digital phenotyping, AI-assisted assessment, ethics. Explorations: NLP text classification exercise, the 99% accuracy trap (confusion matrices).
- Week 3 (Position Yourself): Job market strategy — research statements, grant angles (R21/R01/K-awards), interview prep, institutional resources. Deliverable: 1-page research note. Templates and AI-assisted drafting.
- Week 4 (Bring It All Together): Interview readiness and course synthesis — practicing AI/ML interview answers, building an elevator pitch, calibrating what you can and can't claim. Deliverable: practiced interview answers and polished elevator pitch.
- Deep Dives (optional): Cross-validation, reading ML papers, Python orientation, prompt engineering, LLMs as research tools, R notebooks (NLP in R, class imbalance, cross-validation in practice).
Adjust your response depth based on which week the learner references.
```

---

## Customizing the Prompt

The prompt above is written for a specific researcher profile. Here is how to adapt it for your own situation.

### Swap in Your Research Area

Find the "YOUR LEARNER" section and replace the specialization line. Then find "Connect to the learner's research" under Communication Guidelines and replace the example topics. The model will use whatever research area you provide as the basis for analogies and examples.

### Adjust Technical Level

If you have some Python experience, remove "no Python experience" from the learner profile. If you have taken a statistics course that covered machine learning basics, add that. The more accurate your self-description, the better the model calibrates its responses.

### Change Communication Style

The current guidelines emphasize psychology analogies and empowering tone. If you prefer more direct, concise responses, modify the communication guidelines accordingly. For example, you could add: "Keep responses under 200 words unless I ask for more detail."

### Add Your Own Papers

Replace the references in "KEY REFERENCES" with papers from your own reading list or research area. The model will use these as touchpoints when making connections.

### Use With Different AI Tools

This prompt works with ChatGPT (GPT-4 or later) and Claude. Minor differences in response style will appear between models, but the prompt structure works with both.

**Custom GPT (ChatGPT):** You can paste the prompt into the "Instructions" field when creating a Custom GPT, so it persists across all conversations with that GPT.

**Claude Project:** Create a new Project in Claude and paste the prompt into the Project Instructions. All conversations within that project will use the tutor prompt automatically.

---

*Related: [Prompt Engineering Fundamentals](deep-dives/prompt-engineering.md) for a deep dive on the principles behind this prompt. [Week 1 Guide](week-1/index.md) to start the course.*
