# Climate Change Stance and Sentiment Analysis

An undergraduate natural language processing project completed for **NLP for Social Science (UCLA, Fall 2024)**.

## Research question

How is the stance expressed in climate change-related tweets associated with the emotional sentiment of their language?

## Approach

- Explored and preprocessed climate change-related tweets with existing stance labels.
- Used the `cardiffnlp/twitter-roberta-base-sentiment-latest` sentiment model through the Hugging Face Inference API to evaluate tweet sentiment.
- Compared sentiment across stance categories using visualizations and statistical tests, including chi-square comparisons.
- Examined a second labeled dataset using ANOVA and post-hoc comparisons to explore whether the relationship appeared in another sample.

## Findings

The analysis found statistically significant associations between climate-change stance and expressed sentiment. Across the visualizations, more positive sentiment tended to be associated with tweets expressing belief in climate change, while more negative sentiment tended to appear in denial-oriented tweets.

These are **associations, not evidence of causation**; conclusions depend on the datasets and the sentiment-labeling method. The notebook also discusses variation and outliers across the samples.

## Files

- [`comm188cfinalproject.ipynb`](comm188cfinalproject.ipynb) — original analysis notebook, with the embedded API credential removed for public sharing.
- [Original project report (PDF)](https://github.com/sibala25/sibala25.github.io/blob/main/12_24_SentimentAnalysis.pdf) — currently hosted in my earlier portfolio repository.

## Reproducing the analysis

This is archived coursework, not a fully reproducible software package. The original notebook uses Google Colab file paths and references external datasets that are not included in this repository. The Hugging Face inference endpoint may also differ from the service available when the project was completed.

**Security note:** An API access token originally stored in the notebook was removed for public sharing. The notebook now reads `HUGGING_FACE_TOKEN` from the environment. Do not commit tokens or private credentials to the repository.
