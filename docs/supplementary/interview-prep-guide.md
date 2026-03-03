# Interview Preparation Guide: AI/ML Questions for Psychology Faculty Positions

This guide prepares you for the AI/ML-related questions you may encounter during tenure-track interviews in clinical and developmental psychology. It covers what search committees want, practice questions with model answers, questions to ask them, elevator pitches, and how to handle difficult moments.

---

## What Search Committees Want

### The Spectrum of Expectations

Search committees' AI/ML expectations fall on a spectrum. Understanding where a specific position falls helps you calibrate your responses:

**Level 1 — Awareness** (most common for clinical/developmental positions)
- Can you discuss AI/ML intelligently?
- Do you understand how it's relevant to psychology?
- Are you open to computational approaches?
- *Your preparation covers this fully.*

**Level 2 — Vision** (common for positions mentioning "innovative methods")
- Do you have a concrete plan for incorporating AI/ML into your research?
- Can you articulate specific projects?
- Do you know the relevant literature?
- *Your preparation covers this fully.*

**Level 3 — Experience** (positions that say "experience preferred")
- Have you done any hands-on work with ML?
- Can you discuss methodology specifics?
- Do you have preliminary results or a pilot study?
- *You have foundational experience (Week 2 explorations (NLP classification, accuracy analysis)) and can speak to your development trajectory.*

**Level 4 — Expertise** (dedicated computational methods positions)
- Is AI/ML central to your published research?
- Can you teach advanced methods courses?
- Do you have funded computational work?
- *This is beyond your current positioning — and that's fine. These positions are different hires.*

Most positions you'll apply to are Level 1-3. Your crash course positions you well for all three.

---

## Practice Questions with Model Answers

### Research Questions

#### Q1: "How does your research connect to AI and machine learning?"

**Framework**: Established work → natural bridge → specific AI/ML directions

> "My research on how maternal communication about bodies shapes adolescent body image has generated the kind of rich longitudinal and qualitative data that AI/ML methods can extend powerfully. The most immediate connection is NLP — I have hundreds of pages of mother-daughter conversation transcripts that I've coded qualitatively, and NLP methods could scale that analysis to much larger samples while identifying linguistic patterns too subtle for manual coding. I'm also exploring hands-on experience using AI tools for text classification and qualitative coding, building toward integrating the many risk factors I study — parental, peer, media, individual — into machine learning models that can predict eating disorder trajectories. And I'm excited about digital phenotyping approaches that could capture real-time relationships between social media exposure and body image in adolescent samples."

---

#### Q2: "What specific AI/ML project would you pursue first?"

**Framework**: Concrete, scoped, fundable, connected to existing work

> "My first project would be an R21 exploring NLP analysis of mother-daughter body talk. I have an existing corpus of coded conversation transcripts that could serve as training data — where my qualitative coding becomes the ground truth for the NLP model to learn from. The aim would be to establish whether NLP can reliably identify the linguistic patterns I've found manually — like appearance-focused commentary, comparison language, and hedging around weight — and then apply that automated coding to a much larger sample. If successful, this opens the door to studying mother-daughter body talk at a scale that manual coding simply can't achieve, including cross-cultural comparisons."

---

#### Q3: "Where do you see your research program in five years?"

**Framework**: Established foundation → growing computational integration → broader impact

> "In five years, I want to be running a lab that bridges clinical-developmental psychology and computational methods. My body image and family dynamics work will remain the theoretical core — that's where my expertise and unique contribution lies. But the methods will evolve. I envision combining longitudinal data collection with digital phenotyping, using machine learning to build clinically useful risk prediction models for adolescent eating disorders, and developing NLP tools specifically validated for analyzing parent-child communication about bodies. I'd also like to have established interdisciplinary collaborations with computational researchers here and be contributing to the conversation about responsible AI in youth mental health."

---

### Methods Questions

#### Q4: "What experience do you have with machine learning?"

**Framework**: Honest, specific, growth-oriented

> "I'm building my ML skills through a deliberate training plan. I've completed hands-on experience using AI tools for text classification and qualitative coding — comparing manual and AI-assisted analysis approaches, evaluating classification accuracy, and interpreting where automated methods succeed and struggle. I have a solid conceptual understanding of supervised and unsupervised learning, NLP, and predictive modeling. I'm also engaging with the computational psychology literature — papers by Norris, McClure, and others applying AI/ML to eating disorders research. I'm transparent that I'm early in this development, and I see collaboration as essential in my first few years. What I bring to those collaborations is deep domain expertise, rigorous research design training, and a clear vision for psychologically meaningful applications."

---

#### Q5: "How would you analyze text data from your mother-daughter interviews computationally?"

**Framework**: Show you understand the process, even if you'd need collaboration for implementation

> "The approach I'm working toward starts with my existing qualitative coding as the foundation. I would use my manually coded transcripts as labeled training data — the codes I've already applied become the ground truth the NLP model learns from. For implementation, I'd likely use AI-assisted text analysis and NLP tools for text preprocessing and the classification workflow. The model would learn to associate specific linguistic features — word choice, sentence structure, emotional valence, comparative language — with my thematic codes. Then I could apply that trained model to new, uncoded transcripts at scale. I'd want to validate extensively, checking the model's coding against expert human coding on a held-out set. For the NLP-specific technical work, I'd collaborate with a computational linguist, but I'd be leading the construct definition, study design, and interpretation."

---

#### Q6: "What's the difference between what you'd do with ML versus traditional statistics?"

**Framework**: Both matter, ML extends rather than replaces

> "Great question. Traditional statistical methods like regression and mixed models are essential for testing specific hypotheses about mechanisms — like whether maternal body talk predicts daughter body dissatisfaction after controlling for peer influence. I'll continue using those. Where ML adds value is in three areas. First, prediction: ML models can integrate many variables simultaneously and capture nonlinear interactions to predict who will develop clinical outcomes — which traditional methods handle less well. Second, scale: NLP allows me to analyze text data at volumes that manual coding can't reach. Third, discovery: unsupervised methods can reveal patterns and subgroups I wouldn't have hypothesized. I see these as complementary — ML generates hypotheses and builds prediction tools; traditional methods test mechanisms."

---

### Collaboration Questions

#### Q7: "How would you collaborate with our data science center / computational faculty?"

**Framework**: Clear about what you bring and what you need

> "I see myself as the domain expert in that collaboration. I bring the research questions — which factors predict eating disorder onset in adolescents, how does maternal communication function as a risk factor, what linguistic patterns in mother-daughter conversations signal risk. I bring construct expertise — knowing what 'body dissatisfaction' means clinically, not just statistically. And I bring rigorous research design and human subjects knowledge, especially regarding minors. A computational collaborator brings the technical implementation expertise — the NLP methods, the model architecture decisions, the optimization. Together, we produce work that's both technically sound and psychologically meaningful. I've found that computational researchers are often looking for domain experts to collaborate with — they have the tools but need the questions and the data."

---

### Teaching Questions

#### Q8: "Could you teach a course on AI and psychology?"

**Framework**: Specific course ideas, appropriate scope

> "Absolutely. I'd be excited to develop an undergraduate course called 'Psychology in the Age of AI' — an accessible introduction to how AI is transforming psychological research, clinical practice, and everyday life. No programming required — the emphasis would be on critical thinking about AI's capabilities and limitations, with hands-on activities using ChatGPT and similar tools. For graduate students, I could develop a methods course on AI-assisted text analysis and NLP tools for psychology, designed specifically for psychology students who have quantitative training but no CS background. I'd also be interested in a graduate seminar on ethics of AI in mental health, which connects directly to my research on vulnerable populations."

---

### Ethics Questions

#### Q9: "What ethical concerns do you see with using AI in your research?"

**Framework**: Specific to your research area, nuanced, actionable

> "Several concerns are central to my work. First, algorithmic bias: body image classification models trained predominantly on thin, White beauty standards will encode those standards — producing tools that misclassify or underserve diverse populations. This isn't hypothetical; it's a documented pattern in AI systems. Second, consent with minors: if I'm doing digital phenotyping with adolescents, the consent process needs to be meaningful and age-appropriate — can a 13-year-old truly understand that their social media data will be analyzed by an ML algorithm? Third, clinical responsibility: if a predictive model flags an adolescent as high-risk, what are the obligations to act? These aren't reasons to avoid AI/ML — they're reasons to ensure that people with clinical and developmental expertise are involved in designing these tools. I see this as part of my scholarly contribution: developing AI/ML applications that are not only technically effective but ethically responsible."

---

#### Q10: "How would you ensure your AI/ML research is equitable?"

**Framework**: Specific practices, not just principles

> "Equity has to be built in from the start, not checked at the end. Practically, this means several things for my research. First, diverse training data: any NLP model I develop for coding body image content needs to be trained on language from diverse racial, ethnic, and body-size populations — not just the thin, White, cisgender samples that dominate this literature. Second, subgroup validation: when I build predictive models, I'd evaluate performance separately across demographic groups to identify disparities. Third, participatory design: involving adolescents and families — particularly from marginalized communities — in defining what body image constructs mean to them and how AI tools should function. Fourth, transparency: publishing model performance across subgroups, not just aggregate accuracy. This approach makes the research better, not just more equitable."

---

#### Q11: "A colleague is skeptical about AI in psychology. How would you respond?"

**Framework**: Validate the concern, then redirect constructively

> "I think healthy skepticism is appropriate and valuable. There are real risks — hype outpacing evidence, tools being deployed before they're validated, algorithmic bias causing harm. I share those concerns. Where I'd push back gently is on the idea that psychology can afford to ignore AI/ML entirely. Computational methods are being applied to psychological phenomena whether psychologists are involved or not — by computer scientists who may not understand the constructs, by tech companies without clinical training. I'd rather have psychologists at the table, bringing our theoretical knowledge, ethical training, and understanding of human complexity to shape how these tools are developed and used. We don't have to adopt every new method uncritically, but we do need to engage with the ones that are going to affect our field and our populations."

---

#### Q12: "What would you need from us to be successful with your AI/ML research?"

**Framework**: Show you've thought about infrastructure

> "Three things. First, access to computing resources — whether that's a university HPC cluster or cloud computing credits — for training ML models on larger datasets. Second, opportunities for interdisciplinary collaboration, whether through a data science center, cross-departmental seminars, or connections to computational researchers. Third, some flexibility in my first few years to invest in training — attending computational methods workshops, taking courses, developing these skills alongside my active research program. I'd also be interested in learning about any existing computational infrastructure or collaborations in the department that I could contribute to."

---

## Questions to Ask Them

These questions signal genuine, thoughtful interest in AI/ML infrastructure:

1. "What computing resources are available for researchers doing machine learning or large-scale data analysis?"
2. "Are there faculty in other departments working on NLP, machine learning, or computational social science who might be interested in psychology collaborations?"
3. "Does the university have a data science center, institute, or similar resource that supports social science researchers?"
4. "How does the department see the role of computational and AI methods in its future?"
5. "Are there interdisciplinary working groups, seminars, or reading groups focused on technology and behavioral science?"
6. "What support exists for faculty who want to develop new methodological skills — workshops, course releases, training grants?"
7. "Are graduate students coming in with more computational skills than in previous cohorts? How is the department adapting training to reflect that?"

---

## 60-Second Elevator Pitch

### Casual Version (at a conference reception)

> "I study how mothers and daughters talk about bodies — and how those conversations shape adolescent body image and eating disorder risk. It's longitudinal, mixed-methods work that's generated really rich data. What I'm excited about right now is bringing computational tools to it — using NLP to analyze conversation transcripts at a scale I can't do manually, and machine learning to build better prediction models for who's at risk. I see myself as the psychology person who makes sure those tools are grounded in what we actually know about development and clinical risk."

### Formal Version (at the start of a research presentation)

> "My research program examines how parental communication — particularly maternal commentary about bodies and appearance — shapes body image development and eating disorder risk across adolescence. I use longitudinal designs, qualitative methods with mother-daughter dyads, and quantitative modeling. I'm now extending this work with computational approaches: natural language processing to analyze parent-child communication at scale, and machine learning to build integrative risk prediction models. My goal is a research program that combines deep domain expertise in body image and adolescent development with the computational tools that can amplify its impact."

### Written Version (for a bio or website)

> "[Your name] is a [developmental/clinical] psychologist studying the role of maternal communication in adolescent body image and eating disorder risk. Her research uses longitudinal and qualitative methods to understand how mothers' body talk shapes daughters' self-perception across development. She is currently integrating natural language processing and machine learning into her research program, leveraging computational tools to analyze parent-child communication at scale and build predictive models for eating disorder risk. She is committed to ensuring that AI/ML tools applied to youth mental health are ethically responsible, clinically grounded, and validated across diverse populations."

---

## Red Flags and How to Handle Them

### When You Don't Know Something

**Scenario**: An interviewer asks about a specific ML technique you're not familiar with.

**Don't**: Pretend you know it. Bluff. Get flustered.

**Do**: "I'm not familiar with that specific technique — can you tell me more about how it's being applied? I'd be interested to learn how it relates to the NLP and prediction work I'm building toward."

This shows intellectual curiosity and honesty, which are valued far more than fake expertise.

### When They Expect More Than You Have

**Scenario**: The committee seems to want someone who already publishes with AI/ML methods.

**Don't**: Overstate your current skills. Promise things you can't deliver.

**Do**: "I want to be transparent about where I am — I have a strong conceptual foundation and emerging hands-on skills, with a clear development trajectory. Where I'm already strong is in the domain expertise, the research questions, and the study design that computational methods need to be grounded in. My plan is to deepen my computational skills through collaboration and targeted training in my first few years."

If the position truly requires someone who already publishes with deep learning, it may not be the right fit — and that's valuable information.

### When You're Asked to Compare Methods You Don't Fully Understand

**Scenario**: "Would you use a transformer or an LSTM for your text analysis?"

**Don't**: Pick one randomly and pretend you understand the tradeoff.

**Do**: "That's a technical decision I'd make in collaboration with a computational colleague, based on the specific characteristics of my data. What I can speak to is what I need the model to do — accurately classify body-related language in conversational transcripts — and I'd evaluate any approach against that criterion with rigorous validation."

This shows you understand the process even if you can't make the technical choice alone.

### When They're Skeptical of AI/ML in Psychology

**Scenario**: A committee member seems dismissive of AI/ML as a fad.

**Don't**: Be defensive. Argue about the importance of AI.

**Do**: "I appreciate that skepticism — and I share the concern about hype outpacing evidence. What draws me to these methods isn't the buzzwords; it's specific, practical problems in my research. I have hundreds of hours of conversation transcripts I can't code by hand fast enough, and I have multivariate longitudinal data with complex interactions that linear models don't capture well. AI/ML addresses those specific problems. But I'll always validate computationally generated results against human judgment and clinical knowledge."
