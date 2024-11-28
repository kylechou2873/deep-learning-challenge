# deep-learning-challenge  Report
Overview:
Using Neural Network to predict the success of ventures by Alphabet Soup foundation from the charity_data.csv file provided by Alphabet Soup.
Results:
-Data Preprocessing
    -Target of the model is IS_SUCCESSFUL variable from the csv file
    -Features of the model are everything else beside IS_SUCCESSFUL and EIN variables
    -EIN was the only variable that was removed from the dataset
-Compiling, Training, and Evaluating the Model
    -1st hidden layer has num_input_features*2 = 142 neurons with relu activation function
    -2nd hidden layer has same numbers of the neurons as the first layer, or 142, with relu activation function 
    -3rd hidden layer has half the neurons as the 2nd layer rounded up, or 71, with sigmoid activation function
    -Last output layer with sigmoid activation function 

    -The model was able to achieve just about 75% accuracy. 

    -The best increase in performance came from introducing the NAME variable to the model. 

    -Maybe a more targeted activation functions can be used to achieve a better result; however, I have tried a few different ones, between relu, sigmoid, softmax, gelu, etc, in various layers without significant improvement.  