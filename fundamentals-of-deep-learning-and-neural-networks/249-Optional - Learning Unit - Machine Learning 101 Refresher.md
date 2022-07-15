## Learning Objectives

* What is Machine Learning?
* Input and Target Variables
* Train and Test Sets
* Types of Algorithms

## The ABC of Machine Learning

### What is Machine Learning?

* Machine learning allows systems to automatically learn and improve from experience without being explicitly programmed.
* It allows computers to discover hidden and valuable insights
* In a nutshell, Machine Learning is a new way of communicating your wishes to a computer.

### Where is Machine Learning used?
* Fraud detection - Eg: Credit card fraud detection. It will help us to detect whether a transaction is fraudulent or not.
* Email spam filtering - Eg: Helps categorize whether a particular email should go in the inbox or the spam box.
* Recommendation engines - Eg: E-commerce platforms like Amazon can recommend you a similar product based on your previously browsed list of products and many more!!!

### What is a Machine Learning (ML) model?

For now, let's consider it a Magical box that helps us predict what we want. In the below case, we want to predict whether an incoming email should land in our inbox or the spam folder. We will discuss more about ML models soon.






![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_832e78e729054fc1844698be4b6a6075.png)






## Keywords in ML

Let's understand some keywords in ML! The same terminologies will be used in Deep Learning. It is thus crucial to understand them properly:

### Features or Variables

These are the most common terms we will come across from now on. Features and Variables are the same in a dataset; they are often interchangeably used. So there is no need to worry about it!



![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_a2567e05b6de49d8acd27242b49bf659.png)




### Target/Label Variable

* The target variable or label of a dataset is the feature of a dataset about which you want to gain a deeper understanding. It is the variable that is, or should be, the output.

* In detecting spam emails, the label will be the category the email belongs to, i.e., 'spam' or 'not spam'.





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_f8f76e74dd2141e0b6cab54140cce44d.png)







### Predictor/Input Variables

One or more variables used to determine (or predict) the 'Target Variable' are known as Input Variables. They are sometimes called Predictor Variables or Descriptors as well. In the spam detector example, the features could include the following:
* Words in the email text
* Sender's address
* Time of day the email was sent
* Web and graphical content
* Email contains the phrase "congrats you won $1 billion - share your bank details."




![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_d598608ba9084f9389c341df04e40741.png)










### Dependent and Independent Variables
* You've been studying input and output/target variables. Commonly, the input variable is known as the independent variable, and the target variable is known as the dependent variable.
* In a nutshell, our target variable is nothing but a dependent variable. Why dependent? Because the values of this variable are dependent on other variables (i.e., input variables)
* And, our input variables are known as independent variables. Here the values of these variables are not dependent on any other variables.

Let's look at some examples to learn more about them!

* In the below dataset, we might be curious to predict "crime_rate" in the future, so that becomes our target variable (dependent variable) and the rest of the variables become input variables (independent variables) for building a machine learning model.



![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_1405693eefdf47208d3c47a985c8207c.png)





### Another example

* An independent variable is like a knob you can turn - an adjustable thing.
* A dependent variable is what changes when you turn the knob.
* You can change the hours of study, and as a result, the course grade changes.
* That makes the hours of study the independent variable and the course grade the dependent variable.
* Also, hours of study might not be the only factor affecting the course grade. There might be other independent variables like the quality of the books or even the quality of education given by your instructor/teacher.

### Synonyms Recap
Too many synonyms to memorize? Let me put them all down in one place for better understanding:
* Variables = Features
* Input Variables = Attributes = Predictors = Descriptors = Independent Variables
* Target Variables = Labels = Outcomes = Dependent Variables

## Train and Test Sets

### Train and Test Set







![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_03c311cc355c4a4dbc514c0edab15ff9.png)











* To use an analogy, let's say you teach a child to multiply by letting the kid train on the small multiplication table, i.e., everything from $1\times1$ to $9\times9$.
* Next, you test whether the kid can perform the same multiplications. The result is a success. The kid gets it right almost every time.
* What's the problem here?
* You don't know if the kid understands multiplication or has simply memorized the table!







![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_a1deacbc10ad4c72962d940a585f12ad.png)









### Train and Test Dataset

* So what you would do instead is test the kid on multiplications like $11\times12$ outside the table.
* This is precisely why we need to test machine learning models on unseen or test data. Otherwise, we cannot know whether the algorithm has learned a generalizable pattern or has memorized the training data.
* TRAINING DATA: The observations in the training set form the experience that the algorithm uses to learn.
* TEST DATA: The test set is a set of observations used to evaluate the
performance of the model using some performance metric.

No observations from the training set must be included in the test set. If the test set does contain examples from the training set, it won't be easy to assess whether the algorithm has learned to generalize from the training set or has memorized it.

### Train Test Split
* Consider an Example where our Original Dataset has 1000 rows.
* When we build our ML model, we will split our dataset into two parts (70% train data and 30% test data).
* We will train our model on 70% of data, i.e., 700 rows, and then test our model performance on 30% of data, i.e., 300 rows. As discussed above, while testing our model, we will not provide the outcome to our model for the test data although we know the outcome and instead let our model give us the outcome for those 300 rows.
* Later, we will compare the outcome of our model to the actual outcome of our test data to get the accuracy of our model predictions.
* For splitting our data into the training and testing sets, we use the train_test_split method of the sci-kit-learn library.

### Data Splitting
1. We separate the data into input and target variable
2. We further divide them into train and test datasets





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_983b9fb1f97c4ef6bf395bf831d51240.png)






Let's consider the following data with ten entries, and our objective is to predict whether someone has purchased a product or not, i.e., the "ProductPurchase" column = Yes or No.



![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_a618c47f8258469eb88fa04ef7ad939c.png)






Here, Country, Age, and Salary are the Input variables used to predict the target variable - ProductPurchase.

### Separate Input(X) and Target Variables(y)

* We separate the dataset into two new datasets, one with input variables - X (Country, Age, and Salary) and the other with the target variable - y (ProductPurchase).
* X now has the data without the 'ProductPurchase' column (this is achieved with the 'drop' function).
* y, on the other hand, contains only the 'ProductPurchase' column.





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_6a4d0a9ba1554cb38edffbbfa68f10de.png)






### Splitting into train and test datasets!


* We'll now split the X dataset into two sets — X_train and X_test.
* Similarly, we'll split the y dataset into two sets — y_train and y_test.
* test_size: The ratio of the dataset to be used in the test set. If there are 100 rows, 67 rows will be used in the train set and 33 in the test set.
* random_state: It is provided to obtain the same result every time we run the code. It ensures that the train and test set rows remain the same each time.



![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_487b21932f1c441d9f8d161543abc731.png)



Reference here: [ML with Titanic Data](https://github.com/dphi-official/First_ML_Model/blob/master/ML_with_titanic_data.ipynb)

## Types of Algorithms

### Supervised Learning Algorithms

Let's talk about the datasets that have both input variables and target variables (labels for the data)—ranging from predicting the survival rate of a person in the Titanic Dataset, where the Survival Rate is already given, to predicting the House Price according to house characteristics, where the house prices are provided.

The algorithms that work on such datasets are known as Supervised Learning Algorithms.

It is called supervised learning because the process of an algorithm learning from the training dataset can be thought of as a teacher supervising the learning process. We know the correct answers; the algorithm iteratively makes predictions on the training data and is corrected by the teacher. Learning stops when the algorithm achieves an acceptable level of performance.

### Unsupervised Learning Algorithms

Unsupervised learning is where you have unlabeled data (or no
target variable) in the dataset.

Unsupervised Learning Algorithms aim to find some structure in the dataset.

These are called unsupervised learning because, unlike supervised learning, there are no correct answers and there is no teacher. Algorithms are left on their own to discover and present the interesting structure in the data.

### Types of Supervised Learning Algorithms

Supervised Learning can be further divided into two types:
1. Classification
2. Regression

### Classification vs Regression






![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_e8ac5a25e09a471fa6544c0a404c4dd9.png)





To decide whether to use a regression or classification model, the first question you should ask yourself is:

Does your target variable have a continuous value, or is it discrete (binary or multi-class)?

#### Regression

If your answer is continuous values, you're dealing with Regression.

If you're trying to predict quantities like height, income, price, or scores, you should use a model that will output a continuous number.

So if your objective is to determine tomorrow's temperature, you should use a regression model.

#### Classification

Let's come to the second case, where you can see that the target variable is divided into classes. You'll be using Classification.

When the number of classes is 2, it is known as Binary Classification. E.g., Will it be hot or cold tomorrow is a binary classification problem with two categories: Hot and Cold.

When it is more than 2, it is known as Multi-Class Classification. E.g., Classify movies as Good, Average, or Bad according to reviews.





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_b5b78616c1c6409fa7bfc39e252b8895.png)





Understanding your target variable's characteristics is essential before you begin running models and forming predictions.