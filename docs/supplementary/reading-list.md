# Reading List: AI/ML in Psychology Research

An annotated bibliography organized by priority and topic. Start with the Minimal Viable Reading Plan, then branch out based on your interests.

---

## Minimal Viable Reading Plan

If you're short on time, here's the priority order:

1. **Before applications** (essential): Read Norris et al. (2024) and McClure et al. (2025) in full. Skim Monaco et al. (2024). These give you enough to discuss AI/ML in eating disorders knowledgeably
2. **Before interviews**: Read Rothenberg et al. (2023) for the adolescent prediction angle. Skim 2-3 papers from the "Go Deeper" section most relevant to your planned research
3. **First month on tenure track**: Work through *Tidy Modeling with R* (the full tidymodels textbook at tmwr.org). Read Ghosh et al. (2024) for the clinical ML landscape
4. **First year on tenure track**: Work through *Supervised Machine Learning for Text Analysis in R* (smltar.com). Read the NLP and ethics papers relevant to your specific projects
5. **Ongoing**: Follow StatQuest and 3Blue1Brown on YouTube. Attend one workshop per year. Subscribe to one podcast

---

## Start Here: 5 Must-Reads

These papers give you the broadest, most immediately useful overview of AI/ML in your research area. Read at least the abstracts of all five; read in full the ones most relevant to your specific work.

### 1. Norris, Obeid, & El Emam (2024)
**Full title**: "Examining the role of artificial intelligence to advance knowledge and address barriers to research in eating disorders"
**Journal**: *International Journal of Eating Disorders*, 57(6), 1357-1368
**DOI**: [10.1002/eat.24215](https://doi.org/10.1002/eat.24215)

**Why read it**: This is the single best map of how AI is being applied in eating disorder research right now. Covers AI's potential for data sharing/pooling, data augmentation, addressing research barriers, and bias in datasets. Reading this one paper will give you a comprehensive overview and a library of references to explore.

**Key takeaway**: There is tremendous potential to embed AI across eating disorders research, but regulation, ethical guidelines, and provider/patient trust are needed for responsible adoption.

---

### 2. McClure, Fuller-Tyszkiewicz, Messer, & Linardon (2025)
**Full title**: "Machine-Learning Applications in Eating-Disorder-Outcome Prediction: A Systematic Scoping Review"
**Journal**: *Clinical Psychological Science* (SAGE)
**DOI**: [10.1177/21677026251340348](https://doi.org/10.1177/21677026251340348)

**Why read it**: This systematic scoping review identified 75 studies on ML applications in ED outcome prediction. Shows the practical application of ML concepts you learned in Week 1 — decision trees, random forests, and SVMs were the most commonly used models.

**Key takeaway**: ML has been used to predict ED diagnostic status (45 studies), escalation of risk/symptoms (13 studies), treatment outcomes (12 studies), and ED onset (6 studies). The field is growing rapidly, with clear opportunities for your research.

---

### 3. Monaco, Vignapiano, Piacente et al. (2024)
**Full title**: "An advanced Artificial Intelligence platform for a personalised treatment of Eating Disorders"
**Journal**: *Frontiers in Psychiatry*, 15, 1414439
**DOI**: [10.3389/fpsyt.2024.1414439](https://doi.org/10.3389/fpsyt.2024.1414439)

**Why read it**: Represents the cutting edge of AI application in your specific area. Presents the Master Data Platform (MDP), an AI-powered platform that integrates clinical assessments, demographics, and physiological data to personalize ED treatment, plan treatment strategies, predict relapse, and includes a chatbot for patient engagement.

**Key takeaway**: AI platforms for ED treatment are moving from concept to implementation, creating opportunities for clinical researchers to shape how these tools are developed and validated.

---

### 4. Ghosh, Burger, Simeunovic-Ostojic, Maas, & Petkovic (2024)
**Full title**: "Review of Machine Learning Solutions for Eating Disorders"
**Journal**: *International Journal of Medical Informatics*, 189, 105526
**DOI**: [10.1016/j.ijmedinf.2024.105526](https://doi.org/10.1016/j.ijmedinf.2024.105526)

**Why read it**: A narrative review bridging the gap between ED researchers and AI practitioners. Covers current ML and AI applications in eating disorders with emphasis on clinical management, presenting state-of-the-art applications and identifying limitations.

**Key takeaway**: The field needs clinician-researchers who understand both the psychology and the computational methods — your profile is exactly what's needed for responsible development.

---

### 5. Rothenberg et al. (2023)
**Full title**: "Predicting Adolescent Mental Health Outcomes Across Cultures: A Machine Learning Approach"
**Journal**: *Journal of Youth and Adolescence*, 52(8), 1595-1619
**DOI**: [10.1007/s10964-023-01767-w](https://doi.org/10.1007/s10964-023-01767-w)

**Why read it**: ML models examined 79 variables assessed at age 10 to predict adolescent mental health at ages 13 and 17 across multiple cultures. Demonstrates how data-driven and theory-driven methods can be integrated for cross-cultural youth mental health prediction.

**Key takeaway**: Models accurately classified mental health difficulties for approximately 7 in 10 adolescents. Key predictors included emotional symptoms, peer/conduct problems, stress, parental BMI, body dissatisfaction, and childhood BMI — many of which overlap with your research variables.

---

## Go Deeper: By Topic

### NLP in Psychology and Eating Disorders

- `Before interviews` **Mackowska, Koscien, Wojcik, Rojewska, & Spinczyk (2024)**, "Using Natural Language Processing for a Computer-Aided Rapid Assessment of the Human Condition in Terms of Anorexia Nervosa," *Applied Sciences*, 14(8), 3367. Applies NLP and ML to classify body image notes from young adults, successfully differentiating individuals with AN based on linguistic profiles.

- `First year` **Merhbene, Puttick, & Kurpicz-Briki (2024)**, "Investigating machine learning and natural language processing techniques applied for detecting eating disorders: a systematic literature review," *Frontiers in Psychiatry*, 15, 1319522. Comprehensive systematic review of ML and NLP techniques for ED detection covering both clinical and non-clinical data sources.

- `First year` **Sadowski et al. (2025)**, "Negative and Positive Body-Related Emotions Derived From Voice Recordings During a Mirror Task in Anorexia and Bulimia Nervosa: A Natural Language Processing Approach Using RoBERTa," *International Journal of Eating Disorders*. DOI: [10.1111/eat.70007](https://doi.org/10.1111/eat.70007). Uses transformer-based NLP (RoBERTa) to identify body-related emotions from voice recordings during a mirror exposure task.

- `Before interviews` **Therapy transcript analysis using NLP**: Search for studies analyzing therapeutic process and outcome using NLP methods applied to session transcripts. Multiple research groups are active in this area.

### Predictive Modeling in Clinical Science

- `Before interviews` **Katsiferis, Joensen, Petersen, Ekstrom, & Olsen (2025)**, "Developing machine learning models of self-reported and register-based data to predict eating disorders in adolescence," *npj Mental Health Research*. Developed diagnostic and prognostic models using 44,357 participants from the Danish National Birth Cohort. Achieved AUC of 81.3 (diagnostic) and 76.9 (prognostic). Key predictors: sex, emotional symptoms, stress, parental BMI, body dissatisfaction.

- `First year` **Monaco, Vignapiano, Di Gruttola et al. (2025)**, "Neuroimaging and machine learning in eating disorders: a systematic review," *Eating and Weight Disorders*, 30, 46. PRISMA-compliant review of neuroimaging + ML for ED diagnosis and prognosis. Found only 5 studies meeting criteria — indicating this is a nascent but promising area.

- `Ongoing` **Machine learning for suicide risk prediction**: A substantial literature exists on ML prediction of suicide risk — methodologically relevant even if not your specific area, because the same approaches apply to ED risk prediction.

### Digital Phenotyping and EMA
- `First year` **Digital phenotyping and adolescent mental health**: Studies using smartphone passive sensing with adolescent populations. Look for work from the Onnela Lab (Harvard) and similar groups
- `First year` **EMA and machine learning**: Papers combining ecological momentary assessment with ML analysis. Particularly relevant for understanding within-person dynamics
- `Ongoing` **Social media exposure measurement via digital phenotyping**: Studies that go beyond self-report to capture actual social media content exposure

### Body Image and Technology

- `Before applications` **Quittkat, Hartmann, Dusing, & Buhlmann (2024)**, "Like Mother, Like Daughter? Double Standards in Body Evaluation and Their Familial Transmission in Female Adolescents and Their Mothers," *Cognitive Therapy and Research*. DOI: [10.1007/s10608-024-10507-8](https://doi.org/10.1007/s10608-024-10507-8). Demonstrates that daughters evaluate their own bodies more negatively than peers' bodies, and that higher negative maternal feedback is associated with more self-deprecating double standards. Directly relevant to your research; consider how NLP could be applied to this communication.

- `Before interviews` **Social media and body image in adolescents — meta-analyses**: Recent meta-analyses quantifying the relationship between social media use and body image. These identify the effect sizes your ML models would be trying to improve upon

- `Ongoing` **Fitspiration, thinspiration, and body positivity on social media**: Content analysis studies that could be scaled with NLP methods

### AI Ethics and Eating Disorders

- `Before interviews` **He & Ji (2025)**, "Artificial Intelligence and Social Media for the Detection of Eating Disorders," *International Journal of Eating Disorders*, 58(7), 1187-1190. Examines how AI and social media data can be leveraged for ED detection, discussing both potential and ethical challenges of mining social media for mental health screening.

- `Before applications` **Linardon (2025)**, "Conducting Eating Disorder Research in the Era of Generative AI," *International Journal of Eating Disorders*. Guidelines for ED researchers on appropriate use of generative AI tools, addressing limitations, disclosure practices, and ethical implications.

- `Before applications` **Linardon, Liu, Messer, McClure, Anderson, & Jarman (2025)**, "Using Artificial Intelligence to Advance Eating Disorder Research, Treatment and Practice," *International Journal of Eating Disorders*, 58(5), 811-812. Editorial introducing a special issue on AI in eating disorders — excellent for understanding the field's trajectory.

- `Before interviews` **APA guidelines for AI in psychology**: Professional guidance on responsible use of AI in psychological research and practice

- `First year` **Consent and data privacy in digital phenotyping with minors**: Emerging ethical frameworks for passive data collection with youth populations

- `Ongoing` **Weight bias in AI systems**: Studies examining how AI image recognition, language models, and recommendation systems perpetuate weight stigma

---

## Methods Primers: Learning to Do AI/ML

### R-Based ML Guides
- **Tidy Modeling with R** (Kuhn & Silge, 2022): The definitive free online textbook for tidymodels. Available at tmwr.org. Start here for deepening your R-based ML skills after the Week 2 notebook
- **An Introduction to Statistical Learning (ISLR)** (James et al., 2021): Classic ML textbook with R code. Free PDF available. More theoretical than tidymodels book but excellent for understanding why algorithms work
- **Supervised Machine Learning for Text Analysis in R** (Hvitfeldt & Silge, 2022): NLP in R using tidymodels. Free online at smltar.com. Directly relevant to your NLP interests
- **R for Data Science** (Wickham & Grolemund): If you need to strengthen your tidyverse foundations. Free at r4ds.had.co.nz

### Accessible ML Tutorials
- **Google's Machine Learning Crash Course**: Free, interactive, designed for beginners. Uses Python but the concepts transfer directly
- **StatQuest (YouTube)**: Josh Starmer's YouTube channel explains ML algorithms with remarkable clarity. Start with "Machine Learning Fundamentals" and "Random Forests" videos
- **3Blue1Brown — Neural Networks (YouTube)**: Beautiful visual explanations of neural networks. Watch for conceptual understanding, not technical depth

### NLP-Specific Resources
- **quanteda R package documentation**: Text analysis in R. Good starting point for learning NLP in a language you already know
- **Hugging Face course**: Free NLP course. More technical (Python-based) but excellent for understanding transformer models and modern NLP
- **Natural Language Processing with Python (NLTK book)**: Free online textbook. Good if you ever want to add Python to your toolkit

### tidymodels Documentation
- **tidymodels.org**: Official documentation with tutorials, articles, and function references
- **Get Started tutorials**: Step-by-step guides that expand on what you did in the Week 2 notebook
- **Model list**: Every model type available in tidymodels, with code examples

---

## Courses and Online Resources

### Workshops and Short Courses
- **APA Technology, Mind, and Society conference**: Annual conference with workshops on AI/ML in psychology
- **ABCT and APS pre-conference workshops**: Look for computational methods workshops at major psychology conferences
- **Data Science for Psychologists workshops**: Several universities offer summer workshops specifically designed for psychology researchers learning computational methods
- **NIH Office of Data Science Strategy**: Training resources for biomedical researchers learning data science

### Online Courses
- **Coursera — Machine Learning Specialization (Andrew Ng)**: The most famous ML course. Conceptually excellent, uses Python
- **Coursera — Applied Data Science with R**: R-based data science course relevant to your skills
- **edX — Data Science professional certificates**: Multiple universities offer certificate programs
- **DataCamp — Machine Learning with R**: Interactive R-based ML courses, some available free

### YouTube Channels
- **StatQuest with Josh Starmer**: Best for intuitive understanding of ML algorithms
- **3Blue1Brown**: Best for visual/mathematical intuition about neural networks
- **Cassie Kozyrkov (Google)**: Decision science and ML for non-engineers

### Podcasts
- **Talking Machines**: Accessible conversations about ML research
- **Linear Digressions**: ML concepts explained for non-experts (archived but still useful)
- **TWIML (This Week in Machine Learning)**: More technical, but good for staying current

### Professional Communities
- **Society for Improvement of Psychological Science (SIPS)**: Increasingly includes computational methods discussions
- **Computational Psychiatry groups**: Growing community at the intersection of computation and mental health
- **R-Ladies**: Global organization supporting gender minorities in R programming. Active community with mentoring and workshops
- **Posit Community (formerly RStudio Community)**: Online forum for R and tidymodels questions

---

## How to Use This List

### Timing Tags

Each entry in the "Go Deeper" sections above is tagged with when it's most useful: `Before applications`, `Before interviews`, `First year`, or `Ongoing`. Use the Minimal Viable Reading Plan at the top of this page for the priority order.
