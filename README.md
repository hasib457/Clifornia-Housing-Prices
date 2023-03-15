# Clifornia-Housing-Prices
This problem is in chapter 2 of “Hands-On Machine Learning with Scikit-Learn, Keras and TensorFlow by Aurélien Géron (O’Reilly). Copyright 2019 Aurélien Géron, 978-1-492-03264-9.” In order to enhance my ability and memory, I'm here to reimplement this entire procedure.
## Frame the Problem
​
The task is to use California census data to build a model of housing prices in the state. This data includes metrics such as the population, median income, and median housing price for each block group in California. Block groups are the smallest geographical unit for which the US Census Bureau publishes sample data (a
block group typically has a population of 600 to 3,000 people). We will call them “districts” for short.

1. It is a **supervised learning** task. Because given labeled training examples (each instance comes with the expected output, i.e., the district’s median housing price). 
2. It is a **regression task**. Because asked to predict a value. 
    - More specifically, this is a **multiple regression** problem since the system will use multiple attributes to make a prediction (it will use the district’s population, the median income, etc.). 
    - It is also a **univariate regression** problem since we are only trying to predict a single value for each district. If we were trying to predict multiple values per district, it would be a **multivariate regression** problem. 
3. There is no continuous flow of data coming in the system, there is no particular need to adjust to changing data rapidly, and the data is small enough to fit in memory, so plain **batch learning** should do just fine.
​

## we will work through an example project end to end, pretending to be a recently hired data scientist at a real estate company. Here are the main steps we will go through:
  1. Look at the big picture.
  2. Get the data.
  3. Discover and visualize the data to gain insights.
  4. Prepare the data for Machine Learning algorithms.
  5. Select a model and train it.
  6. Fine-tune the model.
  7. Present the solution.
  8. Launch, monitor, and maintain the system.
