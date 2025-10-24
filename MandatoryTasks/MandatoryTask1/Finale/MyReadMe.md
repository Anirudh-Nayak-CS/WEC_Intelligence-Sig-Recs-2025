# ML System Design 

## Overview 
- This project utilizes a fine-tuned ROBERTA model as the  Closed and Extractive Question and Answer Language model based on provided Context and a T5 model for English-to-French translation.


## System Architecture

- **Component 1**: Fine-tuned Roberta model for [Roberta's Task].

- **Component 2**: Pre-trained T5 model for translation.

- Roberta's output is inputed into T5 model

## Why i chose those T5 models? 

- Since T5 Model is a general text to text transformer which can perform many tasks like translation ,question answering , summarization and much more (it is fairly good at each of them) so I found it quite interesting and chose this model out of curiosity to see how it would fare at the task of translation 

## How to use the system? 

- Load the fine-tuned RoBERTa model [https://huggingface.co/DingyNayak/Roberta].

- Load the T5 model [https://huggingface.co/docs/transformers/en/model_doc/t5].

- Give a question and relevant context. The model (Roberta+ T5) gives the answer in French.