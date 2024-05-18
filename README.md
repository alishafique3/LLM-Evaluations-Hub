# LLM Evaluations Hub

<p>
For an overview of <strong>NeRFs</strong>, checkout the Survey 
<a href="https://example.com">Neural Volume Rendering: NeRF And Beyond</a>, Blog post 
<a href="https://example.com">NeRF Explosion 2020</a> 
and Collection 
<a href="https://example.com">awesome-NeRF</a>
</p>
        

<h2 class="section-title">Overview</h2>
<ul>
<li><a href="#metric">Evaluation Metrics</a></li>
<li><a href="#framework">Frameworks</a></li>
<li><a href="#application">Applications</a></li>
</ul>
        
<div id="metric" class="section">
<h2 class="section-title">Evaluation Metrics</h2>
<h4>ROUGE</h4>
<ul>
<li>Rouge library, used for evaluating summarization and machine translation in natural language processing.  [<a href="https://github.com/pltrdy/rouge/tree/master">github</a>]</li>
</ul>
        
</div>


<!-- Repeat similar blocks for other sections -->
<div id="framework" class="section">
<h2 class="section-title">Frameworks</h2>
<h4>Huggingface datasets</h4>
Datasets provides various common and NLP-specific metrics for you to measure your models performance.<br> 
<code class = "language-python">from datasets import list_metrics
metrics_list = list_metrics()
len(metrics_list)
print(metrics_list)
</code>
<i>output:</i> ['accuracy', 'bertscore', 'bleu', 'bleurt', 'cer', 'comet', 'coval', 'cuad', 'f1', 'gleu', 'glue', 'indic_glue', 'matthews_correlation', 'meteor', 'pearsonr', 'precision', 'recall', 'rouge', 'sacrebleu', 'sari', 'seqeval', 'spearmanr', 'squad', 'squad_v2', 'super_glue', 'wer', 'wiki_split', 'xnli']
<br>
[<a href="https://huggingface.co/docs/datasets/metrics">webpage</a>]
        
<h4>RAGAS</h4>
Ragas is a framework that helps you evaluate your Retrieval Augmented Generation (RAG) pipelines.<br> 
Metrics: Faithfulness, Answer Relevance, Context Precision, Context Relevancy, Context Recall, Context entities recall, Answer semantic similarity, Answer Correctness, and Aspect Critique. <br>
[<a href="https://docs.ragas.io/en/stable/index.html">webpage</a>], [<a href="https://github.com/rajshah4/LLM-Evaluation/blob/main/ragas_quickstart.ipynb">quick start</a>], [<a href="https://colab.research.google.com/drive/1vWeJBXdFEObuihO7Z8ui2CAYkdHQORqo?usp=sharing#scrollTo=Q3fIJM8ebasA">example 1</a>]
<!-- Content for SLAM -->
</div>

<div id="application" class="section">
<h2 class="section-title">Applications</h2>
<h4>Sentiment Analysis</h4>
<ul>
<li>In this tutorial, sentiment task is evaluated using confusion matrix and classification report.  [<a href="https://github.com/rajshah4/LLM-Evaluation/blob/main/Sentiment_LLM.ipynb">github</a>]</li>
</ul>

</div>
