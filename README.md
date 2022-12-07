# Project Title: Venture Funding with Deep Learning

# Background:

You work as a risk management associate at Alphabet Soup, a venture capital firm. Alphabet Soup’s business team receives many funding applications from startups every day. This team has asked you to help them create a model that predicts whether applicants will be successful if funded by Alphabet Soup.

The business team has given you a CSV file containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. The CSV file contains a variety of information about each business, including whether or not it ultimately became successful. With your knowledge of machine learning and neural networks, you decide to use the features in the provided dataset to create a binary classifier model that will predict whether an applicant will become a successful business.

# What You're Creating:

To predict whether Alphabet Soup funding applicants will be successful, you will create a binary classification model using a deep neural network.

This challenge consists of three technical deliverables. You will do the following:

Preprocess data for a neural network model.

Use the model-fit-predict pattern to compile and evaluate a binary classification model.

Optimize the model.

## Prepare the Data for Use on a Neural Network Model
Using your knowledge of Pandas and scikit-learn’s StandardScaler(), preprocess the dataset so that you can use it to compile and evaluate the neural network model later.

Complete the following data preparation steps:

1. Read the applicants_data.csv file into a Pandas DataFrame. Review the DataFrame, looking for categorical variables that will need to be encoded, as well as columns that could eventually define your features and target variables.

2. Drop the “EIN” (Employer Identification Number) and “NAME” columns from the DataFrame, because they are not relevant to the binary classification model.

3. Encode the dataset’s categorical variables using OneHotEncoder, and then place the encoded variables into a new DataFrame.

4. Add the original DataFrame’s numerical variables to the DataFrame containing the encoded variables.

5. Using the preprocessed data, create the features (X) and target (y) datasets. The target dataset should be defined by the preprocessed DataFrame column “IS_SUCCESSFUL”. The remaining columns should define the features dataset.

6. Split the features and target sets into training and testing datasets.

7. Use scikit-learn's StandardScaler to scale the features data.

## Compile and Evaluate a Binary Classification Model Using a Neural Network
Use your knowledge of TensorFlow to design a binary classification deep neural network model. This model should use the dataset’s features to predict whether an Alphabet Soup–funded startup will be successful based on the features in the dataset. Consider the number of inputs before determining the number of layers that your model will contain or the number of neurons on each layer. Then, compile and fit your model. Finally, evaluate your binary classification model to calculate the model’s loss and accuracy.

To do so, complete the following steps:

1. Create a deep neural network by assigning the number of input features, the number of layers, and the number of neurons on each layer using Tensorflow’s Keras.

2. Compile and fit the model using the binary_crossentropy loss function, the adam optimizer, and the accuracy evaluation metric.

3. Evaluate the model using the test data to determine the model’s loss and accuracy.

4. Save and export your model to an HDF5 file, and name the file AlphabetSoup.h5.

## Optimize the Neural Network Model
Using your knowledge of TensorFlow and Keras, optimize your model to improve the model's accuracy. Even if you do not successfully achieve a better accuracy, you'll need to demonstrate at least two attempts to optimize the model. You can include these attempts in your existing notebook. Or, you can make copies of the starter notebook in the same folder, rename them, and code each model optimization in a new notebook.

To do so, complete the following steps:

1. Define at least two new deep neural network models (resulting in the original model, plus two optimization attempts). With each, try to improve on your first model’s predictive accuracy.

2. After finishing your models, display the accuracy scores achieved by each model, and compare the results.

3. Save each of your models as an HDF5 file.


Dataset:
---
applicants_data.csv


## Results
* Original Model Results (/Resources/AlphabetSoup.h5):
    * Accuracy Score: 72.59%
    * Loss Score: 77.21%
    
* Alternative Model 1 Results (/Resources/AlphabetSoup_A1.h5):
    * Accuracy Score: 70.64%
    * Loss Score: 181.03% 

* Alternative Model 2 Results (/Resources/AlphabetSoup_A2.h5):
    * Accuracy Score: 73.18%
    * Loss Score: 55.26% 

---

## Technologies: Python 3, Jupyter Notebook
---
Python 3 or later.

Jupyter Notebook for IDE.

---

## Usage:
---

Ensure the proper libraries and dependencies have been imported.

![image](https://user-images.githubusercontent.com/34729547/206214943-3e3607ef-d5b9-42f5-a04e-fa4b40ee51a7.png)


---

## Contributors: Nia Robinson

LinkedIn: https://www.linkedin.com/in/niaelanrobinson/

---

## License

MIT License.
