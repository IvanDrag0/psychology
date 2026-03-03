# Week 1 Explorations: See It In Action

Three guided activities that put you in front of AI tools before any lecture. All data is provided inline — you don't need to find anything.

---

## Exploration 1: Qualitative Coding Face-Off

**Tools needed**: ChatGPT or Claude
**Goal**: Experience how AI-based coding compares to your manual qualitative coding — and develop informed opinions about when each approach is stronger

!!! example "This is your Week 1 starting point"
    If you're coming from the guide, you were sent here first. Do this activity before reading the rest of Week 1 — the guide debriefs what you experience here.

### The Interview Excerpt

Below is a fictional but realistic excerpt from a mother-daughter interview about body image. Read it carefully.

> **Interviewer**: Can you tell me about a recent time when you and your mom talked about bodies or appearance?
>
> **Daughter (age 14, "Mia")**: Um, yeah. So we were getting ready for my cousin's wedding last month, and we went dress shopping. And my mom kept saying things like "that's not flattering" about dresses I picked, which — I mean, I know she didn't mean it in a bad way? But it felt like she was saying my body was wrong for the dress instead of the dress being wrong for me. And then she tried on her own dress and kept looking in the mirror and saying "I look huge in this" and pulling at the fabric. And I was just standing there like... if SHE thinks she looks bad, and she's way thinner than me, then what am I supposed to think about myself?
>
> **Interviewer**: How did that make you feel?
>
> **Mia**: Honestly? Kind of terrible. Like, she tells me I'm beautiful and I should love my body, but then she says all this negative stuff about her own body, which is smaller than mine. So the message I actually get is that bodies like mine — bigger bodies — are the problem. She doesn't even realize she's doing it. I think she thinks she's only talking about herself, but I'm right there hearing it.
>
> **Interviewer**: Have you ever talked to her about how that feels?
>
> **Mia**: No. Because she'd feel SO bad. She'd cry. And then I'd have to comfort her, and it would become about her feelings and not mine. So I just... keep it to myself. Sometimes I tell my friend Jade, because her mom does the same thing.

### Part A: Your Manual Coding

Before showing this to ChatGPT, **code the excerpt yourself**. On a piece of paper or in a document, identify the major themes you see. For each theme:

1. Name the theme
2. Identify which specific text supports it
3. Note any sub-themes or nuances

There's no single right answer — this is qualitative work, and your expertise shapes what you see.

**Some prompts if you need them**: What psychological processes are visible? What relational dynamics are at play? What body image constructs are represented?

### Part B: AI Coding

Open ChatGPT or Claude and paste this prompt:

```text
I'm a psychology researcher studying mother-daughter body image communication. I need you to act as a qualitative coder. Analyze the following interview excerpt and identify the major themes. For each theme, provide: (1) the theme name, (2) a brief description, (3) specific quotes from the text that support the theme, and (4) any relevant sub-themes.

Here is the excerpt:

Interviewer: Can you tell me about a recent time when you and your mom talked about bodies or appearance?

Daughter (age 14, "Mia"): Um, yeah. So we were getting ready for my cousin's wedding last month, and we went dress shopping. And my mom kept saying things like "that's not flattering" about dresses I picked, which — I mean, I know she didn't mean it in a bad way? But it felt like she was saying my body was wrong for the dress instead of the dress being wrong for me. And then she tried on her own dress and kept looking in the mirror and saying "I look huge in this" and pulling at the fabric. And I was just standing there like... if SHE thinks she looks bad, and she's way thinner than me, then what am I supposed to think about myself?

Interviewer: How did that make you feel?

Mia: Honestly? Kind of terrible. Like, she tells me I'm beautiful and I should love my body, but then she says all this negative stuff about her own body, which is smaller than mine. So the message I actually get is that bodies like mine — bigger bodies — are the problem. She doesn't even realize she's doing it. I think she thinks she's only talking about herself, but I'm right there hearing it.

Interviewer: Have you ever talked to her about how that feels?

Mia: No. Because she'd feel SO bad. She'd cry. And then I'd have to comfort her, and it would become about her feelings and not mine. So I just... keep it to myself. Sometimes I tell my friend Jade, because her mom does the same thing.
```

Read the AI's coding carefully.

### Part C: Compare and Reflect

Now compare your manual coding with the AI's coding:

1. **Overlap**: Which themes did both you and the AI identify? These likely represent the most prominent, surface-level themes.

2. **What you caught that the AI missed**: Did your psychology training help you see something the AI didn't? Look for:
    - Implicit developmental dynamics (e.g., the parentification when Mia says she'd have to comfort her mom)
    - Clinical implications (e.g., risk factors for disordered eating)
    - Relational patterns that require knowledge of attachment or family systems theory

3. **What the AI caught that you missed**: Did the AI identify any themes you overlooked? Sometimes AI finds patterns we skip because they seem obvious.

4. **Depth vs. breadth**: Which approach was deeper? Which was broader? If you had 200 transcripts instead of one, how would this comparison change?

5. **Practical implications**: If you were designing a study with 200 transcripts, how might you combine human and AI coding?

> **Key Takeaway**: AI-based coding is not a replacement for your qualitative expertise — it's a collaborator. The AI is fast and consistent but lacks the theoretical depth you bring. The most powerful approach combines both.

---

## Exploration 2: Guided Paper Reading

**Tools needed**: None (all information provided below)
**Goal**: Walk through a real ML paper in psychology and understand what the methods mean — without needing to read the full paper

### The Paper

**Rothenberg et al. (2023).** "Predicting Adolescent Mental Health Outcomes Across Cultures: A Machine Learning Approach." *Journal of Youth and Adolescence*, 52(8), 1595-1619.

### What They Did (3-Sentence Summary)

Researchers used machine learning to predict adolescent mental health outcomes across multiple cultures. They measured 79 variables at age 10 and used them to predict mental health at ages 13 and 17. They compared three ML approaches — LASSO regression, random forests, and gradient boosting — and found that models could accurately classify mental health difficulties for approximately 7 in 10 adolescents.

### Key Details

| Detail | Value |
|--------|-------|
| **Sample** | Adolescents from multiple cultural contexts |
| **Predictor variables (features)** | 79 variables measured at age 10 |
| **Outcomes predicted** | Mental health at ages 13 and 17 |
| **ML methods used** | LASSO, random forests, gradient boosting |
| **Accuracy** | ~70% (correctly classified ~7 in 10 adolescents) |
| **Key predictors** | Emotional symptoms, peer/conduct problems, stress, parental BMI, body dissatisfaction, childhood BMI |

### Guided Questions

Work through these questions. Think about each one before revealing the discussion.

**1. Why did the researchers use 79 predictor variables instead of picking a few based on theory?**

??? tip "Click to reveal"
    Traditional psychology studies typically test a small number of theoretically motivated predictors. ML takes a different approach: feed in everything that might be relevant and let the algorithm figure out which variables matter most. With 79 variables, the model can detect complex interactions and nonlinear relationships that a researcher might not hypothesize in advance. This is one of ML's key strengths — discovery-driven analysis that complements theory-driven work.

**2. What does "~70% accuracy" mean in practical terms? Is that good?**

??? tip "Click to reveal"
    70% means the model correctly identified whether an adolescent would have mental health difficulties about 7 times out of 10. Whether that's "good" depends on context. For a screening tool, 70% is a reasonable starting point — especially when predicting years into the future. Compare it to chance: if 30% of the sample has difficulties, always guessing "no difficulties" gives 70% accuracy but catches zero at-risk youth. The model's value is that it does better than this base rate for the cases that matter most.

**3. Why did they compare three different ML methods (LASSO, random forest, gradient boosting)?**

??? tip "Click to reveal"
    No single ML algorithm is best for every problem. LASSO is a regularized regression — familiar to psychologists — that automatically selects the most important variables. Random forests build hundreds of decision trees and aggregate their votes. Gradient boosting builds models sequentially, each correcting the last one's errors. Comparing all three shows which approach best captures the patterns in this specific dataset, and whether results are consistent across methods (which increases confidence in the findings).

**4. Body dissatisfaction showed up as a key predictor. What does that tell us?**

??? tip "Click to reveal"
    The fact that body dissatisfaction at age 10 predicted mental health outcomes years later — even when competing against 78 other variables — speaks to its importance as a risk factor. This is a feature importance finding: out of everything measured, the ML model identified body dissatisfaction as one of the variables that mattered most. For your research, this is a powerful data point: it computationally confirms what body image researchers have argued theoretically.

**5. How could you build on this study using your own research expertise?**

??? tip "Click to reveal"
    Several directions: (a) Use NLP to analyze how parent-child conversations about bodies predict the same outcomes — adding qualitative richness to the quantitative predictors. (b) Test whether adding mother-specific variables (maternal body talk patterns, maternal body dissatisfaction) improves prediction beyond what the 79 original variables achieved. (c) Examine whether the model performs differently for different subgroups (e.g., by gender, culture, body size) — a fairness and bias question. Your domain expertise would make any of these extensions more psychologically grounded than a purely computational approach.

> **Want the full framework?** See the [Reading ML Papers](../deep-dives/reading-ml-papers.md) deep dive for a complete guide to evaluating ML papers in psychology.

---

## Exploration 3: AI as Research Brainstorming Partner

!!! tip "If you have more time"
    This exploration is optional. Complete it if you want to generate raw material for the career documents you'll build in Week 3.

**Tools needed**: ChatGPT or Claude, plus one of your own paper abstracts (or the sample below)
**Goal**: Experience how AI can extend existing research ideas with AI/ML directions

### Instructions

#### Step 1: Choose Your Paper

Pick one of the following:

- **Option A**: An abstract from one of your own published papers or a paper in progress
- **Option B**: An abstract from a paper you admire in your research area
- **Option C**: Use this sample abstract:

> *This study examined how mothers' comments about their own bodies and their daughters' bodies predicted body dissatisfaction and disordered eating behaviors in a sample of 250 mother-daughter dyads. Daughters ranged in age from 12 to 17 years. Mothers completed measures of body talk frequency and content, body dissatisfaction, and eating behavior. Daughters completed measures of body dissatisfaction, social comparison tendency, and disordered eating symptoms. Hierarchical regression analyses revealed that maternal body talk directed at daughters' bodies was a stronger predictor of daughter body dissatisfaction than mothers' self-directed body talk, even after controlling for daughters' BMI and social comparison tendency. Results highlight the importance of maternal communication in adolescent body image development and suggest targets for prevention programs.*

#### Step 2: Paste and Prompt

Open a new ChatGPT/Claude conversation. Paste this prompt, replacing `[ABSTRACT]` with your chosen abstract:

```text
I'm a psychology researcher exploring how AI and machine learning could extend my work. Here's the abstract of one of my studies:

[ABSTRACT]

Suggest 5 ways this research could be extended or strengthened using AI/ML methods. For each suggestion: (1) describe the specific AI/ML technique, (2) explain what new questions it could answer, (3) describe what additional data might be needed, and (4) rate the feasibility for someone who knows R but is new to ML (low/medium/high).
```

#### Step 3: Go Deeper on One Idea

Pick the suggestion that excites you most and paste this follow-up:

```text
Let's dive deeper into suggestion [number]. Walk me through what this study would look like step by step — from the research question to the data collection to the analysis. Explain any AI/ML terms you use in plain language. Be specific but realistic.
```

> **Save your outputs** — you'll use these brainstormed ideas in Week 3 when you draft research statement language and brainstorm grant angles.

---

## What's Next

Return to the [Week 1 Guide](index.md) to debrief what you just experienced and build the vocabulary around it.
