# LLM Evaluations Hub

This repository is dedicated to the comprehensive list of evaluation tools for large language models (LLMs). It includes a diverse set of evaluation frameworks and performance metrics to assess aspects such as relevance, accuracy, fluency, coherence, readability, coverage, and diversity of generated content.

## 1. datasets
- Datasets provide various common and NLP-specific metrics for you to measure your models performance.
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
- Evaluate is a library that makes evaluating and comparing models and reporting their performance easier and more standardized. It has three types of evaluations: Metrics, comparison, and measurement. You can also create new evaluation modules and push them to a dedicated Space in the Huggingface Hub
- Metrics: Evaluate provides access to dozens of popular metrics. It covers a range of modalities such as text, computer vision, audio, etc. as well as tools to evaluate models or datasets. Comparisons are used to measure the difference between models and measurements are tools to evaluate datasets. [[webpage](https://huggingface.co/evaluate-metric)]
- [[homepage](https://huggingface.co/docs/evaluate/index)]

## 3. Ragas
- Ragas is a framework that helps you evaluate your Retrieval Augmented Generation (RAG) pipelines.
- Metrics: Faithfulness, Answer Relevance, Context Precision, Context Relevancy, Context Recall, Context entities recall, Answer semantic similarity, Answer Correctness, and Aspect Critique.
- [[homepage](https://docs.ragas.io/en/stable/index.html)], [[quick start](https://github.com/rajshah4/LLM-Evaluation/blob/main/ragas_quickstart.ipynb)], [[example_1](https://colab.research.google.com/drive/1vWeJBXdFEObuihO7Z8ui2CAYkdHQORqo?usp=sharing#scrollTo=Q3fIJM8ebasA)]

## 4. TruLens
- TruLens is a software tool that helps you to objectively measure the quality and effectiveness of your LLM-based applications using feedback functions. It fits easily into your LLM app dev process (LangChain or LlamaIndex). Simply install and add a couple of lines to your LLM app. Track any application, and evaluate it with the model of your choice. 
- Metrics: Context Relevance, Groundedness, Answer Relevance, Comprehensiveness, Harmful or toxic language, User sentiment, Language mismatch, Fairness and bias, other custom feedback functions you provide, logging human feedback about LLMs performance.
- [[homepage](https://www.trulens.org/)], [[Documentation](https://www.trulens.org/trulens_eval/getting_started/)], [[Quickstart](https://www.trulens.org/trulens_eval/getting_started/quickstarts/quickstart/)]

## 5. Deepeval
- DeepEval is an open-source evaluation framework for LLMs. DeepEval makes it extremely easy to build and iterate on LLM (applications). Easily "unit test" LLM outputs in a similar way to Pytest. 14+ LLM-evaluated metrics, Synthetic dataset generation, Metrics are simple to customize and covers all use cases, Real-time evaluations in production.
- Metrics: G-Eval, Summarization, Faithfulness, Answer Relevancy, Contextual Relevancy, Contextual Precision, Contextual Recall, Ragas, Hallucination, Toxicity, Bias
- Benchmarking:     BIG-Bench Hard, HellaSwag, MMLU (Massive Multitask Language Understanding), DROP, TruthfulQA, HumanEval, GSM8K
- [[homepage](https://github.com/confident-ai/deepeval?tab=readme-ov-file)], [[Documentation](https://docs.confident-ai.com/docs/getting-started)], [[Blogs](https://www.confident-ai.com/blog)]

## 6. LangSmith
- LangSmith is used to inspect, monitor and evaluate your LLM application, so that you can continuously optimize and deploy with confidence. It also support Unit tests.
- Metrics: Simple Heuristics, AI-assisted: "LLM-as-judge", Log humans feedback
- [[Quickstart](https://docs.smith.langchain.com/)]

## 7. MLflow LLM Evaluate
- MLflow provides an API mlflow.evaluate() to help evaluate your LLMs. It consists of 3 main components: A model to evaluate, Metrics, and Evaluation data.
- Metrics: It consists of statistical metrics and model based metrics. It includes answer similarity, answer correctness, answer relevance, faithfulness, rougeL, toxicity, Custom LLM based metric
- [[Documentation](https://mlflow.org/docs/latest/llms/llm-evaluate/index.html#)]

## 8. OpemAI Evals


## 9. Amazon Mechanical Turk
- Amazon Mechanical Turk to evaluate the model-generated response by humans based on HHH (helpful, honest, harmless) alignment criteria. It is a crowdsourcing marketplace that makes it easier for individuals and businesses to outsource their tasks.
- Metrics: Human-based feedback on model generated response 
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

