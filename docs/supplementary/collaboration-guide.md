# Collaboration Guide: Working with Computational Researchers

This is reference material for when you've landed a position and are ready to reach out to computational collaborators. There's no urgency here — come back when you have a specific project in mind and a person you'd like to approach.

---

## Why Collaborate

The most impactful AI/ML work in psychology is collaborative. Look at the papers that are actually changing clinical practice — automated screening tools, NLP-based assessment, predictive models for treatment response — and you will find a psychologist and a computer scientist on the author list. Usually both are near the front.

This is not a failure. It is how the field works.

**What you bring:**

- **Research questions that matter.** You know which clinical problems are urgent, which theoretical gaps need filling, and which measurement challenges keep the field stuck.
- **Data.** You have IRB-approved access to coded transcripts, longitudinal datasets, clinical measures, and participant relationships built on years of careful work.
- **Theoretical framework.** You can interpret what a model's output actually means for real people and real families.
- **Publication venues.** You know which journals matter, what reviewers expect, and how to frame findings for a psychology audience.

**What a computational collaborator brings:**

- **Methods expertise.** They know which algorithm fits which problem, how to validate models properly, and how to avoid the technical pitfalls.
- **Coding fluency.** They can build pipelines, process text data at scale, and implement models efficiently.
- **Optimization skills.** They know how to tune performance, handle messy real-world data computationally, and scale analyses.

Neither of you can do the other's job well. Together, you produce work that is both technically sound and clinically meaningful.

---

## Finding Collaborators

You need to find someone who has complementary skills, is interested in human behavior or health, and is looking for exactly what you offer: a domain expert with data and questions.

### At Your Institution

Start local. The easiest collaborations are with people you can meet in person.

- **Data science centers or institutes.** Most R1 universities now have one. They often have faculty affiliates, postdocs, or staff scientists looking for applied projects.
- **Statistics departments.** Look for faculty working on applied statistics, Bayesian methods, or statistical learning. They often want real-world applications for their methods.
- **Computer science departments.** Search for researchers in NLP, human-computer interaction, or computational social science.
- **Informatics or biomedical informatics.** These departments bridge health and computation by design.
- **Public health biostatisticians.** They already think about health outcomes and are often familiar with longitudinal and survey data.
- **Digital health groups.** If your institution has a digital health lab or center, the researchers there are actively looking for clinical domain experts.

### At Conferences

- **Computational psychology sessions.** These appear increasingly at APA, APS, and ABCT. The presenters are exactly who you want to talk to.
- **Technology and digital health workshops.** ABCT has been expanding these. APS has relevant poster sessions.
- **Society for Improvement of Psychological Science (SIPS).** Strong culture of methodological innovation and openness to collaboration.
- **Interdisciplinary conferences.** AMIA (informatics), ACL (NLP), and CHI (human-computer interaction) all have health or behavioral tracks.

### Online

- **Twitter/X academic communities.** Follow hashtags like #PsychTwitter, #CompPsych, #NLProc, and #DigitalHealth. Engage with researchers whose work interests you.
- **GitHub.** Search for repositories related to psychology + NLP or mental health + machine learning. The people building open tools want collaborators.
- **ResearchGate and Google Scholar.** Find people publishing at the intersection. Read their papers, then reach out.

### Through Existing Networks

- **Ask your advisor.** They may know someone, or know someone who knows someone.
- **Ask current collaborators** who they have worked with on computational projects.
- **Reverse engineer the author lists** of papers you admire. If you read a great paper applying NLP to therapy transcripts, email the first author.

### Cold Emails

They work better than you think in academia. Most researchers — especially early-career ones — are happy to hear from someone with a concrete project idea and real data. The key is making it easy for them to say yes.

---

## The Pitch

The way you approach a potential collaborator matters enormously. You are not asking for a favor. You are proposing a partnership where both sides benefit.

### Key Principles

**Lead with your research question and data, not with a request for technical help.** The difference between "I need someone to do ML for me" and "I have 40 coded transcripts of mother-daughter conversations about body image and a specific question about whether NLP can predict our manual codes" is the difference between being ignored and getting a meeting.

**Show that you have done your preparation.** Mention that you understand the difference between supervised and unsupervised learning. Reference a specific technique that might apply. You do not need to be an expert, but you need to show you will not require hand-holding on basic concepts.

**Be specific about what you want to explore.** Vague requests get vague responses (or no response). A concrete project description gives the other person something to react to.

**Make the collaboration mutually beneficial.** Computational researchers need applications for their methods, access to real-world data, domain expertise for interpreting results, and publications in applied journals. You offer all of that. Say so explicitly.

### Template Email

Below is a template you can customize. Adjust the details to match your situation, but keep the structure: context, question, what you bring, what you are looking for, and a clear ask.

> Subject: Potential collaboration — NLP for adolescent body image research
>
> Dr. [Name],
>
> I am a psychology PhD researcher studying mother-daughter communication about body image and its impact on adolescent development. I came across your work on [specific paper or project] and thought there might be a productive overlap with my research.
>
> I have a dataset of 40 manually coded transcripts of mother-daughter conversations, along with longitudinal survey data on body dissatisfaction. I am interested in whether NLP methods could learn to predict our manual coding categories, which would both validate the coding scheme and create a scalable tool for future work.
>
> I bring the domain expertise, data, IRB approval, theoretical framework, and familiarity with the publication landscape in developmental and clinical psychology. I am looking for a collaborator with NLP expertise who would be interested in co-developing and co-authoring this work.
>
> I have conceptual fluency with ML approaches and hands-on experience using AI tools for text classification, so I can engage substantively with the technical side. Would you be open to a 20-minute conversation to see if this is a good fit?
>
> Best,
> [Your name]

### What NOT to Do

**Do not ask them to teach you ML.** A collaborator is a partner, not a tutor.

**Do not present yourself as a blank slate.** You have years of training in research design, measurement, statistics, clinical interpretation, and a specific content area. That is enormously valuable.

**Do not propose something vague.** "I think AI is really interesting and I would love to explore how it could help my research" is not a pitch. Arrive with a specific question, a specific dataset, and a rough idea of what methods might apply.

---

## Your First Project Together

Your first collaborative project should be small enough to succeed and meaningful enough to publish.

### The Ideal First Project

Take something you have already done manually and see if ML can learn to do it. The natural candidate:

**"Train an NLP classifier to predict manual codes in [your] transcripts."**

Why this works:

- You already have the data
- You already have the gold standard (your manual codes)
- The question is publishable regardless of outcome
- It produces something useful: a tool you can apply to future data
- The scope is contained

### Key Scoping Principles

**Start with data you already have.** Do not design a new study for your first ML project.

**Pick a question that is publishable regardless of ML performance.** If the model works beautifully, great. If it performs at chance, that is also informative.

**Define success criteria upfront.** Before you start, agree with your collaborator on what "good enough" performance looks like.

**Keep regular contact.** Brief, frequent check-ins keep the project moving.

### Other Realistic First Projects

- **Predictive modeling with longitudinal data.** Build a predictive model identifying which individuals are most at risk.
- **Sentiment analysis of social media data.** NLP-based sentiment and theme analysis can reveal patterns across thousands of posts that manual coding could never reach.
- **Automated coding of open-ended survey responses.** A classifier trained on a manually coded subset can scale your coding to the full dataset.

---

## Collaboration Template

Use this project brief to organize your thinking and share it with potential collaborators. Fill it out before your first meeting.

---

### Project Brief: [Working Title]

**Research Question**
[One sentence. Be as specific as possible. Example: "Can an NLP classifier trained on manually coded mother-daughter transcripts achieve inter-rater-level agreement on body image communication categories?"]

**Why It Matters**
[2-3 sentences on clinical or theoretical significance.]

**Available Data**
[What you have. Be specific about sample size, variables, format, and any access restrictions.]

**Proposed ML Approach**
[Your best guess. It is completely fine if this changes after discussion.]

**Your Role**
[What you will contribute. Example: "Domain expertise, data access and IRB management, clinical interpretation of model output, lead on manuscript writing, theoretical framing."]

**Collaborator's Role**
[What you need from them. Example: "NLP model development, training, and validation. Text preprocessing pipeline. Technical methods writing."]

**Timeline**
[Realistic estimate with key milestones.]

**Target Outcome**
[What does success look like?]

**Target Venue**
[Where will you submit?]
