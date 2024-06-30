# LGontard_Thesis_MSc_IS_DS
Thesis topic: Using Natural Language Processing to Quantify Politicization in Foreign Aid Reports

This repository provides the code related to the Master Thesis on " Using Natural Language Processing to Quantify Politicization in Foreign Aid Reports" at UVA under the supervision of Jelke Bloem.

Abstract:
This paper offers a solution to process unstandardized text in the context of evaluation reports of foreign aid projects, by introducing the use of contextual word embedding to distinguish ideological differences between interventions conducted under Republican and Democratic administrations.
These differences are reflected by politicization. Given the nature of the texts, attempts have been made to quantify this concept using Natural Language Processing (NLP) to avoid relying on experts. 
Current methods generate a quantitative baseline score for reports using a static embedding model, Doc2Vec. Still, such embedding is not able to capture the importance of topics in context, nor to compare the parties' ideologies.Contextual embedding models enable the extraction of politicization scores for keywords and documents.Using Bidirectional Encoder Representations from Transformers (BERT) and its enhanced version, Robustly Optimized BERT Pretraining Approach (RoBERTa), we obtain statistical evidence that our models can distinguish between politicized and non-politicized keywords, leading to a significant correlation between our politicization metric for the reports and ‘silver standard’ scores.

It is structured as follows:

Experiments:
* A comprehensive EDA :
* An implementation of contextualized embeddings using BERT and the variable _Presidential control_: `BERT_institutional_split.ipynb`
* An implementation of contextualized embeddings using BERT and the variable _Institutional control_: `BERT_presidential_split.ipynb` 
* An implementation of contextualized embeddings using RoBERTa and the variable _Presidential control_: `RoBERTa_institutional_split.ipynb`
* An implementation of contextualized embeddings using RoBERTa and the variable _Institutional control_: `RoBERTa_presidential_split.ipynb` 

The artifact of the EDA is the dataset augmented from three variables which are three different ways to split the reports( using the variable _president_start_ (not used in final analysis) and then using the _Institutional control_ and _Presidential control_ and :
* `df_politicization_2_gov_splits.xlsx`
* `df_keywords`

For each of the contextualized embeddings implementation, the artifacts are saved as `xlsx` files:

Keywords:
* `df_keywords_institutional_split_bert.xlsx`
* `df_keywords_presidential_split_bert.xlsx`
* `df_keywords_institutional_split_roberta.xlsx`
* `df_keywords_presidential_split_roberta.xlsx`

Tensors:
* `dict_tensors_institutional_split_bert.xlsx`
* `dict_tensors_presidential_split_bert.xlsx`
* `dict_tensors_institutional_split_roberta.xlsx`
* `dict_tensors_presidential_split_roberta.xlsx`

