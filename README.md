# ml-financial-tweet-sentiment-classifier
The endgoal of this project was to predict the sentiment (negative, neutral or positive) of finance-related tweet using standard machine learning processes and models.

Model used :
- Logistic Regression 
- KNN
- RF
- SVM
- Neural Networks (MLP)
- FinBERT 


We followed a standard machine learning workflow on Python with **scikit-learn** , **PyTorch**, **transformers** :

- **Data Preprocessing** : cleaning actions/tickers , url and special character -> tokenization -> lemmatization -> vectorization (BOW and TF-IDF)
- **Model Implementation** : we first implemented models on binary classifcation task (negative VS non-negative) to evaluate and compare their performance.
- **Model Optimization** : we displayed the importance of hyperparameter tunning and cross-validation steps by comparing MLP and RF algortihms VS their fine-tuned versions
- **Deep Learning Model Implementation** : We used a fine-tuned tweet-sentiment-analysis RoBERTa model from Hugging Face to perform a multiclass classification task. To improve performance we applied a back-translation technique to virtually increase the training pool and have the best performance possible on this set. 
