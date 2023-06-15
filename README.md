# deep-learning-challenge ALPHABET-SOUP (first try) (COPY OF ALPHABET SOUP: 2,3,4 try to get better training)
## 1. Overview :
The purpose for this analysis is to help the nonprofit foundation “Alphabet Soup” and provide them a tool that can help it select the applicants for funding with the best chance of success in their ventures. We used machine learning and neural networks, to predict whether applicants will be successful if funded by Alphabet Soup.
We received a CSV provided by the Alphabet Soup’s business team, containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. 

## Results: 
### * Data Preprocessing
    * What variable(s) are the target(s) for your model?
    * Our Target variable was the “IS_SUCCESSFUL” column. 
    * The rest of the variables are the features used to train our model EXCEPT: name and EIN which are solely identification columns. 
    * We removed the columns NAME and EIN due to the lack of importance. This columns are only for identifying the client and provide no relevant information to the machine learning model.
### * Compiling, Training, and Evaluating the Model
    * I chose 1 hidden layer plus input and output layers. 
        * Input: 80 neurons and relu as our activation function
        * 1st hidden layer: 30 neurons and relu as activation function
        * Output layer: 1 neuron and sigmoid as activation function
    * Even though I tried all of the optimization steps: 
        * Dropping more or fewer columns.
        * Creating more bins for rare occurrences in columns.
        * Increasing or decreasing the number of values for each bin.
        * Add more neurons to a hidden layer.
        * Add more hidden layers.
        * Use different activation functions for the hidden layers.
        * Add or reduce the number of epochs to the training regimen.
    * I was not able to achieve the desired model performance. So I decided to leave it with 72% accuracy. 
    * What steps did you take in your attempts to increase model performance?
        * I dropped another column trying to reduce unnecessary noice.
        * Increased and decreased the number of values for each bin, multiple times with different variations.
        * Added more neurons to a hidden layer multiple times with different variations.
        * Added more hidden layers.
        * Used different activation functions for the hidden layers, tanh, relu and sigmoid in different combinations.
        * Added and reduced (50 , 100, and 200) the number of epochs to the training regimen.
## Summary: 
We cleansed the data and tried training the model moving around the different hidden layers, numbers of nods, and changing the bining around. We could not get an accuracy greater than 73%. I would not recommend this model. My recommendation would be to look into automatization of the training. 