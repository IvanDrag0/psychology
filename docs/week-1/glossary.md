# Week 1 Glossary: AI/ML Terminology for Psychology Researchers

This glossary covers the ~30 terms you'll encounter most frequently in Week 1. Each entry includes a plain-English definition, a psychology analogy to anchor the concept, and a research example. Terms marked with **[Interview Term]** are ones you should be able to define and discuss confidently in a job interview.

For the complete A-Z glossary covering all three weeks, see [Complete Glossary](../supplementary/complete-glossary.md).

---

## Natural Language Processing

These are the first concepts you'll encounter through the qualitative coding exercise.

### Natural Language Processing (NLP) **[Interview Term]**

???+ note "Full definition"

    **Definition**: The branch of AI focused on enabling computers to understand, interpret, and generate human language.

    **Psychology analogy**: Think of it as automated qualitative coding at a massive scale. Instead of you reading 200 interview transcripts and identifying themes, the computer reads them and identifies patterns in the language.

    **Example**: Using NLP to analyze thousands of posts on eating disorder recovery forums to identify common themes, emotional trajectories, and linguistic markers of recovery vs. relapse.

---

### Sentiment Analysis

???+ note "Full definition"

    **Definition**: An NLP technique that determines the emotional tone of text (positive, negative, neutral) or more nuanced emotions.

    **Psychology analogy**: Like having a research assistant code the emotional valence of open-ended responses --- but automated and scalable to millions of texts.

    **Example**: Analyzing the sentiment of how mothers and daughters discuss body image in text messages over time --- tracking whether conversations become more positive or negative.

---

### Topic Modeling

???+ note "Full definition"

    **Definition**: An unsupervised NLP technique that discovers abstract "topics" or themes across a collection of documents.

    **Psychology analogy**: Very similar to thematic analysis in qualitative research, but computational. The algorithm reads all your documents and says "I found these clusters of words that tend to appear together --- they might represent themes."

    **Example**: Running topic modeling on adolescent therapy session transcripts to discover recurring themes (e.g., peer pressure, family conflict, appearance anxiety) without predefined codes.

---

### Text Mining

???+ note "Full definition"

    **Definition**: The process of extracting useful information and patterns from large amounts of text data.

    **Psychology analogy**: Like a turbocharged literature review or content analysis. Instead of manually counting how often certain words appear or themes arise, the computer does it across thousands of documents.

    **Example**: Mining social media data to track how frequently adolescents mention body-related terms and how those frequencies correlate with cultural events (e.g., fashion weeks, diet culture trends).

---

## LLM / AI / ML Hierarchy

### Artificial Intelligence (AI) **[Interview Term]**

???+ note "Full definition"

    **Definition**: The broad field of creating computer systems that can perform tasks typically requiring human intelligence --- like understanding language, recognizing patterns, or making decisions.

    **Psychology analogy**: Think of AI as the umbrella term, the way "psychology" encompasses everything from neuroscience to social psych. It's the whole discipline, not one specific method.

    **Example**: A system that reads therapy session transcripts and flags potential risk indicators is an AI application.

---

### Machine Learning (ML) **[Interview Term]**

???+ note "Full definition"

    **Definition**: A subset of AI where computers learn patterns from data rather than being explicitly programmed with rules. You give it examples, and it figures out the patterns.

    **Psychology analogy**: Instead of writing out "if score > 20 on BDI, flag for depression," you give the computer 10,000 patient profiles with outcomes and let it discover which combinations of variables predict depression. It's like regression on steroids --- the computer finds the model for you.

    **Example**: Training a model on adolescent social media use data to predict which patterns of use are associated with body dissatisfaction.

---

### Deep Learning **[Interview Term]**

??? note "Full definition"

    **Definition**: A subset of machine learning that uses neural networks with many layers. Particularly powerful for complex data like images, text, and speech.

    **Psychology analogy**: If machine learning is like running a regression, deep learning is like running a very complex structural equation model with dozens of latent variables and pathways --- it can capture intricate, nonlinear relationships, but it's harder to interpret.

    **Example**: A deep learning model that analyzes Instagram images to classify body-related content and detect potentially harmful appearance-focused messaging.

---

### Algorithm

??? note "Full definition"

    **Definition**: A set of step-by-step instructions for solving a problem. In ML, it's the specific mathematical procedure used to learn patterns from data.

    **Psychology analogy**: Think of it like a statistical procedure. "Run a t-test" is an algorithm --- a defined sequence of steps that takes data in and gives a result out. "Run a random forest" is just a different algorithm.

    **Example**: Logistic regression is an algorithm. So is random forest. They're different procedures for the same general goal --- finding patterns in data.

---

### Model **[Interview Term]**

??? note "Full definition"

    **Definition**: The output of running an algorithm on data. Once trained, a model can make predictions on new data it hasn't seen before.

    **Psychology analogy**: This is exactly like a fitted regression model. After you run `lm()` in R, the resulting object with its coefficients IS the model. In ML, same concept --- you train it, and the trained result is the model.

    **Example**: A model trained on longitudinal data that predicts eating disorder risk trajectories in adolescents based on early risk factors.

---

## Supervised and Unsupervised Learning

### Supervised Learning **[Interview Term]**

???+ note "Full definition"

    **Definition**: ML where you provide both the input data (features) and the correct answers (labels), and the model learns to map inputs to outputs.

    **Psychology analogy**: This is like every regression or classification analysis you've ever run. You have predictors and an outcome, and you're asking the computer to learn the relationship. Supervised = "I'm telling you what the right answer looks like."

    **Example**: Predicting whether an adolescent will develop clinical-level body dissatisfaction (yes/no label) based on early risk factors (features) measured at age 12.

---

### Unsupervised Learning **[Interview Term]**

???+ note "Full definition"

    **Definition**: ML where you provide only the input data --- no labels. The model discovers hidden patterns, groupings, or structure on its own.

    **Psychology analogy**: This is like exploratory factor analysis or cluster analysis. You don't tell the algorithm how many factors to extract or what the clusters should look like --- it finds the structure in the data. Unsupervised = "I'm not telling you the answer; you find the patterns."

    **Example**: Clustering mother-daughter dyads based on communication patterns to discover naturally occurring "communication styles" that weren't predefined by the researcher.

---

### Classification

??? note "Full definition"

    **Definition**: A supervised learning task where the outcome is a category (e.g., yes/no, low/medium/high risk, diagnostic category).

    **Psychology analogy**: Like logistic regression --- you're predicting group membership. Binary classification (two categories) is exactly logistic regression's territory.

    **Example**: Classifying social media posts as promoting "thin ideal," "body positivity," or "neutral" content.

---

### Regression (in ML)

??? note "Full definition"

    **Definition**: A supervised learning task where the outcome is a continuous number.

    **Psychology analogy**: Exactly what you think --- predicting a continuous outcome. The only difference is that in ML, you might use algorithms beyond OLS regression (like random forests or gradient boosting) to make continuous predictions.

    **Example**: Predicting a continuous body dissatisfaction score at age 16 from variables measured at age 12.

---

### Clustering

??? note "Full definition"

    **Definition**: An unsupervised learning technique that groups similar data points together without predefined categories.

    **Psychology analogy**: This is cluster analysis, which you may have encountered. K-means clustering in ML is literally the same k-means you might have used in SPSS.

    **Example**: Identifying subgroups of adolescents with similar patterns of social media use, peer relationships, and body image --- without defining the groups in advance.

---

## Data Concepts and Evaluation

### Features **[Interview Term]**

??? note "Full definition"

    **Definition**: The input variables used to make predictions. In a spreadsheet, these are your columns of data (minus the outcome).

    **Psychology analogy**: These are your predictor variables or independent variables. Exactly the same concept, different word. In ML, we call them "features" because the field grew out of computer science, not statistics.

    **Example**: In a model predicting body dissatisfaction, features might include: age, social media hours per day, frequency of appearance-related comments from mother, peer influence score, BMI.

---

### Labels

??? note "Full definition"

    **Definition**: The outcome variable you're trying to predict in supervised learning.

    **Psychology analogy**: This is your dependent variable or outcome variable. Same thing, different name.

    **Example**: In a classification task, the label might be "clinical eating disorder: yes/no." In a regression task, it might be a continuous body dissatisfaction score.

---

### Training

??? note "Full definition"

    **Definition**: The process of showing a model many examples so it can learn the underlying patterns. The model adjusts its internal parameters to minimize errors on the training data.

    **Psychology analogy**: Like the calibration phase in test development. You administer items to a large sample so the scoring algorithm learns how items relate to the construct. The model "learns" from the calibration data.

    **Example**: Training a text classification model by showing it thousands of social media posts that have been manually coded as "body positive," "body negative," or "neutral."

---

### Training Set / Test Set **[Interview Term]**

??? note "Full definition"

    **Definition**: The training set is the data the model learns from. The test set is held-out data used to evaluate how well the model performs on new, unseen examples.

    **Psychology analogy**: This is cross-validation, which you likely already know. You wouldn't evaluate a measure's predictive validity using the same sample you developed it on --- that would inflate your results. Same principle: train on one portion, test on another.

    **Example**: You split your dataset of 500 adolescents 80/20. The model learns patterns from 400 participants and is evaluated on the remaining 100 to see if those patterns generalize.

---

### Overfitting **[Interview Term]**

??? note "Full definition"

    **Definition**: When a model learns the noise and quirks of the training data so well that it performs poorly on new data. It has memorized rather than learned.

    **Psychology analogy**: This is like capitalizing on chance in your sample. If you run a regression with 50 predictors and 60 participants, you'll get a great R-squared that will never replicate. The model "overfit" your specific sample.

    **Example**: A model that perfectly predicts body image outcomes in your training sample of predominantly White suburban adolescents but fails completely when applied to a diverse urban sample.

---

### Accuracy

??? note "Full definition"

    **Definition**: The percentage of predictions the model got right. Simple but can be misleading with imbalanced data.

    **Psychology analogy**: Like the overall hit rate in a screening measure. If 95% of your sample is non-clinical, a model that always predicts "non-clinical" gets 95% accuracy but is useless.

    **Example**: A model predicting eating disorder diagnosis that is 90% accurate --- but only because 90% of the sample doesn't have an eating disorder.

---

### Precision and Recall **[Interview Term]**

??? note "Full definition"

    **Definition**: **Precision** = of all the cases the model flagged as positive, how many actually were? **Recall** = of all the actual positive cases, how many did the model catch?

    **Psychology analogy**: Precision is like positive predictive value (PPV). Recall is like sensitivity. You already know this tradeoff --- a screening tool can be sensitive (catches everyone who might have the condition, with some false alarms) or specific (only flags people who definitely have it, but misses some).

    **Example**: In an eating disorder screening model --- high recall means you catch most at-risk adolescents (but also flag some who aren't at risk); high precision means the ones you flag are truly at risk (but you miss some who are).

---

### Cross-Validation **[Interview Term]**

??? note "Full definition"

    **Definition**: A technique for evaluating model performance by dividing data into multiple subsets, training on some and testing on others, then averaging results.

    **Psychology analogy**: You already know this concept. K-fold cross-validation is commonly used in scale development (e.g., "we used 10-fold cross-validation to evaluate model fit"). Same exact idea applied more broadly.

    **Example**: Using 5-fold cross-validation to evaluate a predictive model of body dissatisfaction trajectories, ensuring the results are stable across different subsets of your adolescent sample.

---

### Feature Engineering **[Interview Term]**

??? note "Full definition"

    **Definition**: The process of creating new input variables from your raw data to help the model learn better.

    **Psychology analogy**: This is like creating composite scores, computing change scores, or deriving interaction terms before running your analysis. You're transforming raw data into more meaningful variables.

    **Example**: Instead of feeding raw social media timestamps to a model, you engineer features like "average daily screen time," "late-night usage ratio," and "appearance-related content percentage" --- all of which are more psychologically meaningful.

---

### Dimensionality Reduction

??? note "Full definition"

    **Definition**: Techniques that reduce the number of variables in your data while preserving the most important patterns.

    **Psychology analogy**: This IS factor analysis, essentially. Principal Component Analysis (PCA), one of the most common dimensionality reduction techniques, is likely something you've already encountered or used.

    **Example**: Reducing 50 social media behavior variables down to 5 meaningful components before feeding them into a predictive model for body dissatisfaction.

---

## Psychology-Specific AI/ML Terms

### Computational Psychology **[Interview Term]**

??? note "Full definition"

    **Definition**: An approach to psychology that uses computational methods --- including AI/ML, simulation, and mathematical modeling --- to understand human behavior and mental processes.

    **Psychology analogy**: This is the subfield identity you're learning to inhabit. It doesn't mean you have to be a computer scientist --- it means you use computational tools to answer psychological questions.

    **Example**: Using machine learning to identify which combination of maternal, peer, and media factors best predicts the developmental trajectory of body image from early to late adolescence.

---

### Digital Phenotyping **[Interview Term]**

??? note "Full definition"

    **Definition**: Using data from smartphones and wearable devices (GPS, screen time, social media activity, sleep patterns) to characterize human behavior and health.

    **Psychology analogy**: Think of it as passive behavioral observation in the digital age. Instead of behavioral coding in a lab, you're capturing real-world behavior through digital traces.

    **Example**: Tracking adolescents' social media usage patterns, screen time, and app switching behavior to identify digital signatures associated with increasing body dissatisfaction.

---

### Ecological Momentary Assessment (EMA)

??? note "Full definition"

    **Definition**: A method of collecting real-time data from participants in their natural environments, typically via smartphone prompts multiple times per day.

    **Psychology analogy**: You likely already know EMA --- it's widely used in clinical and health psychology. In the AI/ML context, EMA generates the kind of intensive longitudinal data that ML methods are particularly good at analyzing.

    **Example**: Prompting adolescents 5 times daily about body image, mood, and recent social media exposure, then using ML to detect within-person patterns that predict body dissatisfaction spikes.

---

### Explainable AI (XAI) **[Interview Term]**

??? note "Full definition"

    **Definition**: Methods and tools that make AI/ML model predictions understandable to humans. Addresses the "black box" problem --- understanding not just what the model predicts, but why.

    **Psychology analogy**: This is the interpretability concern. In regression, you can look at coefficients and understand what's driving the prediction. Many ML models don't offer that transparency by default. XAI is the push to bring interpretability back.

    **Example**: Using SHAP values to understand which features (maternal communication, peer influence, social media hours) most strongly drive an ML model's prediction of eating disorder risk --- making the model useful for clinicians, not just accurate.

---

### Algorithmic Bias **[Interview Term]**

??? note "Full definition"

    **Definition**: When an AI/ML system produces systematically unfair or prejudiced results, usually because the training data reflects existing societal biases.

    **Psychology analogy**: This is like measurement bias or sampling bias --- but in the data the model learns from. If your training data overrepresents one demographic, the model "learns" that demographic's patterns and performs poorly for others.

    **Example**: A body image classification model trained primarily on content from thin, White women may fail to accurately classify body image content from women of color or plus-size individuals --- perpetuating narrow beauty standards algorithmically.

---

## Quick Reference: Interview-Ready Terms

If you can comfortably define and give an example for these terms, you'll be well-prepared for most AI/ML conversations in psychology job interviews:

| Term | One-Liner |
|------|-----------|
| Machine Learning | Computers learning patterns from data instead of being explicitly programmed |
| Supervised Learning | ML with labeled outcomes --- like regression and classification |
| Unsupervised Learning | ML that finds hidden patterns --- like cluster analysis and factor analysis |
| NLP | Teaching computers to understand and analyze human language |
| Features / Labels | Predictor variables and outcome variables |
| Training/Test Split | Evaluating your model on data it hasn't seen --- cross-validation logic |
| Overfitting | When your model memorizes noise and won't generalize |
| Precision / Recall | PPV and sensitivity --- the tradeoff between false positives and false negatives |
| Computational Psychology | Using computational tools (including AI/ML) to study human behavior |
| Digital Phenotyping | Characterizing behavior through smartphone and wearable data |
| Explainable AI (XAI) | Making ML predictions interpretable and transparent |
| Algorithmic Bias | When ML systems produce unfair results due to biased training data |
| Feature Engineering | Creating meaningful variables from raw data to improve model performance |
