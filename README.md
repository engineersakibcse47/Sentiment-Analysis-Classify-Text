## Project: Sentiment Analysis with DistilBERT

### Introduction:
Sentiment analysis, also known as opinion mining, is the process of determining the sentiment expressed in a piece of text. It has numerous applications across various industries, including market research, customer feedback analysis, and social media monitoring. In this project, I employed the DistilBERT model, a lightweight version of BERT (Bidirectional Encoder Representations from Transformers), to perform sentiment analysis on IMDb movie reviews.

### Objective:
The primary objective of this project is to develop a sentiment analysis model capable of accurately classifying IMDb movie reviews as either positive or negative.

### Dataset:
I utilized the [IMDb dataset](https://www.kaggle.com/code/lakshmi25npathi/sentiment-analysis-of-imdb-movie-reviews), which contains movie reviews along with their corresponding sentiment labels (positive or negative). The dataset was preprocessed to remove HTML tags, special characters, and numbers using regular expressions.

### Methodology:
Data Preprocessing: Preprocessing involved cleaning the text data by removing HTML tags, special characters, and numbers.
Custom Dataset Creation: I created a custom dataset class using PyTorch, which prepares the text data for input into the DistilBERT model by tokenizing the text and encoding it into input IDs and attention masks.
Model Training: The DistilBERT model for sequence classification was fine-tuned on the IMDb dataset using PyTorch Lightning's Trainer class. The training process involved specifying training arguments such as batch size, learning rate, and number of epochs.
Model Evaluation: I evaluated the trained model using metrics such as accuracy and F1 score on a separate test dataset. Evaluation was performed after each epoch to monitor the model's performance throughout training.
Model Deployment: The trained model was saved for future use in sentiment analysis tasks.

### Results:
After training the DistilBERT model for three epochs, the following results were obtained: `Accuracy: 91.95%`

### Interface:
I created a simple interface for making predictions using the trained model. The interface accepts input text and returns the predicted sentiment label (positive or negative) along with the corresponding probability score.

### Conclusion:
In conclusion, I successfully developed a sentiment analysis model using the DistilBERT architecture, achieving high accuracy and F1 score on IMDb movie reviews. The trained model can be further improved by fine-tuning on larger datasets or incorporating additional preprocessing techniques. This project demonstrates the effectiveness of transformer-based models for natural language processing tasks, particularly sentiment analysis.
