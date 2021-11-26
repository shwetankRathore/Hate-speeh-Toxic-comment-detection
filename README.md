### Hate Speech / Toxic Comment detection

- The project aims at improving the user experience of using any website for online chats, conversation and posts by flagging and removing the textual material containing hate and toxicity.
- Given any text or paragraph containing a few lines in natural language (such as English), the objective is to classify it as belonging to one of the following categories:- normal, obscene, threatening, insulting, toxic, severely toxic and hate.
- This is a multi-class classification problem as well as a multi-label classification problem, since a post can be abusive in multiple ways. The model will output the probability of the post belonging to each of the categories and based on a certain threshold (which can be tuned as a hyperparameter), a comment may be classified to be belonging to a category/set of categories

### Dataset

The dataset has been taken from Kaggle(https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/data)

It consists of two data files:
- train.csv: Contains comments with their labels (0 or 1).
- preprocessed_data.csv: Obtained after preprocessing train.csv.

Codes are written in .ipynb files, which contain both the code and their outputs:
- Data Visualization (Visualisation.ipynb)
- Data Preprocessing (TextProcessing.ipynb)
- Naive Bayes (Naive-bayes.ipynb)
- SVM - Binary Relevance (SVM.ipynb)
- Logistic Regression - Binary Relevance and Classifier Chains (Logistic_Regression.ipynb)

### Results

We have used AUC_ROC Score to evaluate the performance of the models. These are the results:

Model | Mean AUC_ROC Score
--- | ---
Support Vector Machines (Binary Relevance) | 0.6375
Support Vector Machines (Classifier Chains) | 0.6529
Logistic Regression (Binary Relevance) | 0.6446
Logistic Regression (Classifier Chains) | 0.6446
