# AlphabetSoup

Analysis

How many neurons and layers did you select for your neural network model? Why?
I selected 3 layers for the neural netword model as the basic network model since it provided a variety of activation functions to obtain weight coefficients for the amount of input variables in the data. The number of neurons indicated were configured per the rule of thumb of taking the number of inputs and times it by 2 or 3 to indicate the number of neurons. The final accuracy obtained was 53% with a loss of 69%. 

Were you able to achieve the target model performance? What steps did you take to try and increase model performance?
I was not able to achieve target model performance. A variety of steps were taken to increase the model performance. I had initially bucketed only one variable that had a large variety of unique categories (Classification) and then went back to bucket a second category with a large amount of unique categories (Application Type). The variables that I initially selected as features were "Is Successful" and "Status" but throughout the modeling target performance iterations, "Status" was not providing any sort of performance impact in the loss and accuracy values. 

To improve the model a variety of steps were taken:
- Input dataset was checked to determine grouping indexes in the density plots that might bucket values at a more effective value. This was done with the goal of minimizing values that might be outliers and bucketing them so as not to impact the model. 
- The amount of neurons was alternated between a factor of 2 times the input values or 3. Smaller numbers were also tested with decreased accuracy and small impact. 
- After testing a variety of activation functions for the hidden layers, Sigmoid functions were the best at producing an increased accuracy level. This is because our values have been normalized to fit the Sigmoid function best. The Tanh would have provided a close second activation function, but did not yield increased accuracy results. Since the comparison logistic regression accuracy tested was so low, the ReLu function also provided similar insight to the Sigmoid function in the model. 

If you were to implement a different model to solve this classification problem, which would you choose? Why?
The RandomForest Classifier as a point of comparison with this dataset would be chosen. One reason is because given the current state of the model, the RandomForest Classifier might be able to better function with the data as it is tabulated and it depends on weak models such as how this one currently is. With this tabulated data, there is a significant amount of forests that can be created and have enough data points to support the creation of a RandomForest function. Finally since the data has been cleaned it could also perform as well as a deep neural network model would. 
