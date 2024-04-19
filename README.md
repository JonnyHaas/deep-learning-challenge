# deep-learning-challenge
Module 21 Challenge
I choose to complete all of my Notebook coding within Google Colab versus jupyter Notebook as I understood the challenge instructions.  I also downloaded my Notebook back to my local drive and then pushed it to Github for submittal.  It appeared there may be options to push directly from Colab, however I stuck to a known method.

For the Requirements, I completed the following:
- Create a dataframe
- Drop the EIN and Name Columns
- Determine the number of unique values for each column
- Count the data points for each column
- Other value of 276
- Classifications
- Cutoff Value

Compile, Train and Evaulate completed

For the first run I did 10 Epochs and obtained an accuracy of 0.7281 and a loss of 0.5675.

Optimize the Model
For Step 2: I didn't really understand the instructions, so I asked ChatGPT and it generated code which I ran saved the model's weight every 5 epochs.  As the model ran, it appeared teh accuracy was above 0.74, after completion of 100, Epoch 100 showed an accuracy of 0.7416 and a loss of 0.5322.  I then changed the model's weight to every 10 epochs.  The accuracy then went to 0.746 with loss of 0.5273.  Again, I wasn't really sure what I was doing.  I saved the notebook as AlphabetSoupCharity_Optiminzation1 which contains both 5 and 10.

Write a Report on the Neural Network Model
- The purpose of this analysis is to build and optimize a neural network model that predicts whether a charity donation will be used effectively by the recipient organization, based on historical data from Alphabet Soup, a philanthropic organization. The model aims to help Alphabet Soup determine the likelihood of funding success to ensure that donations lead to significant and impactful outcomes.
- The target for the model is 'IS_SUCCESSFUL', which indicates whether the money given to an organization was used effectively.
- 'EIN' and 'NAME' columns were removed from the dataset as they do not contribute to the prediction of grant success. These are identifiers for organizations and do not hold predictive power.
- We determined the number of unique values in each column to identify which features are categorical and require encoding or binning. Columns with a large number of unique entries (greater than 10) were further analyzed to determine the frequency of each unique value. Less frequent categories were binned into an 'Other' category to streamline the model and improve its generalization capabilities.
- The categorical variables were encoded using pd.get_dummies() to transform them into a format suitable for the neural network model.
- The model included all preprocessed feature variables from the dataset.
- The neural network consisted of two hidden layers. The first layer had 80 neurons, and the second had 30 neurons, both using the ReLU activation function for non-linearity.
- The output layer had a single neuron with a sigmoid activation function to predict the binary outcome.
- The model was compiled with the Adam optimizer. It was trained on scaled feature data for 100 epochs.
- The neural network model designed for Alphabet Soup Charity successfully predicts the effective use of funds with an accuracy of 74.6%. While the model performs well, further tuning and experimentation with different architectures might yield even better results.




