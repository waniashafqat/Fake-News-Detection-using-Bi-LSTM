# Fake News Detection using Bi-directional LSTM on ISOT Dataset.

Fake news detection is a critical task in Natural Language Processing (NLP), aimed at identifying and classifying news articles or text as real or fake. The goal of this project is to develop a deep learning model using Bidirectional Long-Short Term Memory (Bi LSTM) for fake news detection. The importance of this task lies in its potential to combat the spread of misinformation, which can have significant impacts on society, politics, and public health.

![image](https://github.com/waniashafqat/Fake-News-Detection-using-Bi-LSTM/assets/73712563/e9e17279-7f61-4ea7-9acc-3978b4b7d40d)


## Objectives

The project aims to achieve the following objectives:

•	To develop a fake news detection system using Bi LSTM to classify news articles.

•	To evaluate the performance and accuracy of the model.

•	To preprocess the dataset to remove noise and enhance the quality of the input data.

•	To validate the model's effectiveness using the ISOT fake news dataset.

•	To investigate the impact of different word embeddings on the model's performance.

•	To create a robust and scalable solution for real-time fake news detection.

## Dataset

The project employs the ISOT Fake News dataset by the ISOT Research Lab, consisting of a diverse collection of fake news and truthful articles. This dataset is obtained from reputable news sources as well as unreliable sites flagged by Politifact.com. The articles are primarily in English and cover a wide range of topics. The fake news articles were identified using a combination of manual checks and automated techniques.

## Methodology

The project will be developed using the following methodology:

•	Data Collection: Importing the ISOT fake news detection dataset, which consists of real and fake news articles.

•	Data Preprocessing: Cleaning the dataset by removing unnecessary characters, converting text to lowercase, and eliminating inflectional morphemes. Also, cropping the titles into sentences with a maximum length of 42 ensures reasonable input lengths.

•	Word Embedding: Converting the preprocessed text into a format that the deep learning model can handle. Use word embedding techniques such as ‘tokenization’ and ‘padding’ to represent words as numerical vectors.

•	Model Development and Architecture: Sequential model with multiple layers including an embedding layer with an output dimension of 128, followed by a bi-LSTM layer with 128 units. The model also incorporates a dense layer with 128 units and ReLU activation and an output dense layer with sigmoid activation for binary classification. The model is compiled with the Adam optimizer and binary cross-entropy loss.

![image](https://github.com/waniashafqat/Fake-News-Detection-using-Bi-LSTM/assets/73712563/5088411c-7605-4421-a0e9-5a6648179c0e)

•	Model Training: Splitting the dataset into training, evaluation, and testing sets and training the model using the training data and evaluating its performance on the testing data. Performing hyperparameter tuning to optimize the model's performance.

![image](https://github.com/waniashafqat/Fake-News-Detection-using-Bi-LSTM/assets/73712563/4ba629df-5d0e-4e84-93b1-83ea7d1caf66)


 
## Results 
•	The model achieved an accuracy of 99.82% on the test set for fake news detection.

![image](https://github.com/waniashafqat/Fake-News-Detection-using-Bi-LSTM/assets/73712563/63786a45-b842-44f9-9d07-6bbe34de752c)

•	The confusion matrix provides insight into the model's performance in terms of true positive, true negative, false positive, and false negative predictions. 

![image](https://github.com/waniashafqat/Fake-News-Detection-using-Bi-LSTM/assets/73712563/3fcd96a2-c292-4dc0-8b5b-7c0feef089df)

•	The categories are labeled as ‘1’ for real/true news and ‘0’ for fake news. 


