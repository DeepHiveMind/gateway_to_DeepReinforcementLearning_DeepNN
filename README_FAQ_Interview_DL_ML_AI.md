
Q. The most obvious differences between NumPy arrays and TensorFlow Tensors?
 Answer: such as, Tensors can be backed by accelerator memory (like GPU, TPU).Tensors are immutable.
 
Q.We all know that we shouldn’t set the initial weights to zeros, but under what circumstances, we can set them to zeros?

Q.What’s the mathematical priciple of momentum, RMSprop, and Adam?

Q.What’s the difference between those imagenet winner models?

Q.What’s the usage of embedding layer? And why we need this layer?

Q.Why GRU is better than LSTM?

Answer: GRU’s has fewer tensor operations; therefore, they are a little speedier to train then LSTM’s.
The core concept of LSTM’s are the cell state/ like memory, and it’s various gates. To review, the Forget gate decides what is relevant to keep from prior steps. The input gate decides what information is relevant to add from the current step. The output gate determines what the next hidden state should be. 
GRU’s got rid of the cell state and used the hidden state to transfer information. It also only has two gates, a reset gate and update gate.The update gate acts similar to the forget and input gate of an LSTM. It decides what information to throw away and what new information to add. The reset gate is another gate is used to decide how much past information to forget.
Reference- https://towardsdatascience.com/illustrated-guide-to-lstms-and-gru-s-a-step-by-step-explanation-44e9eb85bf21)

Q. You are given a data set. The data set contains many variables, some of which are highly correlated and you know about it. Your manager has asked you to run PCA. Would you remove correlated variables first? Why?

Answer: Chances are, you might be tempted to say No, but that would be incorrect. Discarding correlated variables have a substantial effect on PCA because, in presence of correlated variables, the variance explained by a particular component gets inflated.

For example: You have 3 variables in a data set, of which 2 are correlated. If you run PCA on this data set, the first principal component would exhibit twice the variance than it would exhibit with uncorrelated variables. Also, adding correlated variables lets PCA put more importance on those variable, which is misleading.

 Q. After spending several hours, you are now anxious to build a high accuracy model. As a result, you build 5 GBM models, thinking a boosting algorithm would do the magic. Unfortunately, neither of models could perform better than benchmark score. Finally, you decided to combine those models. Though, ensembled models are known to return high accuracy, but you are unfortunate. Where did you miss?

Answer: As we know, ensemble learners are based on the idea of combining weak learners to create strong learners. But, these learners provide superior result when the combined models are uncorrelated. Since, we have used 5 GBM models and got no accuracy improvement, suggests that the models are correlated. The problem with correlated models is, all the models provide same information.

For example: If model 1 has classified User1122 as 1, there are high chances model 2 and model 3 would have done the same, even if its actual value is 0. Therefore, ensemble learners are built on the premise of combining weak uncorrelated models to obtain better predictions.

Q. You have built a multiple regression model. Your model R² isn’t as good as you wanted. For improvement, your remove the intercept term, your model R² becomes 0.8 from 0.3. Is it possible? How?

Answer: Yes, it is possible. We need to understand the significance of intercept term in a regression model. The intercept term shows model prediction without any independent variable i.e. mean prediction. The formula of R² = 1 – ∑(y – y´)²/∑(y – ymean)² where y´ is predicted value.   

When intercept term is present, R² value evaluates your model wrt. to the mean model. In absence of intercept term (ymean), the model can make no such evaluation, with large denominator, ∑(y - y´)²/∑(y)² equation’s value becomes smaller than actual, resulting in higher R².

Q. After analyzing the model, your manager has informed that your regression model is suffering from multicollinearity. How would you check if he’s true? Without losing any information, can you still build a better model?

Answer: To check multicollinearity, we can create a correlation matrix to identify & remove variables having correlation above 75% (deciding a threshold is subjective). In addition, we can use calculate VIF (variance inflation factor) to check the presence of multicollinearity. VIF value <= 4 suggests no multicollinearity whereas a value of >= 10 implies serious multicollinearity. Also, we can use tolerance as an indicator of multicollinearity.

But, removing correlated variables might lead to loss of information. In order to retain those variables, we can use penalized regression models like ridge or lasso regression. Also, we can add some random noise in correlated variable so that the variables become different from each other. But, adding noise might affect the prediction accuracy, hence this approach should be carefully used.

Q. Is it possible capture the correlation between continuous and categorical variable? If yes, how?

Answer: Yes, we can use ANCOVA (analysis of covariance) technique to capture association between continuous and categorical variables.

Q. Running a binary classification tree algorithm is the easy part. Do you know how does a tree splitting takes place i.e. how does the tree decide which variable to split at the root node and succeeding nodes?

Answer: A classification trees makes decision based on Gini Index and Node Entropy. In simple words, the tree algorithm find the best possible feature which can divide the data set into purest possible children nodes.

Gini index says, if we select two items from a population at random then they must be of same class and probability for this is 1 if population is pure. We can calculate Gini as following:

Calculate Gini for sub-nodes, using formula sum of square of probability for success and failure (p^2+q^2).
Calculate Gini for split using weighted Gini score of each node of that split
Entropy is the measure of impurity as given by (for binary class):

Entropy, Decision Tree

Here p and q is probability of success and failure respectively in that node. Entropy is zero when a node is homogeneous. It is maximum when a both the classes are present in a node at 50% – 50%.  Lower entropy is desirable.

 Q. You are working on a classification problem. For validation purposes, you’ve randomly sampled the training data set into train and validation. You are confident that your model will work incredibly well on unseen data since your validation accuracy is high. However, you get shocked after getting poor test accuracy. What went wrong?

Answer: In case of classification problem, we should always use stratified sampling instead of random sampling. A random sampling doesn’t takes into consideration the proportion of target classes. On the contrary, stratified sampling helps to maintain the distribution of target variable in the resultant distributed samples also.

Q.  You have been asked to evaluate a regression model based on R², adjusted R² and tolerance. What will be your criteria?

Answer: Tolerance (1 / VIF) is used as an indicator of multicollinearity. It is an indicator of percent of variance in a predictor which cannot be accounted by other predictors. Large values of tolerance is desirable.

We will consider adjusted R² as opposed to R² to evaluate model fit because R² increases irrespective of improvement in prediction accuracy as we add more variables. But, adjusted R² would only increase if an additional variable improves the accuracy of model, otherwise stays same. It is difficult to commit a general threshold value for adjusted R² because it varies between data sets. For example: a gene mutation data set might result in lower adjusted R² and still provide fairly good predictions, as compared to a stock market data where lower adjusted R² implies that model is not good.

Q.  Explain machine learning to me like a 5 year old.

Answer: It’s simple. It’s just like how babies learn to walk. Every time they fall down, they learn (unconsciously) & realize that their legs should be straight and not in a bend position. The next time they fall down, they feel pain. They cry. But, they learn ‘not to stand like that again’. In order to avoid that pain, they try harder. To succeed, they even seek support from the door or wall or anything near them, which helps them stand firm.

This is how a machine works & develops intuition from its environment.

Note: The interview is only trying to test if have the ability of explain complex concepts in simple terms.

Q. What is a Bayesian network and how does it relate to AI?

A Bayesian network is a graphical model for probabilistic relationships among a set of variables. It mimics the human brain in processing variables.

Q. What are Constraint Satisfaction Problems?

Constraint Satisfaction Problems (CSPs) are mathematical problems defined as a set of objects the state of which must meet a number of constraints. CSPs are useful for AI because the regularity of their formulation offers a commonality for analyzing and solving problems.

Q. What are some good ways for performing feature selection that do not involve exhaustive search?

Q. How would you evaluate the quality of the clusters that are generated by a run of K-means?

Q.What tools and environments have you used to train and assess models?

Q. Do you have experience with Spark ML or another platform for building machine learning models using very large datasets?

Q. Generative model - https://mlengineer/generative-and-discriminative-models-af5637a66a3

Q. Boltman Machine https://towardsdatascience.com/deep-learning-meets-physics-restricted-boltzmann-machines-part-i-6df5c4918c15

Q. What is Cluster Sampling?
Cluster sampling is a technique used when it becomes difficult to study the target population spread across a wide area and simple random sampling cannot be applied. Cluster Sample is a probability sample where each sampling unit is a collection or cluster of elements.

For eg., A researcher wants to survey the academic performance of high school students in Japan. He can divide the entire population of Japan into different clusters (cities). Then the researcher selects a number of clusters depending on his research through simple or systematic random sampling.

Let’s continue our Data Science Interview Questions blog with some more statistics questions.

 Q.  You are at a Casino. You have two dices to play with. You win $10 every time you roll a 5. If you play till you win and then stop, what is the expected pay-out?
 
 Q. What is the goal of A/B Testing?
It is a statistical hypothesis testing for a randomized experiment with two variables A and B.

The goal of A/B Testing is to identify any changes to the web page to maximize or increase the outcome of an interest. A/B testing is a fantastic method for figuring out the best online promotional and marketing strategies for your business. It can be used to test everything from website copy to sales emails to search ads

An example of this could be identifying the click-through rate for a banner ad.

Q. monte carlo- https://towardsdatascience.com/an-overview-of-monte-carlo-methods-675384eb1694

# A. SOURCES of Deep Learning Interview Questions
https://www.analyticsvidhya.com/blog/2018/05/deep-learning-faq/

https://www.analyticsvidhya.com/blog/2017/01/must-know-questions-deep-learning/

https://www.educba.com/deep-learning-interview-questions/

https://www.youtube.com/watch?v=JYMKEM5c7PU&t=2244s - (Questions are written in Youtube description)

https://mindmajix.com/deep-learning-interview-questions

# B. Tensorflow and Keras 
https://mindmajix.com/tensorflow-interview-questions

https://data-flair.training/blogs/tensorflow-interview-questions/

https://data-flair.training/blogs/tensorflow-interview-questions-and-answers/

# C. AI 
https://medium.com/acing-ai/intel-ai-interview-questions-acing-the-ai-interview-d4a62dbb593c

https://www.simplilearn.com/artificial-intelligence-ai-interview-questions-and-answers-article

https://medium.com/acing-ai/google-ai-interview-questions-acing-the-ai-interview-1791ad7dc3ae

# D.SOURCES of ML Interview questions
https://towardsdatascience.com/data-science-and-machine-learning-interview-questions-3f6207cf040b

https://www.youtube.com/watch?v=t6gOpFLt-Ks&t=5075s

https://www.youtube.com/watch?v=hdZP-83SPqo&list=PLA83b1JHN4lw-BDpu4r__T8cpnvLIJHA-


