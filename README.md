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
- [[webpage](https://huggingface.co/docs/datasets/metrics)]

## 2. evaluate
- Evaluate is a library that makes evaluating and comparing models and reporting their performance easier and more standardized.
- [[webpage](https://pypi.org/project/evaluate/)]

## 3. RAGAS
- Ragas is a framework that helps you evaluate your Retrieval Augmented Generation (RAG) pipelines.
- Metrics: Faithfulness, Answer Relevance, Context Precision, Context Relevancy, Context Recall, Context entities recall, Answer semantic similarity, Answer Correctness, and Aspect Critique.
- [[webpage](https://docs.ragas.io/en/stable/index.html)], [[quick start](https://github.com/rajshah4/LLM-Evaluation/blob/main/ragas_quickstart.ipynb)], [[example_1](https://colab.research.google.com/drive/1vWeJBXdFEObuihO7Z8ui2CAYkdHQORqo?usp=sharing#scrollTo=Q3fIJM8ebasA)]

## 4. Amazon Mechanical Turk
- Amazon Mechanical Turk to evaluate the model-generated response by humans based on HHH (helpful, honest, harmless) alignment criteria. It is a crowdsourcing marketplace that makes it easier for individuals and businesses to outsource their tasks.
- [[webpage](https://www.mturk.com/)]

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

