# Human vs. AI-Generated Text Detection Project
## Project Overview
This project aims to enhance the detection of AI-generated text by leveraging advanced machine learning models and comparing them against existing approaches. We focus on identifying and improving upon the limitations of current models by introducing a superior model architecture that incorporates the latest advancements in neural networks and natural language processing (NLP).

## Table of Contents
* Motivation
* Methodology
* Results
* Installation
* Contributing
* License
  
## Motivation:
AI-generated content (AIGC) is revolutionizing our world, becoming an increasingly pivotal element in our daily lives. Since ChatGPT's debut in November 2022, leading tech companies have ceaselessly showcased the astonishing capabilities of AIGC, pushing boundaries beyond text and images to video. Yet, its rapid growth brings ethical concerns, notably in authorship and creativity. The increasing reliance on AIGC, particularly in AI-generated text in education, risks impairing students' writing development and compromising future creativity and personalization. While numerous AI text detection applications and websites exist, their accuracy in identifying AI-generated content is not always reliable. Thus, we are interested in developing a more precise classification model.

## Methodology
### Dataset Preparation
We utilized two primary datasets:

* HC3 (Hugging Face: Human ChatGPT Comparison Corpus): Consists of 24.3k Q&A pairs with human and ChatGPT-generated answers.
* DAIGT V2 (Kaggle): Contains diverse texts generated by humans and various large language models (LLMs), including ChatGPT and Google Gen-AI.
These datasets were merged, split for training (80%) and testing (20%), and further divided into validation sets to optimize model performance.

### Models and Techniques
* DistilBERT Tokenization: Utilized for converting text into a model-readable format, experimenting with different max token lengths based on system capabilities and data characteristics.
* GloVe Tokenization: Employed for extracting static word embeddings, optimized for computational efficiency and contextual relevance with a fixed max token length.

### Model Implementations:
* LSTM with Attention: Captures long-term dependencies within texts.
* CNNs for Text Classification: Utilizes GloVe embeddings, with one model focusing on hyperparameter tuning.
* DistilBert for Text Classification: Leverages a pre-trained model from Hugging Face for robust text classification.

### Test Dataset
We used the GEMINI PRO LLM DAIGT Dataset and TweepFake, creating a mixed test set to evaluate the generalization capability of our models across different AI-generated texts.

## Results

![download (4)](https://github.com/SherryKu/Human_VS_AI_Text_Detection_Project/assets/149217676/efe92eb5-a5c1-4ee2-92fd-ec428c6e912e)

![download (5)](https://github.com/SherryKu/Human_VS_AI_Text_Detection_Project/assets/149217676/c9586235-cebb-4f27-9fc1-296993fe5267)

<img width="684" alt="Screenshot 2024-05-08 at 05 45 29" src="https://github.com/SherryKu/Human_VS_AI_Text_Detection_Project/assets/149217676/3a0a9c83-1d10-4b4c-822d-5b879631960d">

## Installation

To set up this project locally for development and testing purposes, follow these steps:

```
  git clone https://github.com/your-repository/ai-text-detection.git
  cd ai-text-detection
  pip install -r requirements.txt
```

## Contributing
Team Members:
Veronica Zhao （The implementation of Vanilla Neural Networks, Feedforward Neural Networks, Convoluntional Neural Networks.) 
Yanchen Zhou（The implementation of Long Short-Term Memory.) 
Sherry Liu （The implementation of DistilBert, RoBERTa, AlBERT) 

## License
Distributed under the MIT License. See LICENSE for more information.
