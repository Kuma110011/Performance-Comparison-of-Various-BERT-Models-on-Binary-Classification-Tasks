# Performance Comparison of Various BERT Models on Binary Classification Tasks

Performance Comparison of Various BERT Models on Binary Classification Tasks
This repository contains the code and materials for the paper "Performance Comparison of Various BERT Models on Binary Classification Tasks" by Yunrong Liu and Kuang Ren. The paper investigates the strengths and weaknesses of different BERT-based models (BERT, RoBERTa, XLM, and ALBERT) and compares their performance on binary classification tasks using three datasets: SST, CoLA, and MRPC.

Table of Contents
1.Introduction
2.Datasets
3.Models
4.Setup
5.Usage
6.Results
7.References

## 1. Introduction

The paper aims to provide insights into the performance of BERT-based models in various natural language processing (NLP) tasks, such as sentiment analysis, grammatical error detection, and paraphrase identification. By comparing the models' performance, the study aims to contribute to the development of more effective and efficient NLP solutions.

## 2. Datasets(train, validation, test)

Three datasets were chosen for comparison:

SST(train.tsv, dev.tsv, test.tsv):  
The Stanford Sentiment Treebank dataset consists of movie review sentences with human-annotated sentiment labels.  

CoLA(in_domain_train_processed.tsv, in_domain_dev_processed.tsv, out_of_domain_dev_processed.tsv):  
The Corpus of Linguistic Acceptability dataset consists of English sentences that are grammatically correct or not.  

MRPC(msr_paraphrase_train_edit.tsv, msr_paraphrase_vali_edit.tsv, msr_paraphrase_test2_edit.tsv):   
The Microsoft Research Paraphrase Corpus dataset contains pairs of long sentences, where each pair may be either a paraphrase or not.

## 3. Models

Four prominent language models were selected for comparison:

BERT: Bidirectional Encoder Representations from Transformers  
RoBERTa: A robustly optimized version of BERT  
XLM: Cross-lingual Language Model  
ALBERT: A Lite BERT with parameter reduction techniques  

We campare it from accuracy, precision, runtime and some other field of performance.
## 4. Setup
To set up the environment for running the code, please follow these steps:
1. Clone the repository:
git clone https://github.com/Kuma110011/STAD80_Team_We-donno-whatt-we-doin.git  

2. Create a virtual environment and install the required packages:
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt

## 5. Usage
To fine-tune and evaluate the models on the datasets, run the following command:
python main.py --model [MODEL_NAME] --dataset [DATASET_NAME]

## 6. Results:
The results of the performance comparison:(Accuracy/Precision/Recall/F1


 Model | BERT | ROBERTA	| XLM | ALBERT
 ---- | -----  |----- |----- |----- 
 SST | 0.921/0.922/0.921/0.921 |	0.946/0.946/0.946/0.946|	0.951/0.951/0.951	| 0.897/0.913/0.897/0.896
COLA	|  0.795/0.798/0.703/0.723	| 0.791/0.761/0.737/0.746	| 0.686/0.343/0.500/0.407	| 0.686/0.343/0.500/0.407
MRPC	| 0.749/0.713/0.727/0.718| 0.833/0.824/0.773/0.791| 0.796/0.769/0.741/0.751| 0.727/0.774/0.575/0.554





## LICENSE
[MIT License Copyright (c) 2023 Kuma110011](https://github.com/Kuma110011/STAD80_Team_We-donno-whatt-we-doin/blob/7f2169f32f1f7027de17fc210b5391a9ad37297b/LICENSE)

## Acknowledgment

This project is based on [this repo@YJiangcm](https://github.com/YJiangcm/SST-2-sentiment-analysis)

