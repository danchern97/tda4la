# Acceptability Judgements via Examining the Topology of Attention Maps. Findings of EMNLP 2022

This repository contains code base for the [paper](https://arxiv.org/abs/2205.09630), which introduces a novel method for linguistic acceptability judgements (LA) based on Topological Data Analysis (TDA).

## Authors
Daniil Cherniavskii*, Eduard Tulchinskii*, Vladislav Mikhailov*, Irina Proskurina*, Laida Kushnareva, Ekaterina Artemova, Serguei Barannikov, Irina Piontkovskaya, Dmitri Piontkovski, and Evgeny Burnaev. 2022. Acceptability Judgements via Examining the Topology of Attention Maps. In Findings of the Association for Computational Linguistics: EMNLP 2022, pages 88–107, Abu Dhabi, United Arab Emirates. Association for Computational Linguistics.

*denotes equal contribution of the authors.

## Abstract
The role of the attention mechanism in encoding linguistic knowledge has received special interest in NLP. However, the attention heads' ability to judge the grammatical acceptability of a sentence has been underexplored. This paper approaches the paradigm of acceptability judgments with topological data analysis (TDA), showing that the topological properties of the attention graph can be efficiently exploited for two standard practices in linguistics: binary judgments and linguistic minimal pairs. Topological features enhance the BERT-based acceptability classifier scores by up to 0.24 Matthew's correlation coefficient score on CoLA in three languages (English, Italian, and Swedish). By revealing the topological discrepancy between attention graphs of minimal pairs, we achieve the human-level performance on the BLiMP benchmark, outperforming nine statistical and Transformer LM baselines. At the same time, TDA provides the foundation for analyzing the linguistic functions of attention heads and interpreting the correspondence between the graph features and grammatical phenomena. 

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
 
 To use RTD, you should install a modified Ripser++ package via `pip install git+https://github.com/ArGintum/RipserZeros.git`.

# Usage

 - To transform the (Swe-/Ita-/-)CoLA dataset to a unified format, use `CoLA preparation.ipynb`

 - To calculate topological features, please refer to our previous work: ["Artificial Text Detection via Examining the Topology of Attention Maps"](https://aclanthology.org/2021.emnlp-main.50.pdf) (EMNLP 2021). This repository also contains the code for classification.

 - To calculate BLiMP, use `Linguistic_minimal_pairs.ipynb`.

# Cite us

```
@inproceedings{cherniavskii-etal-2022-acceptability,
    title = "Acceptability Judgements via Examining the Topology of Attention Maps",
    author = "Cherniavskii, Daniil  and
      Tulchinskii, Eduard  and
      Mikhailov, Vladislav  and
      Proskurina, Irina  and
      Kushnareva, Laida  and
      Artemova, Ekaterina  and
      Barannikov, Serguei  and
      Piontkovskaya, Irina  and
      Piontkovski, Dmitri  and
      Burnaev, Evgeny",
    booktitle = "Findings of the Association for Computational Linguistics: EMNLP 2022",
    month = dec,
    year = "2022",
    address = "Abu Dhabi, United Arab Emirates",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2022.findings-emnlp.7",
    pages = "88--107",
    abstract = "The role of the attention mechanism in encoding linguistic knowledge has received special interest in NLP. However, the ability of the attention heads to judge the grammatical acceptability of a sentence has been underexplored. This paper approaches the paradigm of acceptability judgments with topological data analysis (TDA), showing that the geometric properties of the attention graph can be efficiently exploited for two standard practices in linguistics: binary judgments and linguistic minimal pairs. Topological features enhance the BERT-based acceptability classifier scores by 8{\%}-24{\%} on CoLA in three languages (English, Italian, and Swedish). By revealing the topological discrepancy between attention maps of minimal pairs, we achieve the human-level performance on the BLiMP benchmark, outperforming nine statistical and Transformer LM baselines. At the same time, TDA provides the foundation for analyzing the linguistic functions of attention heads and interpreting the correspondence between the graph features and grammatical phenomena. We publicly release the code and other materials used in the experiments.",
}
```
