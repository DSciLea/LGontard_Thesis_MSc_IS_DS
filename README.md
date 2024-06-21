# LGontard_Thesis_MSc_IS_DS
Thesis topic: Using Natural Language Processing to Quantify Politicization in Foreign Aid Reports

This repository provides the code related to the Master Thesis on " Using Natural Language Processing to Quantify Politicization in Foreign Aid Reports" at UVA under the supervision of Jelke Bloem.

It is structured as follow:

* A comprehensive EDA
* An implementation of contextualized embeddings using BERT and the variable _Presidential control_ to split the reports between R and D
*  An implementation of contextualized embeddings using BERT and the variable _Institutional control_ to split the reports between R and D
* An implementation of contextualized embeddings using RoBERTa and the variable _Presidential control_ to split the reports between R and D
* An implementation of contextualized embeddings using RoBERTa and the variable _Institutional control_ to split the reports between R and 

The artifacts of the EDA is the dataset augmented from three variables which are three different ways to split the reports( using the variable _president_start_ (not used in final analysis) and then using the _Institutional control_ and _Presidential control_ and :
* `df_politicization_gov_3.xlsx`--> `df_politicization_3_gov_splits.xlsx`

For each of the contextualized embeddings implementation, the artifacts are saved as `xlsx` files:
* `df_keywords_with_pol_score_gov_full_word.xlsx` --> `df_keywords_with_pol_score_inst_control_BERT.xlsx`
* `df_keywords_with_pol_score_gov_full_word_roberta.xlsx`--> `df_keywords_with_pol_score_inst_control_RoBERTa.xlsx`
* `df_keywords_with_pol_score_gov_3_full_words.xlsx` --> `df_keywords_with_pol_score_pres_control_BERT.xlsx`
* `df_keywords_with_pol_score_gov_3_full_word_roberta.xlsx` --> `df_keywords_with_pol_score_pres_control_RoBERTa.xlsx`


TODO:
- change names of the files
- add the final abstract 
