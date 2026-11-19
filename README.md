20 Newsgroups Text Classification

This Project - 
1. Classifies newsgroup posts into 20 topic categories using machine learning.
2. Compares Multinomial Naive Bayes and Logistic Regression to see which handles multi-class text better.

Work Process -
1. Data Splitting : 80% training and 20% testing sets.
2. Text Features : Converted raw text into numerical features using TF-IDF vectorization.
3. Models Tested :
  i) Multinomial Naive Bayes (`alpha=1.0`)
 ii)Logistic Regression (`C=1.0`, `penalty='l2'`, `max_iter=1000`)
4. Validation : Used 5-fold Stratified Cross-Validation to check accuracy
                 and macro F1 score reliably across splits[cite: 2, 4].

Results -
1. Multinomial Naive Bayes : 89.95% accuracy and 0.8783 macro F1.
2. Logistic Regression : 98.38% accuracy and 0.9826 macro F1.
3. Takeaway : Logistic Regression performed noticeably better and
              gave more consistent predictions across all 20 categories.

In the Notebook -
  i) Full data loading, cleaning, and TF-IDF preprocessing pipeline.
 ii) Side-by-side 5-fold cross-validation score comparison tables.
iii) Confusion matrix heatmaps for both models.
 iv) A bar chart comparing F1 scores across all 20 topics.

Tools -
Python, 
Pandas, 
NumPy, 
Scikit-Learn,
Matplotlib,
and Seaborn.
