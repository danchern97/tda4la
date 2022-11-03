# Acceptability Judgements via Examining the Topology of Attention Maps (EMNLP 2022)

This repository contains code base for the [paper](https://openreview.net/forum?id=dm_wGpuMfls) which introduces a novel method for language acceptability judjement (LA) based on Topological Data Analysis (TDA).

The role of the attention mechanism in encoding linguistic knowledge has received special interest in NLP. However, the ability of the attention heads to judge the grammatical acceptability of a sentence has been underexplored. This paper approaches the paradigm of acceptability judgments with topological data analysis (TDA), showing that the geometric properties of the attention graph can be efficiently exploited for two standard practices in linguistics: binary judgments and linguistic minimal pairs. Topological features enhance the BERT-based acceptability classifier scores by 8%-24% on CoLA in three languages (English, Italian, and Swedish). By revealing the topological discrepancy between attention maps of minimal pairs, we achieve the human-level performance on the BLiMP benchmark, outperforming nine statistical and Transformer LM baselines. At the same time, TDA provides the foundation for analyzing the linguistic functions of attention heads and interpreting the correspondence between the graph features and grammatical phenomena.

# Dependencies

The code base requires:

 - python 3.8.3
 - matplotlib 3.3.1
 - networkx 2.5.1
 - numpy 1.19.1
 - pandas 1.1.1
 - ripserplusplus 1.1.2
 - scipy 1.5.2
 - sklearn 0.23.2
 - tqdm 4.46.0
 - transformers 4.3.0

# Usage

# Cite us
