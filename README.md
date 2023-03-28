# Neural_Network_Charity_Analysis
![image](https://user-images.githubusercontent.com/112978144/228309768-3cfc1c2d-196a-4cdc-b335-b7e2716e3fa8.png)


# Overview

In this challenge we were assign to use our knowledge of machine learning and neural networks, to use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

* EIN and NAME—Identification columns

* APPLICATION_TYPE—Alphabet Soup application type

* AFFILIATION—Affiliated sector of industry

* CLASSIFICATION—Government organization classification

* USE_CASE—Use case for funding

* ORGANIZATION—Organization type

*STATUS—Active status

* INCOME_AMT—Income classification

*SPECIAL_CONSIDERATIONS—Special consideration for application

*ASK_AMT—Funding amount requested

* IS_SUCCESSFUL—Was the money used effectively

There were four deliverables in this challenge 
Deliverable 1: Preprocessing Data for a Neural Network Model
Deliverable 2: Compile, Train, and Evaluate the Model
Deliverable 3: Optimize the Model
Deliverable 4: A Written Report on the Neural Network Model (README.md)

# Deliverable 1: Preprocessing Data for a Neural Network Model
For deliverable 1 we need to complete the following steps and after completing all these steps we got the required table that is attached below

* Read in the charity_data.csv to a Pandas DataFrame, and be sure to identify the following in your dataset:
* What variable(s) are considered the target(s) for your model?
* What variable(s) are considered the feature(s) for your model?
* Drop the EIN and NAME columns.

![image](https://user-images.githubusercontent.com/112978144/228295563-7827a30f-a02f-4439-b745-2048c1401b0d.png)

* Determine the number of unique values for each column.
![image](https://user-images.githubusercontent.com/112978144/228295759-72d59725-f369-4f86-b54a-3f924639e406.png)
![image](https://user-images.githubusercontent.com/112978144/228296086-4814285b-d4b2-4155-80b0-41365e971173.png)

* For those columns that have more than 10 unique values, determine the number of data points for each unique value.
* Create a density plot to determine the distribution of the column values.
![image](https://user-images.githubusercontent.com/112978144/228296507-8f012b3a-e702-41ce-b9b1-89af856d142a.png)

* Use the density plot to create a cutoff point to bin "rare" categorical variables together in a new column, Other, and then check if the binning was successful.
![image](https://user-images.githubusercontent.com/112978144/228297380-f6f22fe0-d7b6-425e-8be6-b7adcf6ae233.png)

* Generate a list of categorical variables.
# Generate our categorical variable lists
application_cat = ["APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "INCOME_AMT", 
                  "SPECIAL_CONSIDERATIONS", "ASK_AMT"]
* Encode categorical variables using one-hot encoding, and place the variables in a new DataFrame.
*Merge the one-hot encoding DataFrame with the original DataFrame, and drop the originals. After completing all these steps we got following output
![image](https://user-images.githubusercontent.com/112978144/228297943-f306a580-2622-4dfb-9de7-356ce6c3e9f7.png)

# Deliverable 2: Compile, Train, and Evaluate the Model
For deliverable 2 we need to follow the instructions below and use the information file to complete Deliverable 2.

* Continue using the AlphabetSoupCharity.ipynb file where you’ve already performed the preprocessing steps from Deliverable 1.
* Create a neural network model by assigning the number of input features and nodes for each layer using Tensorflow Keras.
* Create the first hidden layer and choose an appropriate activation function.
* If necessary, add a second hidden layer with an appropriate activation function.
* Create an output layer with an appropriate activation function.
* Check the structure of the model.
![image](https://user-images.githubusercontent.com/112978144/228301076-03977463-a404-4d0e-a125-ef2ab08430ec.png)

* Compile and train the model.
* Create a callback that saves the model's weights every 5 epochs.
* Evaluate the model using the test data to determine the loss and accuracy.
![image](https://user-images.githubusercontent.com/112978144/228301492-c04eb2f1-326f-4b86-8aa0-89352412d2a7.png)
![image](https://user-images.githubusercontent.com/112978144/228301932-6b63ef07-f912-4e8b-beee-cc76f50760f9.png)

* Save and export your results to an HDF5 file, and name it AlphabetSoupCharity.h5.

# Deliverable 3: Optimize the Model
For deliverable 3 we need to follow these steps
* Create a new Jupyter Notebook file and name it AlphabetSoupCharity_Optimization.ipynb.
* Import your dependencies, and read in the charity_data.csv to a Pandas DataFrame.
* Preprocess the dataset like you did in Deliverable 1, taking into account any modifications to optimize the model.
* Design a neural network model, taking into account any modifications that will optimize the model to achieve higher than 75% accuracy.
![image](https://user-images.githubusercontent.com/112978144/228309440-d8976aaa-8665-4c1b-88c2-5b401124064f.png)

* Create a callback that saves the model's weights every 5 epochs.
![image](https://user-images.githubusercontent.com/112978144/228308953-c71f4289-1233-4816-a8f1-343290aa2e11.png)

* Save and export your results to an HDF5 file, and name it AlphabetSoupCharity_Optimization.h5.










![image](https://user-images.githubusercontent.com/112978144/228301802-1686e79c-0c04-49a4-b64a-7bc08532f974.png)

