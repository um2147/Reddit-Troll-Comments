# Reddit-r/science-Troll-Comments-Classification

Since the dataset was slightly imbalanced, we started by undersampling the data. A baseline bag of words linear model was first used and an precision of 0.66 was obtained.

Next we experimented with some more techniques including Tf-idf vectorizer, character n-gram and grid search over C parameter to fine-tune the BoW model increasing the precision to 0.76.

Through the BOW analysis, we conclude that the logistic regression model with the above parameterts performed best even when compared to models with added features (no. of punctuation, capital lettered words etc.).

A word2vec FastText model was also employed in this classification task. As observed, the word2vec model does not improve the performance compared to the best model that was obtained in the previous part. Hence, BOW model is prefered for the this dataset with our current implementation
