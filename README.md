# Exercices-réseaux-de-neurones

The aim of this TD 





- Download and read the data using using `pandas` library and check if there are some missing values
- Normalize the data between 0 and 1 
- Use `sklearn.model_selection` to split your data into training and testing sets where the test set represents 30% of the data
- Use `keras.models` to initialize a sequential neural network object model called **model**. What will be your input dimension. [check this page](https://www.tensorflow.org/api_docs/python/tf/keras/Input)

- What is the function that allows you to add layers to the model [check this page](https://www.tensorflow.org/api_docs/python/tf/keras/Sequential)
- Use `model.layers` to create a **Dense** layer with 10 neurons and **relu** as activation function. Can we use other activation functions?? What are they?? [check this page](https://www.tensorflow.org/api_docs/python/tf/keras/Model)
- Generate simulated data and visualize the shape of each one
- Create 2 more layers each one and add them to your model. 
- Create the output layer and add it to your model. Watch out for the choice of the correct activation function for the last layer.
- Compile your model and specify the loss function, the optimizer and the evaluation metrics. Run a command that summarizes your model.
- Fit your model and specify the number of epochs
- Use `evalute` method to evaluate your model to get the accuracy and loss
- Use your network to predict the label of the test set
- Find the best hyper parameters combination. You have to test at least two optimizers, two NN depths, two layer sizes (less than 100) and two types of regularization (you can simplify your code using GridSearchCV class from sklearn library)
- Explain in your words the concept of the two optimizers and the two types of regularization  [check this page](https://www.tensorflow.org/api_docs/python/tf/keras/activations)
- Compare the final best prediction on the test then plot the true and predicted values in the same plot
