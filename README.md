# TensorFlow 2.0 Question Answering
#### Identify the answers to real user questions about Wikipedia page content 
---

### **Description**

The aim of the  [TensorFlow 2.0 Question Answering](https://www.kaggle.com/competitions/tensorflow2-question-answering/overview) project is to develop a machine learning model that can answer questions based on Wikipedia articles. The model is expected to identify the correct long answer to a question from a given Wikipedia article, and then extract the relevant short answer from the long answer. The project is part of a Kaggle competition that provides a dataset of Wikipedia articles, questions, and answers for training and testing the model. The goal is to develop a model that can achieve high accuracy in answering questions from the test set. The dataset is provided by [Google's Natural Questions](https://ai.google.com/research/NaturalQuestions/dataset) , but contains its own unique private test set. A [visualization](https://ai.google.com/research/NaturalQuestions/visualization) of examples shows long and—where available—short answers.

### [Data Fields](https://www.kaggle.com/competitions/tensorflow2-question-answering/data)

- `document_text` - the text of the article in question (with some HTML tags to provide document structure). The text can be tokenized by splitting on whitespace.
- `question_text` - the question to be answered
- `long_answer_candidates` - a JSON array containing all of the plausible long answers.
- `annotations` - a JSON array containing all of the correct long + short answers. Only provided for train.
- `document_url` - the URL for the full article. Provided for informational purposes only. This is NOT the simplified version of the article so indices from this cannot be used directly. The content may also no longer match the html used to generate document_text. Only provided for train.
- `example_id` - unique ID for the sample.

In this project, we have demonstrated how to use TensorFlow 2.0 to build a model that can answer user questions about Wikipedia page content. We have used the Natural Questions dataset to train and evaluate the model.

The project is divided into two parts. In **Part 1**, we focused on **identifying the correct long answer to a question**. We pre-processed the text data, defined the embedding layer using GloVe, and built a model using TensorFlow 2.0. We also evaluated the model and obtained good results.

In **Part 2**, we focused on **extracting the short answer from a long answer**. We defined a separate model for this purpose, which takes the long answer and question as input and predicts the start and end positions of the short answer. We also evaluated this model and obtained good results.

Overall, this project demonstrates the power of deep learning and TensorFlow 2.0 in answering real-world questions using natural language processing. The techniques used in this project can be extended to other applications such as chatbots, virtual assistants, and customer service support.

![Tensor flow 2 0](https://github.com/LavanyaMuthuraman/TensorFlow-2.0-Question-Answering/assets/109660074/ee3ad9f2-c04b-46da-88dd-6b6375a406e4)
