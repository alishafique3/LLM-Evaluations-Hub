# LLM Evaluations Hub

This repository is dedicated to the comprehensive list of evaluation tools for large language models (LLMs). It includes a diverse set of evaluation frameworks and performance metrics to assess aspects such as relevance, accuracy, fluency, coherence, readability, coverage, and diversity of generated content.

## 1. datasets
- Datasets provide various general and NLP-specific metrics to evaluate the performance of your models.
- Metrics
```python
from datasets import list_metrics
metrics_list = list_metrics()<br>
len(metrics_list)<br>
print(metrics_list)
```
```python
['accuracy', 'bertscore', 'bleu', 'bleurt', 'cer', 'comet', 'coval', 'cuad', 'f1', 'gleu', 'glue', 'indic_glue', 'matthews_correlation', 'meteor', 'pearsonr', 'precision', 'recall', 'rouge', 'sacrebleu', 'sari', 'seqeval', 'spearmanr', 'squad', 'squad_v2', 'super_glue', 'wer', 'wiki_split', 'xnli']
```
- [[homepage](https://huggingface.co/docs/datasets/metrics)]

## 2. evaluate
- Evaluate is a library designed to simplify and standardize the evaluation and comparison of models for text, computer vision, and audio. It provides three types of evaluations: metrics, comparisons, and measurements. Additionally, you can create new evaluation modules and upload them to a dedicated space on the Huggingface Hub.
- Metrics: Evaluate provides access to dozens of popular metrics. It covers a range of evaluation metrics such as text, computer vision, audio, etc. as well as tools to evaluate models or datasets. Comparisons are used to measure the difference between models and measurement metrics are used to evaluate datasets. [[webpage](https://huggingface.co/evaluate-metric)]
- [[homepage](https://huggingface.co/docs/evaluate/index)]

## 3. Ragas
- Ragas is a library that is used to evaluate Retrieval Augmented Generation (RAG) pipelines.
- Metrics: Faithfulness, Answer Relevance, Context Precision, Context Relevancy, Context Recall, Context entities recall, Answer semantic similarity, Answer Correctness, and Aspect Critique.
- [[homepage](https://docs.ragas.io/en/stable/index.html)], [[quick start](https://github.com/rajshah4/LLM-Evaluation/blob/main/ragas_quickstart.ipynb)], [[example_1](https://colab.research.google.com/drive/1vWeJBXdFEObuihO7Z8ui2CAYkdHQORqo?usp=sharing#scrollTo=Q3fIJM8ebasA)]

## 4. TruLens
- TruLens is a library that enables you to objectively assess the quality and effectiveness of your LLM-based applications using feedback functions. It integrates seamlessly into your LLM app development process (such as LangChain or LlamaIndex). You just need to install it and add a couple of lines to your LLM app. You can then monitor any application and evaluate it with the model of your choice using a dashboard. 
- Metrics: Context Relevance, Groundedness, Answer Relevance, Comprehensiveness, Harmful or toxic language, User sentiment, Language mismatch, Fairness and bias, other custom feedback functions you provide, logging human feedback about LLMs performance.
- [[homepage](https://www.trulens.org/)], [[Documentation](https://www.trulens.org/trulens_eval/getting_started/)], [[Quickstart](https://www.trulens.org/trulens_eval/getting_started/quickstarts/quickstart/)]

## 5. Deepeval
- DeepEval is an open-source framework for LLMs that simplifies the process of building and evaluating LLM applications. It allows you to easily "unit test" LLM outputs, similar to Pytest. With over 14+ LLM-evaluated metrics, synthetic dataset generation, and highly customizable metrics covering all use cases, DeepEval supports real-time evaluations in production environments.
- Metrics: G-Eval, Summarization, Faithfulness, Answer Relevancy, Contextual Relevancy, Contextual Precision, Contextual Recall, Ragas, Hallucination, Toxicity, Bias
- Benchmarking:     BIG-Bench Hard, HellaSwag, MMLU (Massive Multitask Language Understanding), DROP, TruthfulQA, HumanEval, GSM8K
- [[homepage](https://github.com/confident-ai/deepeval?tab=readme-ov-file)], [[Documentation](https://docs.confident-ai.com/docs/getting-started)], [[Blogs](https://www.confident-ai.com/blog)]

## 6. LangSmith
- LangSmith is designed to inspect, monitor, and evaluate your LLM application. It also enables you to continuously optimize and deploy with confidence.
- Metrics: Simple Heuristics, AI-assisted: "LLM-as-judge", Log humans feedback
- [[Quickstart](https://docs.smith.langchain.com/)]

## 7. MLflow LLM Evaluate
- MLflow provides an API mlflow.evaluate() to help evaluate your LLMs. It consists of 3 main components; A model to evaluate, metrics, and evaluation data.
- Metrics: It consists of statistical metrics and model-based metrics. It includes answer similarity, answer correctness, answer relevance, faithfulness, rougeL, toxicity, Custom LLM-based metric
- [[Documentation](https://mlflow.org/docs/latest/llms/llm-evaluate/index.html#)]

## 8. OpenAI Evals
- OpenAI Evals offers a framework for evaluating large language models (LLMs) and systems built with them. It includes a registry of pre-existing evaluations to test various aspects of OpenAI models and allows you to create custom evaluations tailored to your specific use cases.
- Metrics: There are two main ways we can evaluate/grade completions; writing some validation logic in code or using the model itself to inspect the answer.
- [[Getting Started](https://cookbook.openai.com/examples/evaluation/getting_started_with_openai_evals)]

## 9. Evidently
- It assists in evaluating, testing, and monitoring data and ML-powered systems across a range of tasks. For predictive tasks, it supports classification, regression, ranking, and recommendations. For generative tasks, it handles chatbots, retrieval-augmented generation (RAGs), Q&A, and summarization. Additionally, it offers data monitoring capabilities, including data quality and data drift assessments for text, tabular data, and embeddings.
- Rule-based. Detect specific words or patterns in your data. ML-based. Use external models to score data (e.g., for toxicity, topic, tone). LLM-as-a-judge. Prompt LLMs to categorize or score texts. [[Metrics](https://docs.evidentlyai.com/get-started/tutorial-llm#id-6.-customize-evaluations)]
- [[Quickstart](https://docs.evidentlyai.com/get-started/quickstart-llm)], [[Tutorial](https://docs.evidentlyai.com/get-started/tutorial-llm)], [[Documentation](https://docs.evidentlyai.com/)]

## 10. Amazon Mechanical Turk
- Amazon Mechanical Turk is a crowdsourcing marketplace that allows individuals and businesses to easily outsource their tasks. It can be used to have humans evaluate model-generated responses based on the HHH (helpful, honest, harmless) alignment criteria.
- Metrics: Human-based feedback on model-generated response 
- [[homepage](https://www.mturk.com/)]

## Useful Resources
- Evaluating Large Language Model (LLM) systems: Metrics, challenges, and best practices [[medium](https://medium.com/data-science-at-microsoft/evaluating-llm-systems-metrics-challenges-and-best-practices-664ac25be7e5)].
- Evaluation for Large Language Models and Generative AI - A Deep Dive [[youtube](https://youtu.be/iQl03pQlYWY?si=JB47_iUMTBbOTCHh)].
        
<!--
<h2 class="section-title">Overview</h2>
<ul>
<li><a href="#metric">Evaluation Metrics</a></li>
<li><a href="#framework">Frameworks</a></li>
<li><a href="#human">Human based Evaluations</a></li>
<li><a href="#application">Applications</a></li>  
<li><a href="#resource">Useful Resources</a></li>
</ul> 
        
<div id="metric" class="section">
<h2 class="section-title">Evaluation Metrics</h2>
<h3>ROUGE</h3>
<ul>
<li>Rouge library, used for evaluating summarization and machine translation in natural language processing.  [<a href="https://github.com/pltrdy/rouge/tree/master">github</a>]</li>
</ul>
        
</div> -->

