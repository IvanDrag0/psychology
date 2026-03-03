# LLMs as Research Tools

**Prerequisites**: Week 1 guide, Week 2 guide | **Type**: Deep Dive (Optional)

---

## The Shift: From Assistant to Instrument

You have been using ChatGPT or Claude as a brainstorming partner throughout this course --- generating ideas, explaining concepts, stress-testing arguments. That is one way to use a large language model. But there is a second, more consequential way: using an LLM as a systematic research instrument, embedded directly in the research pipeline.

This distinction matters. When you use an LLM as an assistant, you are the instrument and the LLM is a sounding board. When you use an LLM as a research tool, the LLM is doing structured analytic work --- coding transcripts, classifying text, labeling data --- and you are the methodologist designing, validating, and reporting that process. The outputs can appear in your methods section. They get scrutinized by reviewers.

Psychologists are beginning to use LLMs this way at scale, and the practice is developing faster than the norms around it. Understanding what is being done, what is defensible, and what is still contested will position you to discuss these methods in interviews, evaluate them when you encounter them in the literature, and potentially adopt them in your own work.

---

## LLMs as Qualitative Coders

This is the application most immediately relevant to your research. Qualitative coding is time-intensive, expensive to scale, and dependent on human coders who need training, calibration, and agreement checks. LLMs can be prompted to apply a predefined codebook to text --- and in many cases, they do so at a level of agreement with human coders that falls within the range we consider acceptable for trained research assistants.

The workflow looks like this:

1. Develop your codebook manually, grounded in your theoretical framework and pilot data. This step stays with you. An LLM cannot do this --- it requires your expertise in body image research and your knowledge of the literature.
2. Code a meaningful subset of your data by hand. Fifty transcripts is better than five. These become your gold standard.
3. Write a structured prompt that presents the codebook, defines each code precisely, and asks the LLM to apply it to new text. Optionally, include examples of each code (more on this below).
4. Run the LLM on the remaining transcripts.
5. Compare the LLM's codes to your human codes on a held-out subset. Compute inter-rater reliability (Cohen's kappa or ICC, depending on your coding scale).
6. Report the LLM version, your full prompt, and the reliability figures --- just as you would for a human coder.

Why does this matter for your work? If you are studying mother-daughter relationships around body image, you may have interview transcripts or recorded conversation data that would take months to code by hand across a large sample. LLM-assisted coding could compress that timeline significantly while preserving the rigor of your codebook. The scaling potential is real: what might be feasible for 40 participants could become feasible for 400.

What does the evidence say? Several published studies in psychology and adjacent fields have found that LLMs achieve kappa values in the 0.7--0.85 range on structured coding tasks, which is comparable to what we expect from trained human coders. Performance is strongest when the codes are clearly defined, behaviorally anchored, and applied to relatively explicit text content. It degrades on codes that require inference about internal states, cultural knowledge the LLM may not share, or clinical subtlety that depends on context accumulated across a full session.

The limitations matter here. An LLM coding for "appearance commentary" in mother-daughter conversations will likely capture explicit statements. It will be less reliable on implied commentary --- the pause before answering a question about weight, the deflection that functions as criticism, the compliment that carries a conditional edge. Those are exactly the kinds of meaning that your training as a developmental psychologist equips you to recognize. LLM coding is a scalability tool, not a replacement for interpretation.

A concrete example: you could use an LLM to code conversation transcripts for the following codes, applied to each speaking turn:

- **Appearance commentary**: any statement directly referencing physical appearance
- **Body comparison**: explicit or implicit comparison of one body to another
- **Weight talk**: references to weight, size, eating, or dietary behavior
- **Positive appearance feedback**: affirming statements about appearance
- **Critical appearance feedback**: evaluative or negative statements about appearance

These codes are concrete enough that an LLM can apply them reliably. The interpretive layer --- what those patterns mean for daughter body image outcomes across development --- remains yours.

---

## Zero-Shot and Few-Shot Classification

Once you understand qualitative coding with LLMs, two related techniques become accessible.

**Zero-shot classification** means giving the LLM a set of categories and a piece of text, with no examples, and asking it to classify. You are relying entirely on the LLM's pretrained knowledge of language to understand what your categories mean.

> "Classify the following social media post as body-positive, body-negative, or neutral. Post: [text]. Category:"

This works surprisingly well for tasks where the categories map onto common linguistic patterns. It works less well when your categories are theoretically specific in ways that diverge from everyday language use. "Body-positive" as a researcher studying Tylka's conceptualization of body appreciation is not identical to "body-positive" as that phrase is used colloquially. If that distinction matters for your research question --- and it likely does --- you need to either fine-tune your prompt carefully or move to few-shot classification.

**Few-shot classification** means providing three to five labeled examples of each category before asking the LLM to classify new text. You are giving the LLM a local definition of each category through demonstration rather than description alone.

> "Here are examples of body-positive posts: [examples]. Here are examples of body-negative posts: [examples]. Here are examples of neutral posts: [examples]. Now classify the following: [text]. Category:"

Few-shot classification is more reliable than zero-shot for nuanced psychological constructs because it anchors the LLM's interpretation of your categories to your actual operationalization. It is also more expensive --- in tokens, and in the time it takes to select good examples. But for content analysis of social media data or open-ended survey responses, it can replace the initial pass that would otherwise require a team of trained coders working through thousands of posts.

When does this work well? When categories are mutually exclusive, well-defined, and applied to text that is relatively direct in its meaning. When does it struggle? When categories require contextual knowledge (knowing who is speaking to whom, and what their history is), when content is highly ambiguous, and when the LLM's training data may underrepresent the population whose language you are analyzing.

---

## Prompt Engineering as a Research Skill

!!! tip "New to prompt engineering?"
    If you haven't worked through the basics yet, start with [Prompt Engineering Fundamentals](prompt-engineering.md) first. That page covers the general principles — role assignment, context, constraints, output formatting, and iterative refinement. This section builds on those fundamentals and applies them specifically to research-grade use cases where reproducibility and validation matter.

Prompt engineering has a reputation as a soft skill --- a matter of phrasing things nicely. In a research context, it is a methodological skill that requires the same rigor as designing a survey instrument or writing a standardized interview protocol.

In research use, a well-engineered prompt is specific about the construct being measured, defines categories with enough precision to reduce ambiguity, provides examples that anchor the LLM's interpretation, asks for structured output (a code, a rating, a category label), and optionally requests a confidence rating or a brief rationale for the classification.

Here is an example of a research-grade prompt for coding body image content in mother-daughter interaction transcripts:

---

*You are assisting with qualitative coding of mother-daughter conversation transcripts for a psychology research study. Your task is to code each speaking turn using the codebook below.*

*Codebook:*
- *APPEAR: The speaker makes any direct reference to physical appearance, body shape, weight, or size.*
- *COMPARE: The speaker explicitly or implicitly compares one body to another (e.g., "you look like I did at your age" or "other girls your age").*
- *DIET: The speaker references eating, food, dieting, exercise for weight control, or calorie content.*
- *POSITIVE: The speaker gives positive appearance-related feedback (compliments, affirmations).*
- *NEGATIVE: The speaker gives critical, corrective, or negative appearance-related feedback.*
- *NONE: The speaking turn contains no appearance-related content.*

*Instructions: Read the speaking turn carefully. Assign one or more codes from the list above. If multiple codes apply, list all that apply. If no codes apply, assign NONE. Do not assign codes you are uncertain about. After each code, provide a one-sentence rationale.*

*Speaking turn: [insert text here]*

---

Several principles are demonstrated here. The role framing ("You are assisting with qualitative coding") has been shown in some studies to improve consistency. The codes are defined with enough specificity to reduce ambiguity. Rationale is requested, which lets you audit the LLM's reasoning. And the instruction to withhold uncertain codes introduces a form of calibration.

Reproducibility is a genuine challenge. The same prompt submitted to the same LLM can produce different outputs across runs because most LLMs are stochastic by default. When doing research coding, set temperature to 0 if the API allows it (this makes the model deterministic). Document your exact prompt in your methods or supplementary materials --- not a paraphrase, the exact text. Report the specific LLM version and the date of use, because the same model can behave differently across updates. These practices are not yet universal in the literature, but they are what rigorous reviewers will increasingly expect.

---

## LLMs for Data Augmentation

A more technical but increasingly common use: generating synthetic training data when real data is limited, sensitive, or expensive to collect.

Suppose you want to train a text classifier to identify body image content in social media posts, but you only have access to 200 labeled examples --- not enough to train a reliable classifier. You could use an LLM to generate additional synthetic examples of each content type, then train your classifier on the combined real-plus-synthetic dataset. The LLM is not providing data about the world; it is providing plausible language patterns that help the model learn the decision boundaries between your categories.

This approach has genuine value in psychology for populations where data is rare (clinical samples, sensitive topics) or where data collection is constrained by ethics or access. The critical ethical boundary is that synthetic data must be used to develop and train models, not to draw substantive conclusions. You cannot report that a study of synthetic survey responses revealed something about real adolescents. What you can say is that a classifier trained on synthetic data generalized well to real data when validated against a held-out labeled sample.

---

## LLMs as Simulated Participants (and Why to Be Cautious)

A more contested practice: some researchers have explored using LLMs to simulate human responses --- generating what a participant "might say" in an interview, or how a person "might respond" to a survey item. The appeal is obvious. Piloting a 40-item measure on 500 simulated respondents before collecting a single data point from real participants would save enormous time and resources.

The problem is equally obvious. LLMs do not think or feel. Their outputs reflect statistical patterns in training data --- text produced by humans in contexts that may or may not resemble the population you study. An LLM simulating a 15-year-old girl's response to questions about body dissatisfaction is not modeling adolescent psychology; it is generating text that resembles what has been written about adolescent girls' body dissatisfaction in the corpora it was trained on. These are fundamentally different things, and conflating them is a methodological error.

The current consensus in the field is cautious but not prohibitive. Using LLMs to pilot instrument design --- checking whether items are interpreted as intended, identifying ambiguous wording, stress-testing the response format --- is reasonable, with appropriate acknowledgment that the responses are not human data. This is not categorically different from cognitive interviewing with a convenience sample; it is a faster, cheaper, lower-validity version of the same idea. What is not appropriate is treating LLM-generated responses as data about your target population, or using them to make inferences about psychological constructs in real people.

For your work, this means you could use Claude or ChatGPT to pilot your interview protocol --- generate plausible responses to your questions, look for places where the wording seems to produce confused or off-target responses, and revise accordingly. That is a reasonable use. You should not report it as a study.

---

## Reporting Standards

The field is moving toward clearer expectations for how LLM-assisted research should be disclosed. What reviewers and editors will increasingly expect:

**Identify the model.** Report the specific LLM (e.g., GPT-4o, Claude 3.5 Sonnet), its version number if available, the access platform (API vs. ChatGPT interface), and the date of use. Models are updated continuously, and the same model name at different points in time may produce meaningfully different outputs.

**Report your prompts in full.** Include the complete text of every prompt used for data analysis in your supplementary materials. A paraphrase is not sufficient. Other researchers need to be able to replicate your procedure, and that requires the exact prompt.

**Report inter-rater reliability.** If you used an LLM to code or classify data, report agreement between LLM output and human coding using an appropriate statistic. Cohen's kappa is appropriate for nominal codes. Intraclass correlation or weighted kappa is appropriate for ordinal ratings. Do not report LLM-human agreement as if it were human-human agreement --- be clear about what each comparison represents.

**Acknowledge limitations explicitly.** Hallucination risk, training data bias, non-reproducibility across model versions, and the possibility that the LLM's interpretation of your construct diverges from your theoretical operationalization are all legitimate limitations. Reviewers will raise them if you do not.

Linardon (2025) has published guidelines for AI use in eating disorders research that are relevant to your area and worth consulting directly. It is already on the reading list.

---

## What This Means for Your Career

The ability to discuss LLMs-as-research-tools in an interview is a genuine differentiator right now, because most applicants either have not thought about it at all or have thought about it only as a time-saving device. Being able to speak about it as a methodological choice --- with awareness of the validation requirements, the reporting standards, and the limitations --- signals the kind of methodological sophistication that ML-oriented research teams and cross-disciplinary programs value.

A framing that works well in interviews: "I am interested in using LLMs to scale qualitative coding work on mother-daughter interaction transcripts, with rigorous validation against human coding. The LLM handles the volume; the validity of the construct operationalization stays with me."

This framing does three things. It shows you understand the tool. It shows you understand the limits of the tool. And it positions your expertise --- in body image, in adolescent development, in qualitative method design --- as the thing that makes the tool scientifically meaningful. That is exactly the right framing, because it is accurate.

This is also a natural extension of the Exploration 1 exercise from Week 2, where you compared qualitative coding approaches. If you did that exercise and noticed places where your coding and the LLM's coding diverged, those divergences are methodologically informative. They point to the places where your expertise adds what the model cannot provide.

The key message, repeated because it is worth repeating: LLMs do not replace your expertise. They amplify the reach of your expertise. The amplification is only as valid as your design, your validation, and your willingness to scrutinize the output critically. That scrutiny is something only a trained researcher can do, and it is why the method requires you, not instead of you.

---

## Getting Started

The most useful thing you can do with this module is not read it a second time --- it is to run a small experiment.

Take five excerpts from your existing interview or observation data. Code them yourself using your standard codebook. Then write a structured prompt, following the principles in the prompt engineering section above, and ask ChatGPT or Claude to code the same five excerpts. Compare the results excerpt by excerpt, code by code.

If agreement is high --- say, kappa above 0.70 --- you have the seed of a workflow worth developing. The next step would be to test it on a larger held-out set, refine your prompt based on disagreements, and think about how you would report the validation process in a methods section.

If agreement is low, examine the pattern of disagreements carefully. Where does the LLM fail? Does it miss implicit content? Does it apply codes too liberally or too conservatively? Does it show systematic bias toward certain speakers or turn types? Those failures are not just problems to solve --- they are findings about what your expertise contributes that the model cannot replicate. That is worth knowing too.

Either outcome tells you something. And that is how a research tool is supposed to work.

---

*Related modules: [Reading ML Papers](reading-ml-papers.md) for evaluating published LLM-in-research studies. [R Notebooks](r-notebooks.md) for hands-on text analysis.*
