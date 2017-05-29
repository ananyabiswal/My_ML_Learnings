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
## Probabilistic vs Deterministic Model:
A **deterministic mathematical** model is meant to yield a single solution describing the outcome of some "experiment" given appropriate inputs. 
A **probabilistic model** is, instead, meant to give a distribution of possible outcomes (i.e. it describes all outcomes and gives some measure of how likely each is to occur).

****************************************************************************************************************************

## MACHINE LEARNING
 Machine Learning can be termed as a process of inculcating the property of continuous learning and adaption (prediction and forecasting of events or value of variable) in machines. In addition to this the results should move towards realistic and accurate results in due course of time. A very good example would be playing a certain game(eg chess) in which we might win the initial games very easily  but after a couple of games we might even reach a situation where it is near  to impossible to win. The game was not initially designed by developer considering all possible infinite moves but in due course the game learns and applies the deduced learning to win. A similar instance is when initially when we get into production we have little or sometimes no knowledge about the project .We are given KT(learning) and we use it to do the task assigned. When we sometimes are unable to do the work our colleagues rectify it (improvement to get accurate results) and we learn from them. After a certain period of time we are able to solve every problem and we learn ways to solve new challenges by using previous knowledge. Learning is continuous.
  
## WHY MACHINE LEARNING?
Learning of machines are significant when
1) Human expertise is not sufficient and enough (navigating on Saturn)
2) Humans lack the ability to demonstrate their expertise (speech recognition)
3) Solution is stochastic or is temporal (stock market or gold price)
4) Solution needs to be adjusted to specific classes (user biometrics)
  Machine learning is the application of combination of mathematics and statistics to build intelligent machines.
## TYPES OF MACHINE LEARNING
Machine learning can be classified into following types:-
1) Supervised machine learning-
A training set is given with the correct value of the target attribute. Based on this the model generalizes to find the value of the target value based on the change in input variables. This techniques in other words is learning from examples. Regression and classification fall under this category. Example in real life is how a child learns what is red as explained above.
 
2) Unsupervised machine learning-
When the correct value (label) of the attributes is not given it is termed as supervised learning.eg clustering.
This technique can be used to study the purchasing pattern of customers, pattern recognition etc.
 
3) Reinforcement Learning –
This techniques lies between supervised (known target value for training set) and unsupervised machine learning (unknown target value). The machine is told when it is wrong but it is not told how to rectify the issue. It has to use varied and intelligent methods in order to get the correct result. For example you are developer in a project. Tester identifies a bug. He just tells the bug and then you have to rectify it by using various intelligent sources or methods. This is why this technique is sometimes called learning with critic. 
 
4) Evolutionary Learning-
Evolution in biology is also an effective learning process. Organisms accustom their chance of having offspring and improve survival rates. Various algorithms have been developed such as artificial bee colony optimization, swarm optimization, ant colony optimization.
We would now understand regression which is a machine learning technique.
## REGRESSION
This is a widely used technique which proceeds by building an equation to study the relationship between one or more dependent variable and
an independent variable. For example If we want to predict the forest area burnt (target variable/dependent variable) it would depend on a number of various factors such as the rain, season, month, temperature, altitude etc. Thus our main aim would be to construct an equation which would contain the minimum number of dependent attribute that have a high significance in the estimation of the target attribute. The main objective here would be construction of a model which is robust and a highly predictive model.
 
## SIMPLE LINEAR REGRESSION
It is a simple model that is made by considering one dependent (response) Y and one independent variable (regressor) X. The sales of a company depends on the amount of money that is spend on the advertisement. In the above equation Y is the sales and X is the advertisement cost. We can see than there will be an error from the exact sales which is denoted by €.For some value of X (regressor variable) we will get some value of Y (response variable).A very important point to note here is that even if there is no advertisement i.e is the value of X is 0 then also there is some value of sales which is denoted by β0. 
