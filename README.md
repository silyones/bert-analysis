# Sentiment Analysis Mini-Project: BERT vs. RNN vs. LSTM

## Overview
This project compares RNN, LSTM, and BERT for sentiment classification on a tweet dataset (10,000 samples, 3 classes: Negative, Neutral, Positive).

## WorkFlow
![work flow process](https://github.com/silyones/bert-analysis/blob/master/images/wf.png)
### Results
- **RNN**: 68.15% accuracy
- **LSTM**: 74.00% accuracy
- **BERT**: 78.75% accuracy (fine-tuned on GPU)

BERT is the clear winner thanks to Transformers and pretraining!

![Accuracy Comparison](https://github.com/silyones/bert-analysis/blob/master/images/accuracy.png)
<!-- Replace with your plot screenshot, e.g., bar chart showing BERT's lead -->

## Dataset
- Source: https://www.kaggle.com/datasets/kazanova/sentiment140/data (Twitter Sentiment Analysis dataset)
- Preprocessing: Clean URLs, mentions, hashtags; lowercasing; sampling to 10,000 rows.

## Models
- **RNN/LSTM**: Keras Sequential with Embedding + RNN/LSTM + Dense.
- **BERT**: Hugging Face `bert-base-uncased`, fine-tuned with PyTorch.

## Usage
1. Upload dataset to Colab.
2. Run preprocessing.
3. Train BERT on GPU, RNN/LSTM on CPU.
4. Generate plots.

## Visualizations
- Bar, line, pie, and radar charts in `images/` folder.

## Why BERT Wins
Higher accuracy, better handling of context in short, noisy text.

Feel free to fork and experiment! 
#NLP #BERT #DeepLearning
