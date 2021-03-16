# Exercices-réseaux-de-neurones

** YOU HAVE TO SAVE YOUR CODE FOR THE NEXT SESSION**

In this TD, we are going to use neural network models to perform multiclass classification.
We aim to predict the age of abalone from physical measurements. The age of abalone is determined by cutting the shell through the cone, staining it, and counting the number of rings through a microscope -- a boring and time-consuming task. Other measurements, which are easier to obtain, are used to predict the age. Further information, such as weather patterns and location (hence food availability) may be required to solve the problem.
For the sake of simplicity, we are going to consider that we have 7 category of ages denoted "Class_0" to "Class_6" 


- Download the date from [here](https://drive.google.com/file/d/17mJbjugmT02gSAwDEGQDw703lF9OG2jS/view?usp=sharing) and read it using  `pandas` library and check if there are some missing values
- Normalize the data between 0 and 1 and name the new dataset as *data_scaled*. Scale the data using another scaling method and explain the difference between the two methods in your words.
- Use `sklearn.model_selection` to split your data into training and testing sets where the test set represents 30% of the data
- Use `keras.models` to initialize a sequential neural network object model called **model**. What will be your input dimension. [check this page](https://www.tensorflow.org/api_docs/python/tf/keras/Input)

- What is the function that allows you to add layers to the model [check this page](https://www.tensorflow.org/api_docs/python/tf/keras/Sequential)
- Use `model.layers` to create a **Dense** layer with 10 neurons and **relu** as activation function. Can we use other activation functions ?? Give some examples [check this page](https://www.tensorflow.org/api_docs/python/tf/keras/Model)
- Generate simulated data and visualize the shape of each one after writing functions that encodes them
- Create 2 more layers each one and add them to your model. 
- Create the output layer and add it to your model. Watch out for the choice of the correct activation function for the last layer.
- Compile your model and specify the loss function, the optimizer and the evaluation metrics. Run a command that summarizes your model.
- Use `plot_model` from `tf.keras.utils.vis_utils` to plot visualize your model
- Fit your model and specify the number of epochs
- Use `evalute` method to evaluate your model to get the accuracy and loss
- Use your network to predict the label of the test set
- Find the best hyper parameters combination. You have to test at least two optimizers, two losses, two NN depths, two layer sizes (less than 100) and two types of regularization (you can simplify your code using GridSearchCV class from sklearn library)
- Explain in your words the concept of the two optimizers, the two losses and the two types of regularization  [check this page](https://www.tensorflow.org/api_docs/python/tf/keras/activations)
- Compare the final best prediction on the test then plot the true and predicted values in the same plot
- Save your trained model using the `save` method of your `model` object in a `.h5` format


- Create a function that defines the best model computed above and compile it
- Use the method `fit` of the model object, specify the validations size to 0.3, epochs to 150, batch_size to 100 and save the output in a variable called **history**
that contains the history of the training process (training and validation errors ..) . List all the data in **history**. 
- What is the definition of val_acc, acc, val_loss, loss. Plot val_acc and acc on the same figure. Do the same with loss and val_loss.




Lecture notes:
--------------
- Hugo Larochelle [slides](https://drive.google.com/file/d/1CBPuVOr2mGmiIupXjXta4vx8SzU-pzwH/view?usp=sharing) 
