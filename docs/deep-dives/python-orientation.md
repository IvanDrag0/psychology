# Python Orientation for R Users

**Prerequisites**: Week 1 completed | **Type**: Deep Dive (Optional)

---

You do not need Python right now. But as you read papers, watch tutorials, or browse
ML communities, you will encounter Python constantly. This FAQ answers the questions
that come up most often so you can orient yourself without committing to learning a
second language before you are ready.

---

## Do I Actually Need to Learn Python?

Honest answer: not yet, and maybe not for a long time. R with tidymodels covers
classification, regression, random forests, gradient boosting, cross-validation,
and hyperparameter tuning. That is more than enough for the work in this course
and for a wide range of applied ML projects in psychology.

Where Python becomes hard to avoid is deep learning and natural language processing
with transformer models (the architecture behind GPT, BERT, and similar systems).
The ecosystems for those tasks are Python-first, and the R wrappers tend to lag
behind. But that is a bridge you cross later, not now.

## What Is Python Better at Than R?

- **Deep learning frameworks.** PyTorch and TensorFlow are built for Python. R
  interfaces exist (torch for R, keras for R) but the documentation, community
  support, and tutorials overwhelmingly assume Python.
- **NLP with transformer models.** Hugging Face, the main hub for pretrained
  language models, is Python-native. If you want to fine-tune BERT for clinical
  text classification, you will almost certainly do it in Python.
- **Production deployment.** When ML models need to run as part of a web service
  or be embedded in software, Python is the standard.
- **Computer vision.** Image classification, object detection, and similar tasks
  are dominated by Python tooling.
- **General-purpose programming.** Python is a general-purpose language; R is a
  domain-specific one. If a project involves building software beyond analysis,
  Python is more natural.

## What Is R Better at Than Python?

- **The tidymodels workflow.** Clean, consistent, and composable. Nothing in Python
  matches the coherence of recipes, parsnip, rsample, and tune working together.
- **Statistical modeling.** Mixed-effects models (lme4), structural equation
  modeling (lavaan), item response theory, psychometrics -- these are mature and
  well-supported in R. Python equivalents exist but are less developed.
- **ggplot2.** The grammar of graphics remains the gold standard for publication-
  quality statistical visualization.
- **Your discipline knows R.** Your collaborators read R. Your reviewers read R.
  Journals in psychology expect R or SPSS. This matters for reproducibility.
- **RMarkdown and Quarto.** Reproducible documents that weave code, output, and
  prose. Jupyter notebooks serve a similar role in Python, but Quarto in
  particular is more polished for academic writing.
- **Psychology-specific packages.** psych, lavaan, lme4, brms, emmeans, effectsize
  -- these were written by and for behavioral scientists.

## Can I Use Both Languages Together?

Yes. The reticulate package lets you call Python from within R. You can pass data
frames back and forth, use a Python library for one step of your analysis, and
return the results to R for everything else.

Many researchers settle into a pattern: R for data wrangling, exploratory analysis,
and statistical modeling; Python for deep learning or NLP when a specific project
demands it. Running separate projects in separate languages is also perfectly fine.
You do not have to integrate them into a single workflow unless that makes your
life easier.

## When Should I Start Learning Python?

After you are comfortable with tidymodels and you have a concrete project that
requires it. Vague pressure to "know Python" is not a reason. Specific needs are.

Signs that it may be time:

- You want to fine-tune a transformer model for text classification on clinical
  notes or open-ended survey responses.
- You need to use Hugging Face models for sentiment analysis, named entity
  recognition, or text generation.
- A collaborator has built a pipeline in Python and you need to contribute to it
  or reproduce their results.
- You are taking a dedicated deep learning course that uses PyTorch.
- You want to deploy a model as part of an application or API.

If none of those apply, stay in R. You are not falling behind.

## What Is the Minimum I Would Need to Know?

If the day comes, here is a rough mapping from what you already know:

| R (what you know)          | Python equivalent              |
|----------------------------|--------------------------------|
| tidyverse (dplyr, tidyr)   | pandas                         |
| ggplot2                    | matplotlib, seaborn            |
| tidymodels                 | scikit-learn                   |
| quanteda (text analysis)   | NLTK, spaCy                   |
| --                         | Hugging Face transformers      |
| --                         | PyTorch / TensorFlow           |
| RMarkdown / Quarto         | Jupyter notebooks              |

The conceptual knowledge transfers directly. A random forest is a random forest
regardless of language. Cross-validation is cross-validation. The learning curve
is syntax and tooling, not ideas.

## How Would I Actually Learn Python?

A reasonable sequence for someone coming from R:

1. **Start with pandas.** Data manipulation in pandas will feel familiar if you
   know dplyr. The verbs are different but the logic is the same: filter rows,
   select columns, group and summarize.
2. **Then scikit-learn.** It parallels tidymodels -- fit a model, predict, evaluate.
   The API is consistent across model types, just as parsnip is.
3. **Then Hugging Face or PyTorch**, depending on whether your goal is NLP or
   deep learning more broadly.

Useful resources:

- *Python for Data Analysis* by Wes McKinney -- the pandas creator's book, and
  the closest equivalent to *R for Data Science*.
- Google's Python Class -- free, well-structured, assumes no prior Python.
- DataCamp's R-to-Python bridge courses -- explicitly designed for your situation.
- *Deep Learning with Python* by Francois Chollet -- if you reach the deep
  learning stage.

## Will I Lose My R Skills if I Learn Python?

No. The two languages reinforce each other. Understanding data frames in pandas
makes you appreciate tibbles more, and vice versa. The ML concepts are identical.
What changes is the syntax you type, not the way you think about problems.

## Should I Worry About the "Python vs R" Debate?

No. That debate is mostly noise. The practical reality is that both languages are
widely used in data science and they serve overlapping but distinct purposes. In
psychology specifically, R is dominant and will remain so for standard statistical
work. Python extends your reach into areas where R has less support. They are
complements, not competitors.

## The Bottom Line

R is your home base. It is where your discipline lives, where your statistical
training applies most directly, and where tidymodels gives you a clean path into
machine learning. Python is a tool you will pick up when a specific project
demands it -- not because someone on the internet said you should.

Do not let anyone make you feel behind for not knowing Python. Most psychology
researchers who are applying machine learning methods in R are already well ahead
of their field. Python will be there when you are ready for it, and the concepts
you are learning now will transfer cleanly.

For this course, R is all you need.
