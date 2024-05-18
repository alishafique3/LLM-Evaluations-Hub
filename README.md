# LLM Evaluations Hub

<p>
This repository is dedicated to the comprehensive list of evaluation tools for large language models (LLMs). It includes a diverse set of evaluation frameworks and performance metrics to assess aspects such as relevance, accuracy, fluency, coherence, readability, coverage, and diversity of generated content.
</p>
        

<h2 class="section-title">Overview</h2>
<ul>
<li><a href="#metric">Evaluation Metrics</a></li>
<li><a href="#framework">Frameworks</a></li>
<li><a href="#human">Human based Evaluations</a></li>
<!--<li><a href="#application">Applications</a></li>  -->
<li><a href="#resource">Useful Resources</a></li>
</ul>
        
<div id="metric" class="section">
<h2 class="section-title">Evaluation Metrics</h2>
<h3>ROUGE</h3>
<ul>
<li>Rouge library, used for evaluating summarization and machine translation in natural language processing.  [<a href="https://github.com/pltrdy/rouge/tree/master">github</a>]</li>
</ul>
        
</div>


<!-- Repeat similar blocks for other sections -->
<div id="framework" class="section">
<h2 class="section-title">Frameworks</h2>
        
<h3>1. Huggingface datasets</h3>
<ul>
<li>
Datasets provides various common and NLP-specific metrics for you to measure your models performance.
</li>
<li>
<i>from datasets import list_metrics<br>
metrics_list = list_metrics()<br>
len(metrics_list)<br>
print(metrics_list)</i>

<code>output:</code> ['accuracy', 'bertscore', 'bleu', 'bleurt', 'cer', 'comet', 'coval', 'cuad', 'f1', 'gleu', 'glue', 'indic_glue', 'matthews_correlation', 'meteor', 'pearsonr', 'precision', 'recall', 'rouge', 'sacrebleu', 'sari', 'seqeval', 'spearmanr', 'squad', 'squad_v2', 'super_glue', 'wer', 'wiki_split', 'xnli']
</li>
<li>
[<a href="https://huggingface.co/docs/datasets/metrics">webpage</a>]
</li>

</ul>


<h3>2. Huggingface evaluate</h3>
Evaluate is a library that makes evaluating and comparing models and reporting their performance easier and more standardized.<br> 
[<a href="https://pypi.org/project/evaluate/">webpage</a>]
        
<h3>3. RAGAS</h3>
<ul>
<li>
Ragas is a framework that helps you evaluate your Retrieval Augmented Generation (RAG) pipelines.
</li> 
<li>        
Metrics: Faithfulness, Answer Relevance, Context Precision, Context Relevancy, Context Recall, Context entities recall, Answer semantic similarity, Answer Correctness, and Aspect Critique.
</li>
<li>
[<a href="https://docs.ragas.io/en/stable/index.html">webpage</a>], [<a href="https://github.com/rajshah4/LLM-Evaluation/blob/main/ragas_quickstart.ipynb">quick start</a>], [<a href="https://colab.research.google.com/drive/1vWeJBXdFEObuihO7Z8ui2CAYkdHQORqo?usp=sharing#scrollTo=Q3fIJM8ebasA">example 1</a>]
</li>
</ul>
<!-- Content for SLAM -->
</div>


<div id="human" class="section">
<h2 class="section-title">Human based Evaluations</h2>
<ul>
<li>Amazon Mechanical Turk to evaluate the model-generated response. It is a crowdsourcing marketplace that makes it easier for individuals and businesses to outsource their tasks [<a href="https://www.mturk.com/">webpage</a>]</li>

<li>Toloka AI can also be used for human feedback to develop, fine-tune, and evaluate LLMs tailored to your needs [<a href="https://toloka.ai/large-language-models/">webpage</a>]</li>

</ul>

</div>


<!--
<div id="application" class="section">
<h2 class="section-title">Applications</h2>
<h3>Sentiment Analysis</h3>
<ul>
<li>In this tutorial, the sentiment task is evaluated using a confusion matrix and classification report.  [<a href="https://github.com/rajshah4/LLM-Evaluation/blob/main/Sentiment_LLM.ipynb">github</a>]</li>
</ul>

</div>   -->


<div id="resource" class="section">
<h2 class="section-title">Useful Resources</h2>
<ul>
<li>Evaluating Large Language Model (LLM) systems: Metrics, challenges, and best practices.  [<a href="https://medium.com/data-science-at-microsoft/evaluating-llm-systems-metrics-challenges-and-best-practices-664ac25be7e5">medium</a>]</li>
        
<li>Evaluation for Large Language Models and Generative AI - A Deep Dive [<a href="https://youtu.be/iQl03pQlYWY?si=JB47_iUMTBbOTCHh">youtube</a>]</li>
        
</ul>
        
</div>
