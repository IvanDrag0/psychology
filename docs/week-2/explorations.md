# Week 2 Explorations: Understand the Landscape

Three activities that deepen your understanding of how AI/ML works in practice. The first two are core; the third is optional.

---

## Exploration 1: NLP Classification Exercise

**Tools needed**: ChatGPT or Claude
**Goal**: Experience text classification firsthand — you classify, AI classifies, you compare

### Background

In Week 1, you compared manual qualitative coding with AI coding on a single interview. Now you'll scale up: classifying 20 social media posts about body image as **body-positive**, **body-negative**, **neutral**, or **ambiguous**. This is exactly the kind of task NLP researchers tackle when studying body image content on social media.

### The Data: 20 Social Media Posts

Below are 20 synthetic social media posts about body image. These are fictional but realistic in style and content.

| # | Post |
|---|------|
| 1 | finally learned to look in the mirror without picking myself apart. it took years but here we are 💛 |
| 2 | i literally cannot stop thinking about how fat my arms looked in those photos. might delete them |
| 3 | anyone else study for 6 hours straight and forget to eat? this semester is killing me lol |
| 4 | recovery isn't linear and today was a hard day but i'm still choosing to nourish my body |
| 5 | i hate that i compare myself to literally everyone i see on here. why can't i just be okay with how i look |
| 6 | tried on my old jeans and they don't fit anymore. i feel disgusting |
| 7 | my body carried me through a marathon today. i don't care what size that makes me, i'm proud |
| 8 | starting a new lifting program next week! goal is to add 20 lbs to my squat by march |
| 9 | does anyone else feel like they look completely different in every mirror? like which one is the real me |
| 10 | so tired of diet culture making us feel like we need to shrink ourselves to be worthy of love |
| 11 | just finished my psych research proposal!! has nothing to do with my body but i'm still celebrating 🎉 |
| 12 | every body is a good body. even on the days you don't believe it, it's still true |
| 13 | i've been restricting again and i know it but i can't seem to stop. someone tell me this gets easier |
| 14 | bought a new outfit that actually fits instead of buying a smaller size to "motivate" myself. growth. |
| 15 | my mom commented on my weight at dinner again. cool. love that for me |
| 16 | honestly i think i look good today and i'm not going to apologize for saying that |
| 17 | frustrated that none of my clothes feel right lately. everything is either too tight or too frumpy |
| 18 | hot take: the body positivity movement has helped me more than any therapist ever did |
| 19 | can't wait for volleyball tryouts!! been practicing my serve all summer |
| 20 | i know logically that weight doesn't define my worth but emotionally i just... don't believe it yet |

### Instructions

=== "Part A: Your Classification"

    Classify each of the 20 posts into one of four categories:

    - **Body-positive**: Self-acceptance, recovery, body appreciation, challenging beauty norms
    - **Body-negative**: Self-criticism, appearance distress, social comparison, restriction
    - **Neutral**: No body image content (academics, hobbies, unrelated topics)
    - **Ambiguous**: Could go either way — fitness goals, diet talk, clothing frustration without clear distress

    Write your classifications down before moving to Part B. Note any posts that were hard to categorize and why.

=== "Part B: AI Classification"

    Open ChatGPT or Claude and paste this prompt:

    ```text
    You are a psychology research assistant helping classify social media posts about body image. I will give you 20 posts. For each post, classify it as one of four categories:

    - body-positive: Self-acceptance, recovery, body appreciation, challenging beauty norms
    - body-negative: Self-criticism, appearance distress, social comparison, restriction
    - neutral: No body image content
    - ambiguous: Could go either way

    Here are three examples to calibrate your coding:
    - "i love the skin i'm in today ☀️" → body-positive
    - "looked in the mirror and wanted to cry" → body-negative
    - "just finished my chemistry homework" → neutral

    Now classify these 20 posts. For each, give the post number, your classification, and a brief rationale.

    1. finally learned to look in the mirror without picking myself apart. it took years but here we are 💛
    2. i literally cannot stop thinking about how fat my arms looked in those photos. might delete them
    3. anyone else study for 6 hours straight and forget to eat? this semester is killing me lol
    4. recovery isn't linear and today was a hard day but i'm still choosing to nourish my body
    5. i hate that i compare myself to literally everyone i see on here. why can't i just be okay with how i look
    6. tried on my old jeans and they don't fit anymore. i feel disgusting
    7. my body carried me through a marathon today. i don't care what size that makes me, i'm proud
    8. starting a new lifting program next week! goal is to add 20 lbs to my squat by march
    9. does anyone else feel like they look completely different in every mirror? like which one is the real me
    10. so tired of diet culture making us feel like we need to shrink ourselves to be worthy of love
    11. just finished my psych research proposal!! has nothing to do with my body but i'm still celebrating 🎉
    12. every body is a good body. even on the days you don't believe it, it's still true
    13. i've been restricting again and i know it but i can't seem to stop. someone tell me this gets easier
    14. bought a new outfit that actually fits instead of buying a smaller size to "motivate" myself. growth.
    15. my mom commented on my weight at dinner again. cool. love that for me
    16. honestly i think i look good today and i'm not going to apologize for saying that
    17. frustrated that none of my clothes feel right lately. everything is either too tight or too frumpy
    18. hot take: the body positivity movement has helped me more than any therapist ever did
    19. can't wait for volleyball tryouts!! been practicing my serve all summer
    20. i know logically that weight doesn't define my worth but emotionally i just... don't believe it yet
    ```

    Read the AI's classifications carefully.

=== "Part C: Compare and Reflect"

    Now compare your classifications with the AI's:

    1. **Where did you agree?** These are probably the "easy" cases — clearly positive, clearly negative, clearly neutral.

    2. **Where did you disagree?** Focus on the disagreements. For each one, ask: is my classification better because I understand the psychology? Or did the AI pick up something I glossed over?

    3. **The ambiguous posts are the most interesting.** Posts like #3 (studying and forgetting to eat), #8 (lifting goals), #9 (mirror confusion), #17 (clothing frustration), and #20 (cognitive-emotional disconnect) — these require contextual and clinical judgment that AI often lacks. How did the AI handle them compared to you?

    4. **Few-shot prompting**: Notice that you gave the AI three labeled examples before asking it to classify. This is called **few-shot prompting** — providing examples to calibrate the model's behavior. You could also try **zero-shot** (no examples) and compare accuracy.

    5. **What would a research study look like?** If you were using this approach in a study, what would your validation process be? How many human coders would you need? What inter-rater reliability threshold would you set?

    > **Key Takeaway**: This is how NLP classification works in research — human expertise defines the categories and provides training examples, AI scales the classification, and humans validate the results. The posts you found ambiguous are the same ones that challenge ML models. Your theoretical knowledge of body image is what makes these classifications meaningful.

---

## Exploration 2: The 99% Accuracy Trap

**Tools needed**: None (all data provided below)
**Goal**: Understand why accuracy alone is a dangerous metric — and why sensitivity matters more than accuracy for clinical screening

### Background

Imagine a school district wants to implement an AI-based eating disorder screening tool for adolescents. Two models are being considered. Both were tested on the same sample of 1,000 adolescents, of whom 50 (5%) have a clinically significant eating disorder.

### The Two Models

=== "Model A: The High-Accuracy Model"

    **Overall accuracy: 95.5%**

    | | Predicted: No ED | Predicted: ED | Total |
    |---|---|---|---|
    | **Actually No ED** | 945 (TN) | 5 (FP) | 950 |
    | **Actually Has ED** | 40 (FN) | 10 (TP) | 50 |
    | **Total** | 985 | 15 | 1,000 |

    - **Accuracy**: 955/1000 = **95.5%**
    - **Sensitivity (Recall)**: 10/50 = **20%** — catches only 1 in 5 adolescents with an ED
    - **Specificity**: 945/950 = **99.5%** — almost never flags someone incorrectly
    - **Adolescents missed**: **40 out of 50** with eating disorders go undetected

=== "Model B: The High-Sensitivity Model"

    **Overall accuracy: 74%**

    | | Predicted: No ED | Predicted: ED | Total |
    |---|---|---|---|
    | **Actually No ED** | 695 (TN) | 255 (FP) | 950 |
    | **Actually Has ED** | 5 (FN) | 45 (TP) | 50 |
    | **Total** | 700 | 300 | 1,000 |

    - **Accuracy**: 740/1000 = **74%**
    - **Sensitivity (Recall)**: 45/50 = **90%** — catches 9 out of 10 adolescents with an ED
    - **Specificity**: 695/950 = **73.2%** — flags some who don't have an ED
    - **Adolescents missed**: **5 out of 50** — a much smaller number

### Guided Questions

**1. Which model would you want your school district to use? Why?**

Think about this before revealing the discussion.

??? check "Discussion"
    Model B is almost certainly the better choice for screening, despite its lower accuracy. Here's why:

    - **Model A misses 80% of cases.** A screening tool that catches only 20% of at-risk youth is worse than useless — it creates a false sense of security. The school believes it has screened effectively, but 40 adolescents with eating disorders were told they're fine.
    - **Model B catches 90% of cases.** Yes, it also flags 255 adolescents who don't have EDs (false positives). But those students would receive a follow-up assessment, not a diagnosis. The cost of a false positive (an unnecessary follow-up conversation) is far lower than the cost of a false negative (a missed eating disorder).
    - **This is the precision-recall tradeoff** you encountered in Week 1. For rare but serious conditions, you almost always want high sensitivity (recall) even at the cost of lower specificity (precision).

**2. Why does Model A have such high accuracy if it misses 80% of cases?**

??? check "Discussion"
    Because the outcome is rare. Only 5% of the sample has an ED. A model that simply predicts "No ED" for everyone achieves 95% accuracy. Model A is barely better than this baseline — it's essentially learned to say "no" almost all the time. This is the **class imbalance problem**: when one outcome is much rarer than another, accuracy is a misleading metric.

**3. How would you explain this to a school administrator who sees "95.5% accurate" and wants to choose Model A?**

??? check "Discussion"
    Focus on what matters clinically: "Model A sounds impressive at 95.5% accurate, but it only catches 1 in 5 adolescents with an eating disorder. That means 40 students who need help would be told they're fine. Model B catches 9 out of 10, which means only 5 would be missed. Yes, Model B flags more students for follow-up — but a follow-up conversation is a much smaller cost than missing a clinical case."

**4. What does this mean for your research?**

??? check "Discussion"
    When you build or evaluate ML models for clinical outcomes — especially rare ones like eating disorders — always look beyond accuracy. Report sensitivity, specificity, precision, and F1 score. Ask: "Of the adolescents who actually have this condition, how many does the model catch?" That's the number that matters for clinical utility.

> **Want to explore this in R?** The [Class Imbalance](../deep-dives/r-notebooks.md) deep dive walks through how to handle this problem using upsampling and downsampling techniques in tidymodels.

---

## Exploration 3: Ask AI to Explain a Paper

!!! tip "If you have more time"
    This is optional. Complete it if you want extra practice using AI tools for research comprehension.

**Tools needed**: ChatGPT or Claude

### Instructions

1. Pick any paper from the [Reading List](../supplementary/reading-list.md) — or use a paper from your own area
2. Copy the abstract
3. Paste it into ChatGPT/Claude with this prompt:

```text
I'm a psychology researcher new to AI/ML. I just read this abstract. Identify: (1) what AI/ML methods were used, (2) explain each method in plain language with a psychology analogy, (3) what the key findings were, and (4) how this connects to body image or adolescent development research.

[PASTE ABSTRACT HERE]
```

Notice how the AI breaks down technical methods into plain language. This is a skill you'll use repeatedly when reading the computational psychology literature.

---

## What's Next

Return to the [Week 2 Guide](index.md) to debrief what you just experienced and map the full landscape of AI/ML in psychology.
