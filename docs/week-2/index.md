# Week 2: Understand the Landscape

**By the end of this week, you will be able to:**

- Describe how NLP is being used in psychology research, particularly in therapy analysis and social media studies
- Explain the logic of predictive modeling for clinical outcomes and why it matters
- Understand how EMA and digital phenotyping combine with ML methods
- Discuss AI-assisted assessment and intervention, including recent work in eating disorders
- Articulate key ethical issues around AI/ML in psychology — especially with youth populations

---

## Start Here

!!! example "Start Here: Explorations 1 and 2"
    Before reading the guide, complete these two hands-on activities:

    1. **[Exploration 1: NLP Classification Exercise](explorations.md#exploration-1-nlp-classification-exercise)** — Classify 20 social media posts alongside an AI model
    2. **[Exploration 2: The 99% Accuracy Trap](explorations.md#exploration-2-the-99-accuracy-trap)** — Discover why accuracy alone is dangerous for clinical screening

    Come back here when you're done.

---

## What You Just Learned

Welcome back. Let's debrief the two exercises.

**From the NLP classification exercise**, you experienced how text classification works in practice — human defines categories, provides examples, AI scales the classification, human validates. The posts you found ambiguous (fitness goals, clothing frustration, cognitive-emotional disconnect) are exactly the cases that challenge ML models. This is where your expertise is irreplaceable.

**From the accuracy trap**, you learned that a 95.5% accurate model can be clinically useless when it misses 80% of the cases that matter. This is the **class imbalance problem** — and it's pervasive in clinical psychology research where the outcomes we care about most (eating disorders, suicide risk, treatment dropout) are relatively rare.

These two lessons map directly onto the landscape you're about to explore.

---

## The Landscape: 5 Areas Where AI/ML Is Transforming Psychology

???+ note "1. NLP in Psychology Research"

    Natural Language Processing is one of the most immediately relevant AI/ML areas for psychology researchers. If you work with any kind of text data, NLP is the bridge between your qualitative expertise and computational scale.

    **Therapy Session Analysis**: NLP models detect patterns in therapist and client language — mirroring, emotional attunement, topic avoidance — that predict alliance quality and treatment outcomes.

    **Social Media Analysis**: Researchers use NLP to analyze millions of posts, identifying linguistic patterns associated with body dissatisfaction, thin-ideal promotion, and body-positive messaging.

    **Automated Qualitative Coding**: Topic modeling algorithms identify recurring themes across hundreds of transcripts. LLMs (GPT-4, Claude) can serve as qualitative coders with zero-shot or few-shot prompting — achieving inter-rater reliability comparable to trained RAs for many tasks.

    !!! abstract "Paper Spotlight: Norris, Obeid, & El Emam (2024)"
        "Examining the role of artificial intelligence to advance knowledge and address barriers to research in eating disorders" (*International Journal of Eating Disorders*). Provides a comprehensive map of how AI is being applied in eating disorder research, including data sharing, data augmentation, and addressing research barriers.

???+ note "2. Predictive Modeling for Clinical Outcomes"

    Traditional psychology asks: "Which factors are **associated** with this outcome?" Predictive modeling asks: "Can we **predict** this individual's outcome?"

    This isn't just a statistical distinction:

    - **Identification**: Flagging individuals at highest risk before symptoms emerge
    - **Resource allocation**: Directing intervention to those who need it most
    - **Personalization**: Predicting which treatment will work best for a specific individual

    !!! abstract "Paper Spotlight: McClure et al. (2025)"
        "Machine-Learning Applications in Eating-Disorder-Outcome Prediction: A Systematic Scoping Review" (*Clinical Psychological Science*). Reviewed 75 studies using ML for ED outcome prediction. Decision trees, random forests, and SVMs were the most commonly used models.

???+ note "3. EMA and Digital Phenotyping"

    **Ecological Momentary Assessment (EMA)** generates intensive longitudinal data — many observations per person, many variables per observation. ML methods can detect nonlinear within-person patterns and person-specific trigger profiles that traditional methods miss.

    **Digital phenotyping** extends EMA by capturing data passively: screen time, app usage, social media engagement, sleep patterns, physical activity. Imagine tracking an adolescent's Instagram usage patterns and relating them to body image fluctuations captured through EMA — that's the promise.

???+ note "4. AI-Assisted Assessment and Intervention"

    AI is being integrated into clinical tools:

    - **Computer-Adaptive Testing (CAT)**: Assessment that adapts in real time based on responses
    - **AI-Assisted Screening**: ML models combining multiple data sources to flag at-risk individuals (the accuracy trap exercise showed why sensitivity matters here)
    - **Chatbot Interventions**: AI-powered agents delivering psychoeducation and monitoring — extending clinical reach to adolescents who may not seek traditional treatment

    !!! abstract "Paper Spotlight: Monaco et al. (2024)"
        "An advanced Artificial Intelligence platform for a personalised treatment of Eating Disorders" (*Frontiers in Psychiatry*). Describes an AI platform for ED treatment that integrates clinical assessments, demographics, and physiological data to personalize treatment plans and predict relapse.

???+ note "5. LLMs as Research Tools"

    Large language models are being used as research instruments — not just writing assistants:

    - Qualitative coding with zero-shot and few-shot prompting (what you did in Week 1)
    - Literature synthesis and research brainstorming
    - Generating synthetic data for method development
    - Translating measures across languages

    > For a deeper exploration of this area, see the [LLMs as Research Tools](../deep-dives/llms-as-research-tools.md) deep dive.

---

## Ethics and Responsible AI

Ethics isn't just a checkbox. For a psychology researcher, it's a genuine competitive advantage. Your training in research ethics, human subjects protections, and clinical responsibility gives you a lens that many AI/ML researchers lack.

### Privacy and Data Protection

- **HIPAA**: ML models trained on clinical data must comply with privacy regulations
- **FERPA**: If working with school data, student record protections apply
- **Digital phenotyping**: Passively collected smartphone data is extraordinarily revealing. Ethical frameworks are still being developed

### Algorithmic Bias

This is critical, and directly relevant to body image research.

**How bias enters AI/ML systems**:

1. **Training data bias**: A body image classification model trained on content from thin, White women will misclassify content from women of color or plus-size individuals
2. **Label bias**: If clinical diagnoses in training data underrepresent EDs in men or people of color, the model learns those biases
3. **Feature bias**: If predictor variables encode structural inequality (e.g., neighborhood, which correlates with race), the model can perpetuate discrimination

!!! warning "Interview Tip"
    Proactively raising ethical concerns in interviews — especially algorithmic bias and its relevance to your work with diverse populations — demonstrates sophisticated thinking. Search committees are impressed by candidates who think about responsible AI.

### Consent and Minors

- Can a 13-year-old meaningfully understand that their social media data will be analyzed by an ML algorithm?
- What happens to adolescent digital phenotyping data when they turn 18?
- If an ML model flags an adolescent as high-risk, what are the clinical and ethical obligations?

### Ethics as a Differentiator

Your psychology training gives you an ethical lens that most AI researchers lack. In an interview, position yourself as someone who:

- Understands the technical potential (Week 1)
- Knows the research landscape (this week)
- Can identify ethical risks others might miss
- Brings clinical and developmental expertise to responsible AI

!!! warning "Interview Tip"
    Frame ethics as integrated, not separate: "My research on body image with adolescents means I'm especially attuned to how AI/ML tools can perpetuate harmful biases around appearance and weight — and I see addressing that as central to responsible research in this space."

---

## Self-Check

**1.** You're at a conference and someone asks what NLP could do for psychology research. Give them two specific examples from your area.

??? check "Hint"
    Pick concrete applications: automated coding of conversation transcripts, sentiment analysis of social media content, topic modeling of therapy sessions. The stronger your answer, the more specific it is to your data and questions.

**2.** A colleague says "We found that Factor X is associated with depression." Explain how a prediction-focused approach would ask a different question — and why both matter.

??? check "Hint"
    Their approach asks "which factors are associated?" (explanation). Prediction asks "can we forecast this individual's outcome?" Both matter — explanation identifies intervention targets, prediction identifies who needs intervention.

**3.** You're reviewing a paper that reports 97% accuracy for an eating disorder screener. What's the first question you'd ask? Why?

??? check "Hint"
    Ask about the base rate. If only 3-5% of the sample has the condition, 97% accuracy could mean the model just predicts "no" every time. For rare but serious conditions, sensitivity (recall) matters more than overall accuracy.

**4.** A search committee asks about ethical concerns with AI in your research area. What's your answer?

??? check "Hint"
    Strong answers are specific to your population and go beyond naming concerns to articulating plans. Consider: consent/assent for minors, algorithmic bias against diverse groups, privacy of digital phenotyping data, clinical obligations when models flag risk.

> **Answer sketches**: See [Self-Check Answer Keys](../deep-dives/self-check-answer-keys.md) after attempting on your own.

---

## What's Next

In **Week 3**, you'll shift from "what's out there?" to "how do I position myself?" You'll:

- Draft a 1-page research note connecting AI/ML to your work
- Build research statement language incorporating AI/ML vision
- Explore grant angles combining your expertise with AI/ML methods
- Prepare for interview questions about AI/ML

You know the language and you know the landscape. Now you'll learn to position yourself within it.

Move on to **[Week 3: Position Yourself](../week-3/index.md)** when you're ready.
