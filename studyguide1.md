# Topics
### Preliminary Answers Without Looking at Notes/Slides: 
    1. Given a problem, can you tell if it is supervise vs unsupervised learning or regression vs classification problem?
    Answer: supervised versus unsupervised has to do with the labels. With labels is supervised learning while without labels is unsupervised. Both require outputs (predictions). regression gives scalar output                 f(x) = wx + b while classification's output f(x) is a binary value {0,1}.
    2. Be comfortable with linear regression; how do you define it mathematically? What are the parameters? How do you find optimal parameters?
    Answer: the parameters for linear regression is the set of training data x, the y intercept b (deviation from the line? or a global min/max?), and i am not clear on what w is.  W might be the average cost.                 Gradient descent can be used on the training data to find optimal parameters and this technique can help reduce your loss.
    3. Why do we need cost function? What is gradient decent and why it works? How we update a parameter in each iteration?
    Answer: the loss function is the best metric to evaluate our model as of now. gradient descent adds random noise to our model which update the parameters for the set of data and saves the best value that gave             us the lowest cost.
    4. What is the impact of learning rate on finding the optimal parameter?
    Answer: the models learning rate should improve if you find the optimal parameter(s), but it may be ineffective without them. Therefore, the impact is crucial.
    5. Global vs. local optimum?
    Answer: local optimums confuse the model, you want a single global optimum to ensure your model gives the best predictions
    6. Why do we scale input data?
    Answer: it improves your model by hiding the outliers in your data to not skew your model too much since the set of data is usually very large 
    7. What is feature engineering?
    Answer: it refers to selecting the most appropriate columns from your data to include in your model. This is like a select statement in SQL where you select only that number of columns. However, this is much               different in the techniques applied to get there. You can use a split of train/test data, you must use gradient descent, you can use cross validation k-fold. All of this to get a logical/reasonable                 loss function for your model to make the best predictions. 
    8. Why is vectorization helpful?
    Answer: we can use the dot product and since our training data is large, it is easier and more accessible this way.
    9. Be comfortable with logistic regression; how do you define it mathematically? What are the parameters? How do you find optimal parameters?
    Answer: logistic regression is similar in terms of cost function, gradient descent, etc. however, it does not represent a line and rather categorizes the output into a binary domain {0,1}. 
    10. How are decision boundaries defined in logistic regression? 
    Answer: I think decision bounaries refers to either the threshold of when to categorize the output as 1 or 0. Or it refers to letting the iterations be decided by a while loop until the cost is no longer                   getting much better.
    11. What is overfitting?
    Answer: overfitting happens when you overcomplicate your model to your data. bascially you learn your specific data too well and the cost may be incredibly low on your training model. however when you apply                it to unseen data you may be way off because the model is not general enough. 
    12. What is regularization and how is it helpful?
    Answer: regularization refers to the preprocessing of data to remove outliers and have parameters not over influence the model. 
    13. How does regularization change the cost function and update formula in gradient descent?
    Answer: The training data that is coming into the model is now preprocessed and no one parameters influence should effect the model too much. This may help generalize your model and give you a better loss                  function.
    14. Why train/test split?
    Answer: training data cannot be trusted, so we set apart 20% unseen data as test data. That way we can improve our model and test it against unseen data like it would be in production.
    15. Why train/test/validation split?
    16. What is the right approach in model selection?
    17. What is k-fold CV?
    Answer: k-fold CV is the approach that iteratively k times repeats the process of training and testing the model to find the best cost.
    18. What is bias vs. variance? What is overfitting vs. underfitting?
    Answer: they similarly measure whether you are overcomplicating your model to your data versus is your data too complicated to your model. 
    19. What is a decision tree and how do you train it?
    Answer: A decision tree splits its nodes continuously until the max depth is reached or purity is reached in the node
    20. How is information gain calculated for classification problems? ore regression problems?
    Answer: information gain is calculated using the current layer of nodes in a decision tree and calculating the number of expected / size of (n - 1) node
    21. One-hot encoding?
    Answer: one-hot encoding is splitting one feature into n number of columns where each column's value must be a value equal to 0 or 1. It is called one-hot encoding because the value of the feature is the                   column where the value is 1, all other column values for that row would result in 0. 
    22. What is disadvantage of decision trees? How can this be improved?
    Answer: The algorithm seems more complex and more slow. I am not sure what the true answer is. 
    23. What is bagging?
    24. How does RF work? How does Gradient Boosting work?
    25. What is feature importance in tree ensembles?
