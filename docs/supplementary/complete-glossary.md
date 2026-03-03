# Complete Glossary: AI/ML Terminology for Psychology Researchers

A comprehensive A-Z reference covering ~65 terms you may encounter when reading AI/ML papers, attending talks, or interviewing for positions that mention computational methods. Each entry includes a plain-English definition, a psychology analogy or example, and a cross-reference to where the term appears in the course.

For the shorter Week 1 glossary (~30 core terms), see [Week 1 Terminology Glossary](../week-1/glossary.md).

---

## A

### Accuracy
The percentage of predictions a model gets correct. Simple but can be misleading with imbalanced outcomes — e.g., if 95% of your sample is non-clinical, predicting "non-clinical" for everyone gives 95% accuracy but is useless.
*Psychology analogy*: Overall hit rate of a screening measure.
*Course reference*: Week 1 glossary, Week 2 explorations

### Algorithm
A defined set of step-by-step instructions for solving a problem. In ML, it's the specific procedure used to learn patterns from data (e.g., random forest, logistic regression, gradient boosting).
*Psychology analogy*: Like "run a t-test" — a defined statistical procedure with inputs and outputs.
*Course reference*: Week 1 guide, Section 2

### Algorithmic Bias
When an AI/ML system produces systematically unfair results because the training data, labels, or features encode existing societal biases.
*Psychology analogy*: Like measurement bias — if your measure was developed on one population, it may not be valid for others. Same principle applied to ML models.
*Course reference*: Week 1 glossary, Week 2 guide (Ethics section)

### Artificial Intelligence (AI)
The broad field of creating computer systems that can perform tasks typically requiring human intelligence. The umbrella term that encompasses machine learning, deep learning, NLP, robotics, and more.
*Psychology analogy*: Like "psychology" as a discipline — it covers everything from neurons to social behavior. AI covers everything from chess-playing programs to language models.
*Course reference*: Week 1 guide, Section 1

### Attention Mechanism
A component of neural networks (especially transformers) that allows the model to focus on the most relevant parts of input data. The basis for how models like ChatGPT process language.
*Psychology analogy*: Like selective attention in cognitive psychology — the model learns to allocate processing resources to the most informative parts of the input.
*Course reference*: Supplementary context for NLP topics

### AUC (Area Under the Curve)
A metric for evaluating classification models. Measures how well the model distinguishes between classes across all possible thresholds. Ranges from 0.5 (random guessing) to 1.0 (perfect).
*Psychology analogy*: Related to ROC curves used in diagnostic test evaluation. AUC of 0.8 means that 80% of the time, the model correctly ranks a randomly chosen positive case higher than a negative case.
*Course reference*: Extension of Week 2 model evaluation concepts

## B

### Bagging (Bootstrap Aggregating)
Creating multiple models on random subsets of the data and averaging their predictions. Reduces overfitting.
*Psychology analogy*: Like running your analysis on multiple bootstrap samples and averaging results for more stable estimates.
*Course reference*: Underlying concept in random forests (Week 1 guide, Week 2 explorations)

### Batch Size
The number of training examples processed at once before the model updates its parameters. Relevant mainly for deep learning.
*Course reference*: Background concept for deep learning discussion (Week 1 guide)

### Bias (in ML models)
The tendency of a model to make systematic errors. High bias = the model is too simple and misses real patterns (underfitting).
*Psychology analogy*: Like using a linear model to fit a curvilinear relationship — the model is biased toward linearity.
*Course reference*: Concept underlying overfitting/underfitting discussion (Week 1 guide)

### Bias-Variance Tradeoff
The balance between a model being too simple (high bias, misses patterns) and too complex (high variance, memorizes noise). A central concept in ML.
*Psychology analogy*: Like the tradeoff between a parsimonious model (may miss real effects) and a complex model (may capitalize on chance). Same tension, different vocabulary.
*Course reference*: Underlying concept in overfitting discussion (Week 1 guide)

## C

### ChatGPT
A large language model (LLM) developed by OpenAI. Used throughout this course as a learning and drafting tool.
*Course reference*: All exploration activities

### Classification
A supervised learning task where the model predicts a category (e.g., diagnosis present/absent, risk level low/medium/high).
*Psychology analogy*: Logistic regression — you're predicting group membership.
*Course reference*: Week 1 guide, Section 2; Week 2 explorations

### Clustering
An unsupervised learning technique that groups similar data points into clusters without predefined categories.
*Psychology analogy*: Cluster analysis — same concept, same name, same purpose.
*Course reference*: Week 1 guide, Section 2; Week 1 glossary

### Computer-Adaptive Testing (CAT)
Assessment where the algorithm selects the next item based on previous responses, zeroing in on the person's level with fewer items.
*Psychology analogy*: You know this from psychometrics. The GRE is a CAT. The same logic is being applied to clinical measures.
*Course reference*: Week 2 guide, Section 4

### Computational Psychology
Using computational methods — including AI/ML, simulation, and mathematical modeling — to study human behavior and mental processes. The emerging professional identity for psychology researchers who use these tools.
*Course reference*: Week 1 guide, Section 3; Week 1 glossary

### Confusion Matrix
A table showing the counts of true positives, true negatives, false positives, and false negatives for a classification model.
*Psychology analogy*: Like a 2x2 table for a diagnostic test showing hits, misses, false alarms, and correct rejections.
*Course reference*: Week 2 explorations, Step 5

### Cross-Validation
Evaluating model performance by dividing data into multiple subsets (folds), training on some and testing on others, then averaging results.
*Psychology analogy*: You already know this — commonly used in scale development and predictive validity studies.
*Course reference*: Week 1 glossary; Week 2 guide, Section 2

## D

### Data Augmentation
Creating synthetic training examples by modifying existing data (e.g., rotating images, adding noise to text). Helps when you have limited data.
*Psychology analogy*: Like resampling or bootstrapping, but creating new variant examples rather than resampling existing ones.
*Course reference*: Background concept

### Decision Tree
A model that makes predictions by learning a series of if-then rules from the data, creating a flowchart-like structure.
*Psychology analogy*: Like a clinical decision tree — "If symptom A is present AND severity > X, then classify as..."
*Course reference*: Underlying component of random forests (Week 1 guide; Week 2 explorations)

### Deep Learning
A subset of machine learning using neural networks with many layers. Particularly powerful for images, text, and speech.
*Psychology analogy*: Like a complex SEM with dozens of latent variables and pathways — it captures intricate relationships but is harder to interpret.
*Course reference*: Week 1 guide, Section 2; Week 1 glossary

### Digital Phenotyping
Using data from smartphones and wearables (GPS, screen time, social media activity, sleep patterns) to characterize behavior and health.
*Psychology analogy*: Passive behavioral observation in the digital age — capturing real-world behavior through digital traces rather than lab observation.
*Course reference*: Week 1 glossary; Week 2 guide, Section 3

### Dimensionality Reduction
Techniques that reduce many variables to fewer dimensions while preserving important patterns. PCA is the most common.
*Psychology analogy*: This IS factor analysis. PCA in ML is the same PCA from psychometrics.
*Course reference*: Week 1 guide, Section 2; Week 1 glossary

## E

### Ecological Momentary Assessment (EMA)
Collecting real-time data from participants multiple times daily in their natural environment, typically via smartphone.
*Psychology analogy*: You likely already know EMA — it's widely used in clinical and health psychology.
*Course reference*: Week 1 glossary; Week 2 guide, Section 3

### Embedding (Word Embedding)
Representing words as vectors of numbers that capture semantic meaning. Words used in similar contexts get similar vectors (e.g., "happy" and "joyful" would be close in embedding space).
*Psychology analogy*: Like creating a multidimensional scaling map of words based on how similarly they're used — words that are semantically related cluster together.
*Course reference*: NLP context (Week 1 guide, Week 2 guide)

### Ensemble Method
Combining multiple models to produce better predictions than any single model. Random forests and gradient boosting are ensemble methods.
*Psychology analogy*: Like a consensus meeting where multiple clinicians each contribute their assessment and the group decision is usually better than any individual.
*Course reference*: Underlying concept for random forests (Week 1 guide; Week 2 explorations)

### Epoch
One complete pass through the entire training dataset during model training. Deep learning models typically train for many epochs.
*Course reference*: Background concept for deep learning

### Explainable AI (XAI)
Methods and tools for making AI/ML predictions understandable to humans. Addresses the "black box" problem.
*Psychology analogy*: The push to make ML models as interpretable as regression coefficients — knowing not just THAT it predicts, but WHY.
*Course reference*: Week 1 glossary; Week 2 guide, Section 2

## F

### F1 Score
The harmonic mean of precision and recall. Useful when you need to balance both (avoiding false positives AND false negatives).
*Psychology analogy*: Like a composite score that balances sensitivity and PPV for a screening tool.
*Course reference*: Extension of precision/recall (Week 1 glossary)

### Feature
An input variable used to make predictions. In ML, "feature" = "predictor variable" = "independent variable."
*Course reference*: Week 1 guide, Section 1; Week 1 glossary

### Feature Engineering
Creating new, more informative variables from raw data to improve model performance.
*Psychology analogy*: Creating composite scores, change scores, or interaction terms before analysis — transforming raw data into more psychologically meaningful variables.
*Course reference*: Week 1 glossary

### Fine-Tuning
Taking a pre-trained model and training it further on a specific dataset for a specific task.
*Psychology analogy*: Like adapting a well-validated measure to a new population — you start with something that works broadly and refine it for your context.
*Course reference*: Background NLP concept

## G

### Generalization
A model's ability to perform well on new, unseen data — not just the data it was trained on.
*Psychology analogy*: Like external validity — does your finding replicate in a new sample?
*Course reference*: Core concept underlying train/test split (Week 1 guide; Week 2 explorations)

### Gradient Boosting
An ensemble method that builds models sequentially, with each new model focusing on correcting the errors of previous ones.
*Psychology analogy*: Like iterative peer review — each round of revision addresses remaining weaknesses. Popular implementations: XGBoost, LightGBM.
*Course reference*: Week 1 guide, Section 2; Week 2 guide, Section 2

### Ground Truth
The actual, correct labels in your data. What really happened, as opposed to what the model predicted.
*Psychology analogy*: Like the criterion in criterion-related validity — the "real" outcome against which you validate your predictions.
*Course reference*: Underlying concept for model evaluation

## H

### Hyperparameter
Settings you choose before training a model (e.g., number of trees in a random forest, learning rate). Not learned from data.
*Psychology analogy*: Like choosing the number of factors to extract in EFA, or the number of clusters in cluster analysis — decisions the researcher makes, not the algorithm.
*Course reference*: Background concept for Week 2 explorations

## K

### K-Fold Cross-Validation
Splitting data into K equal parts, training on K-1 parts and testing on the remaining part, rotating through all K folds.
*Psychology analogy*: A specific cross-validation procedure. 10-fold CV is common in both ML and psychometric validation.
*Course reference*: Week 1 glossary (Cross-Validation entry)

## L

### Label
The outcome variable in supervised learning — what you're trying to predict.
*Psychology analogy*: Your dependent variable / outcome variable. Same thing, different word.
*Course reference*: Week 1 guide, Section 1; Week 1 glossary

### Large Language Model (LLM)
A very large neural network trained on massive amounts of text data. ChatGPT, Claude, and Gemini are LLMs.
*Course reference*: Background context; used as tools throughout the course

### LASSO (Least Absolute Shrinkage and Selection Operator)
A regression technique that adds a penalty to force some coefficients to exactly zero — effectively performing variable selection automatically.
*Psychology analogy*: Like running a regression that automatically decides which predictors to keep and which to drop. Useful when you have many potential predictors.
*Course reference*: Week 1 guide, Section 2

### Latent Dirichlet Allocation (LDA)
A topic modeling algorithm that discovers abstract topics across a collection of documents.
*Psychology analogy*: Like computational thematic analysis — the algorithm finds clusters of words that tend to co-occur and groups them as "topics."
*Course reference*: Week 2 guide, Section 1 (NLP context)

## M

### Machine Learning (ML)
A subset of AI where computers learn patterns from data rather than being explicitly programmed. The core focus of this course.
*Course reference*: Week 1 guide, Section 1; Week 1 glossary

### Model
The output of training an algorithm on data. Once trained, a model can make predictions on new data.
*Psychology analogy*: Exactly like a fitted regression model — the object that contains the learned patterns.
*Course reference*: Week 1 guide, Section 1; Week 1 glossary

## N

### Natural Language Processing (NLP)
The branch of AI focused on enabling computers to understand, interpret, and generate human language.
*Psychology analogy*: Automated qualitative coding and text analysis at scale.
*Course reference*: Week 1 guide, Section 2; Week 1 glossary; Week 2 guide, Section 1

### Neural Network
A computational system loosely inspired by biological neurons, consisting of layers of interconnected nodes that transform input data into predictions.
*Psychology analogy*: Not really like biological neurons despite the name — think of it as layers of mathematical transformations that can learn complex patterns.
*Course reference*: Week 1 guide, Section 2

## O

### Overfitting
When a model learns the noise and quirks of training data so well that it performs poorly on new data. It has memorized rather than learned.
*Psychology analogy*: Capitalizing on chance — like getting a great R-squared from a model with too many predictors relative to sample size.
*Course reference*: Week 1 guide, Section 2; Week 1 glossary; Week 2 explorations

## P

### Precision
Of all the cases the model flagged as positive, how many actually were positive?
*Psychology analogy*: Positive predictive value (PPV).
*Course reference*: Week 1 glossary; Week 2 explorations

### Prediction (in ML)
Using a trained model to estimate outcomes for new, unseen data.
*Psychology analogy*: Like using a regression equation to predict outcomes for new patients — but potentially with more complex, nonlinear models.
*Course reference*: Week 2 guide, Section 2

### Pre-training
Training a model on a large, general dataset before fine-tuning it for a specific task. Most LLMs are pre-trained on internet text.
*Course reference*: Background concept for understanding ChatGPT and NLP tools

## R

### Random Forest
An ensemble method that builds hundreds of decision trees on random subsets of data and has them vote on the prediction.
*Psychology analogy*: 500 clinicians, each seeing a random subset of patient information, all voting on the diagnosis. The crowd wisdom is usually better than any individual.
*Course reference*: Week 1 guide, Section 2; Week 2 guide, Section 2; Week 2 explorations

### Recall (Sensitivity)
Of all the actual positive cases, how many did the model correctly identify?
*Psychology analogy*: Sensitivity — the same concept you know from diagnostic test evaluation.
*Course reference*: Week 1 glossary; Week 2 explorations

### Regression (in ML)
A supervised learning task where the model predicts a continuous number (as opposed to a category).
*Course reference*: Week 1 guide, Section 2; Week 1 glossary

### Regularization
Adding a penalty to prevent a model from becoming too complex and overfitting. LASSO and Ridge regression are regularized versions of linear regression.
*Psychology analogy*: Like parsimony in model selection — penalizing complexity to favor simpler, more generalizable models.
*Course reference*: Week 1 guide (LASSO/Ridge); Week 2 guide, Section 2

### Reinforcement Learning
ML where an agent learns by interacting with an environment and receiving rewards or penalties.
*Psychology analogy*: Operant conditioning — the model learns through trial and error with positive and negative reinforcement.
*Course reference*: Week 1 guide, Section 2

### ROC Curve
A graph showing the tradeoff between true positive rate (sensitivity) and false positive rate across different classification thresholds.
*Psychology analogy*: ROC curves are used in diagnostic test evaluation in clinical psychology — same concept applied to ML model evaluation.
*Course reference*: Extension of model evaluation concepts (Week 2)

## S

### Sentiment Analysis
An NLP technique that determines the emotional tone of text (positive, negative, neutral, or more nuanced categories).
*Psychology analogy*: Like having a research assistant code the emotional valence of open-ended responses — automated and scalable.
*Course reference*: Week 1 guide, Section 2; Week 1 glossary

### SHAP Values (SHapley Additive exPlanations)
A method from game theory that explains individual predictions by showing how much each feature contributed to pushing the prediction higher or lower.
*Psychology analogy*: Like getting individual beta coefficients for each person — understanding not just what the model predicts, but what drove that specific prediction.
*Course reference*: Week 2 guide, Section 2 (XAI discussion)

### Supervised Learning
ML where you provide both input data and correct answers (labels), and the model learns the mapping between them.
*Psychology analogy*: Every regression and classification analysis you've run. You have predictors and outcomes; the model learns the relationship.
*Course reference*: Week 1 guide, Section 2; Week 1 glossary

## T

### Test Set
Data held out from training, used only for final model evaluation. The model never sees this data during learning.
*Psychology analogy*: Like a holdout sample for cross-validation — the new data you test your model on.
*Course reference*: Week 1 glossary; Week 2 explorations

### Text Mining
Extracting useful information and patterns from large amounts of text data.
*Psychology analogy*: Turbocharged content analysis — counting, categorizing, and finding patterns in text at scale.
*Course reference*: Week 1 glossary

### tidymodels
A collection of R packages for machine learning that follows tidyverse design principles. The primary ML framework used in this course.
*Course reference*: Week 2 explorations (hands-on); Week 2 guide; Week 3 templates

### Topic Modeling
An unsupervised NLP technique that discovers abstract "topics" across a collection of documents.
*Psychology analogy*: Computational thematic analysis — finding recurring themes across texts without predefined codes.
*Course reference*: Week 1 glossary; Week 2 guide, Section 1

### Training Set
The data used to teach the model — the examples it learns from.
*Psychology analogy*: The calibration or development sample.
*Course reference*: Week 1 glossary; Week 2 explorations

### Transformer
The neural network architecture underlying modern language models (GPT, BERT, Claude). Excels at processing sequential data like text.
*Course reference*: Background concept for understanding modern NLP and LLMs

### Transfer Learning
Using knowledge learned from one task to help with a different but related task. The basis for fine-tuning pre-trained models.
*Psychology analogy*: Like generalizing findings from one population or context to inform predictions in a related one.
*Course reference*: Background concept for NLP applications

## U

### Underfitting
When a model is too simple to capture the real patterns in the data. The opposite of overfitting.
*Psychology analogy*: Like using a correlation when the real relationship is curvilinear — your model is too simple and misses real effects.
*Course reference*: Complement to overfitting discussion (Week 1 guide)

### Unsupervised Learning
ML where the model receives only input data (no labels) and discovers hidden structure, patterns, or groupings on its own.
*Psychology analogy*: Exploratory factor analysis and cluster analysis — you don't tell the algorithm the answer; it finds the patterns.
*Course reference*: Week 1 guide, Section 2; Week 1 glossary

## V

### Validation Set
A subset of training data used to tune model settings (hyperparameters) during development. Distinct from the test set, which is reserved for final evaluation.
*Psychology analogy*: Like a development subsample — you use it to refine your approach before the final test.
*Course reference*: Extension of train/test concepts

### Variable Importance
A measure of how much each feature contributes to a model's predictions. Available for random forests, gradient boosting, and via XAI methods for other models.
*Psychology analogy*: Like standardized beta weights in regression — but available for more complex models.
*Course reference*: Week 2 explorations, Step 6; Week 2 guide, Section 2

## W

### Weight (in neural networks)
The numerical parameters that a neural network learns during training. Analogous to coefficients in regression.
*Course reference*: Background concept for neural network discussion

---

## Translate This: CS Jargon to Psychology Language

| CS / ML Term | Psychology Equivalent |
|---|---|
| Features | Predictor variables / IVs |
| Labels | Outcome variable / DV |
| Training | Model fitting / calibration |
| Training set | Development sample |
| Test set | Holdout / validation sample |
| Overfitting | Capitalizing on chance |
| Cross-validation | Cross-validation (same term) |
| Classification | Logistic regression / group prediction |
| Clustering | Cluster analysis |
| Dimensionality reduction | Factor analysis / PCA |
| Hyperparameters | Researcher-specified settings (like # of factors) |
| Ground truth | Criterion / gold standard |
| Precision | Positive predictive value (PPV) |
| Recall | Sensitivity |
| Bias (model) | Systematic error / lack of fit |
| Variance (model) | Instability across samples |
| Regularization | Penalizing model complexity / parsimony |
| Feature engineering | Computing derived variables / composites |
| Ensemble | Committee / aggregated judgment |
| Pipeline | Analysis workflow / processing steps |
| Deployment | Putting into clinical use / real-world application |
| Epoch | One pass through the data |
| Fine-tuning | Adapting to a specific population/context |
| Generalization | External validity / replication |
