# My_ML_Learnings

## A visual introduction to machine learning
In machine learning, computers apply statistical learning techniques to automatically identify patterns in data. These techniques can be used to make highly accurate predictions.
**Dimensions** in a data set are called features, predictors, or variables. 
Creating a model is also known as **training a model.**

One example of a machine learning method is a **decision tree**. Decision trees look at one variable at a time and are a reasonably accessible (though rudimentary) machine learning method.A decision tree uses if-then statements to define patterns in data.
For example, if a home's elevation is above some number, then the home is probably in San Francisco.
In machine learning, these statements are called **forks**, and they **split** the data into two branches based on some value.
That value between the branches is called a **split point**. Homes to the left of that point get categorized in one way, while those to the right are categorized in another. A split point is the decision tree's version of a *boundary*.

Picking a split point has tradeoffs. At the **best split**, the results of each branch should be as homogeneous (or pure) as possible.We have to minimise the number of **false negatives** and **false positives**.

If you want to find the numbers which are greater than 6
here **True negatives** are 6,5,4,3,2,1,0,-1,-2,...
**True positives** are 7,8,9,10,...
Your algo to find the numbers greater than 6 is giving the below list.
**negatives** are 5,4,3,2,1,*7*,*9*,...
**positives** are 7,10,12,14,*2*,*3*,...
In the above example 7 and 9 are **false negatives.**
2 and 3 are **false positives.**
- False negatives are those values who belongs to positive set but falsely categorised as negative.
- False positives are those values which belongs to negative set but falsely categoriesd as positive.

Additional forks will add new information that can increase a tree's **prediction accuracy**.Splitting one layer deeper, the tree's accuracy improvesto some extent.
You could even continue to add branches until the tree's predictions are 100% accurate, so that at the end of every branch, you will either get 1/0 as result.
These ultimate branches of the tree are called **leaf nodes**. Our decision tree models will classify the results in each leaf node according to which result is in the majority.
**Training data** is the data used to train the model to get accurate  predictions.
To test the tree's performance on new data, we need to apply it to **data points** that it has never seen before. This previously unused data is called **test data**.
How the tree is behaving for unknown data is more important.

Ideally, the tree should perform similarly on both known and unknown data.

**Overfitting** meands our model has learned to treat every detail in the training data as important, even details that turned out to be irrelevant.

### Keypoints:
- Machine learning identifies patterns using statistical learning and computers by unearthing boundaries in data sets. You can use it to   make predictions.
- One method for making predictions is called a decision trees, which uses a series of if-then statements to identify boundaries and       define patterns in the data.
- Overfitting happens when some boundaries are based on on distinctions that don't make a difference. You can see if a model overfits by   having test data flow through the model.
