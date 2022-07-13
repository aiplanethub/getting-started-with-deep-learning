# Optional - Basic Maths & Stats



## Learning Objectives
* Linear Algebra
* Basic Statistics



## What is Linear Algebra?
Often the first acquaintance with linear algebra looks something like this:






![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_2f31c5b1a93640a4bbbcabeec8c5bb52.png)








Not very inspiring, right? Two questions immediately arise: where did all this come from, and why is it needed?

**Basic definition:** Linear algebra is a sub-field of mathematics concerned with vectors, matrices, and linear transforms.

### Do You Really Need Linear Algebra?

* It depends on your goal.
* If you just want to use tools from AI and machine learning as a black box, you arguably just need enough math to figure out if your problem fits the models premise.
* But, if you want to develop new ideas, Linear Algebra is your must-learn thing. I don’t mean you need to learn everything concerning math. Doing so you will be stuck at everything and lose motivation towards other more important things like calculus/stats.
* Mathematics in data science and machine learning is not about crunching numbers, but about what is happening, why it’s happening, and how we can play around with different things to obtain the results we want.

### Linear Algebra

* Let’s start with a simple problem.
  * Condition 1: Imagine the price of 2 chocolates and 1 apple is 100 units
  * Condition 2: Similarly imagine, the price of 1 chocolate and 2 apples is 100 units.  
    Now, we want to find the price of 1 chocolate and an apple.
* Suppose the price of 1 chocolate is \$x and the price of an apple is \$y. Values of ‘x’ and ‘y’ can be anything depending on the situation, i.e., ‘x’ and ‘y’ are variables.
* Translating the above information in mathematical form:  
$2x + y = 100$       Equation (1)    
$x + 2y = 100$       Equation (2)

* To find the prices of chocolate and apple, we need the values of ‘x’ and ‘y’ such that it satisfies both the equations.
* The basic problem of linear algebra is to find these values of ‘x’ and ‘y’ which is nothing but the solution to a set of linear equations.

### Graphical Representation of two Equations

![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_d857b39b3b4d4d1db06757cb4160a058.png)

The intersection point is the solution to these two equations.

### Complicating the Problem

* In the earlier example, we had two variables ‘x’ representing the price of a chocolate and ‘y’ representing the price of a apple.
* Now, suppose you are given a set of three conditions with three variables, say
‘x’, ‘y’, and ‘z’, and asked to find the value of three variables.
* The three conditions are given as:  
$x + y + z = 1$       Equation (1)  
$2x + y = 1$         Equation (2)  
$5x + 3y + 2z = 4$           Equation (3)
* By solving the above three equations we can get the values for ‘x’, ‘y’, and ‘z’.
* In Linear Algebra, data is represented in the form of linear equations. These linear equations are in turn represented in the form of matrices and vectors.

### Matrices
* A matrix is a form of representing data in the form of rows and columns. It is a very natural approach to organizing data.
* A real-life example:  
Consider a reactor that needs to be controlled using multiple attributes from various sensors like Pressure (P), Temperature (T), Density (d), etc.





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_2a21d086f85c4cba9243d2e3cead846c.png)





In the matrix above:

- The first column represents Pressure (P)
- The second column represents Temperature (T)
- The third column represents Density (d)
- Each row corresponds to one sample.


### Linear Equations in Matrix Form
* Earlier we had two linear equations:  
$2x + y = 100$       Equation (1)    
$x + 2y = 100$       Equation (2)
* The above two linear equations can be represented in the matrix
form as:  
![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_e747667a65294909ad483aad1d7792a8.png)
* We can get the above two linear equations from the shown matrix equation just by multiplying the two matrices on the left-hand side and equating the corresponding value to the right-hand side.
* Here is nice resource on Matrices for further reading:
https://www.statisticshowto.com/matrices-and-matrix-algebra/

### Additional Resources
* Interested to learn more about linear algebra operations in Machine Learning?
* Check out this helpful resource: https://machinelearningmastery.com/linear-algebra-cheat-sheet-for-machine-learning/

P.S.: Matrix operations like Addition, Multiplication, and Transposing are commonly used in ML.


### Vectors

* Vector is nothing but a one-dimensional matrix.
* For example, [1 2 3 4 5] is a vector. This is known as a row vector. Or,  
${\begin{bmatrix} 1 \\ 2 \\ 3 \\ 4 \\ 5 \end{bmatrix}}$  
is a column vector.

### Derivative As A Concept

Don’t worry if you don’t know what slope means, it’s explained in the video itself:











<iframe width="560" height="315" src="https://www.youtube.com/embed/N2PpRnFqnqY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>












### Derivative As A Slope of Curve








<iframe width="560" height="315" src="https://www.youtube.com/embed/S-dcMvJlMJs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>











## Basic Statistics
### What is Statistics?
* **Statistics:** A branch of mathematics that takes and transforms the data into some useful information which in turn is used to make some decisions.
* Statistics is concerned with
  * Processing and analyzing data
  * Collecting, presenting, and transforming data to assist the decision maker





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_603476c183ed4ce6a394d25b43f27ac3.png)








### What is Data?

Data are facts and statistics collected together for reference or analysis.






![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_3ad06de5177d4d29943680f0455343e5.png)










### Data Types in Statistics
* Categorical
  * Nominal: Doesn’t have an order. For example, the Gender of a person (male or female)
  * Ordinal: Has some order in place. For example, the Grades of students (first division, second division, and third division)
* Numerical
  * Discrete: Discrete Data can only take certain values. They are distinct and separate. Example: the number of students in a class. We can't have half a Student!
  * Continuous: Continuous Data can take any value (within a range). A person's height: could be any value (within the range of human heights), not just certain fixed heights.

Note: we will get used to these terms soon, no need to worry too much about it. Read this article for additional information: https://builtin.com/data-science/data-types-statistics







![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_b54fd7f5c28d436aba3fe7a8256baf6e.png)









### Measures of Central Tendencies
* **Mean**: The mean is the average of a data set. For example, take a list of numbers: $[10, 20, 40, 10, 70]$. Mean = $(10 + 20 + 40 + 10 + 70) / 5 = 30$
* **Median**: The median is the middle of the set of numbers. To find the median, first, we sort the list of numbers: $[10, 10, 20, 40, 70]$. The exact middle number, i.e., 20, is the median.
* **Mode**: The mode is the most common number in a data set. In above list of numbers, 10 has occurred 2 times while other three numbers occurred one time each. So, the mode is 10 here.

Applications of Central Tendencies
MEAN: When you watch a baseball game and you see the player's batting average, that number represents the total number of hits divided by the number of times at bat. In other words, that number is the mean. In school, the final grade you get in a course is usually a mean. This mean represents the total number of points you scored in the class divided by the number of possible points. This is the classic type of average – when your overall performance on many items is evaluated with a single number.
MEDIAN: Although the mean is the most common type of average, the median can also be used to express the average of a group. You may hear about the median salary for a country or city. When the average income for a country is discussed, the median is most often used because it represents the middle of a group. Mean allows very high or very low numbers to sway the outcome but median is an excellent measure of the center of a group of data.
Applications of Central Tendencies
MODE: Imagine that you live in a small town where most of the people are employed by a factory and earn minimum wage. One of the factory owners lives in the town and his salary is in the millions of dollars. If you use a measure like the average to try to compare salaries in the town as a whole, the owner's income would severely throw off the numbers. This is where the measure of mode can be useful in the real world. It tells you what most of the pieces of data are doing within a set of information.
Measures of Dispersion
Range: It is the difference between highest value and the lowest value in the data set.
For a given list of numbers: 10, 20, 40, 10, 70 the range is 70 - 10 = 60.
Variance: The average of the squared differences from the mean. Steps to calculate variance:
Calculate mean (mean is nothing but average)
Find difference of each data from mean
Square all the differences
Take the average of the squares.
Standard Deviation: It shows you how much your data is spread out around the mean. Its symbol is ???? (the greek letter sigma). It is the square root of the variance.
Standard Deviation

Calculating Variance
Steps to calculate variance:
Calculate mean
Find difference of each data from mean
Square all the differences
Take the average of the squares.
Consider the list of numbers: 10, 20, 40, 10, 70.
Mean of the number is 30.
Difference of each data from the mean: -20, -10, 10, -20, 40.
Square of all the differences: 400, 100, 100, 400, 1600
Take the average of the squares:
(400 + 100 + 100 + 400 + 1600) / 5 = 2600 / 5 = 520
That’s it for for this module. Thank you!
Feel free to post any queries in the #help channel on Slack or on the discuss forum