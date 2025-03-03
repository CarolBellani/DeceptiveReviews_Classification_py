# DeceptiveReviews_Classification_py

Two supervised binary classification problems, deceptive/truthful and positive/negative, are analyzed. Logistic, Support Vector Machine and Naïve Bayes are applied with personalized pipelines.

Details: 1600 reviews. https://www.kaggle.com/rtatman/deceptive-opinion-spam-corpus

Explanation of files
=====================

* overall_model_results.xlsx - a summary of all test results, including best model results for each grid search cv, grid search parameters and final results matrix

* Text_Mining_Presentation.pdf - presentation of the project


scripts
=======
1_preprocess1.ipynb - reads "deceptive-opinion.csv" and applies preprocessing steps (including POS tagging) and saves results in "reviews_mod5.csv"

2_test_lr.ipynb - reads "reviews_mod5.csv" and applies logistic regression model to detect decptive opinion and sentiment analysis

2_test_naivebayse.ipynb - reads "reviews_mod5.csv" and applies naive bayes model to detect decptive opinion and sentiment analysis

2_test_svm.ipynb - reads "reviews_mod5.csv" and applies linear and rbf svm models to detect decptive opinion and sentiment analysis

3_POS.ipynb - reads "LIWC2015_mod5.csv" and applies logistic regression on POS columns to detect decptive opinion and sentiment analysis; also use feature union to combine POS columns and TFIDF results detect decptive opinion and sentiment analysis

4_liwc_lr.ipynb - reads "LIWC2015_mod5.csv" and applies logistic regression on LIWC columns to detect decptive opinion and sentiment analysis; also use feature union to combine LIWC columns and TFIDF results detect decptive opinion and sentiment analysis

4_liwc2_svm.ipynb - reads "LIWC2015_mod5.csv" and applies SVM on LIWC columns to detect decptive opinion and sentiment analysis; also use feature union to combine LIWC columns and TFIDF results detect decptive opinion and sentiment analysis

5_final_model_comparison.ipynb - compares model accuracy for deceptive opinion and sentiment analysis using bar graph (using input files "models_decept.csv" and "models_sentiment.csv")


data folder
===========
* deceptive-opinion.csv - original input file from Kaggle
* reviews_mod5.csv - modified input file, including preprocessed columns and POS columns	
* LIWC2015_mod5.csv - added LIWC results to reviews_mod5.csv
* models_decept.csv - model test results for deceptive opinion detection
* models_sentiment.csv - model test results for sentiment analysis

	

output
======

results of the hyperparameters tuning and of the models
