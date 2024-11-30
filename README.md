# deep-learning-challenge

## Overview of the Analysis

A predictive model was developed to assess the probability of success for funding applications from a charity. This model incorporates various organizational details such as affiliation, governmental industry classification, organization type, and income, alongside specifics about the proposal including the use case, amount requested, and special considerations. The dataset used for training and testing also included the final outcome for each application. To prepare the data for analysis, categorical variables were transformed into boolean columns, and the dataset was scaled using the StandardScaler technique before being split into training and testing subsets. The training data was fed into a Neural Network featuring three/four hidden layers with a Rectified Linear Unit activation function. Following training, the accuracy of the model was assessed using the testing data. Despite attempts to optimize the model, none of the adjustments met the desired threshold for effectiveness.          

## Results

* Initial Model:
  * Parameters:
    * 2 hidden layers
	* 40 and 20 nodes per respective hidden layer, 100 epochs
	* Rectified linear unit activation used on all hidden layers
  		* Accuracy: 73.7%

* Optimization 1:
  * Parameters:
   * 3 hidden layers
	* 100, 50, 25 nodes per respective hidden layer, 100 epochs
	* Rectified linear unit activation used on all hidden layers
  		* Accuracy: 73.9%

* Optimization 2:
  * Parameters:
    * 4 hidden layers, but instead of 100 epochs, 50 epochs
	* 100, 75, 50, and 25 nodes respectively
	* Rectified linear unit activation used on all hidden layers
  		* Accuracy: 73.8%

* Optimization 3:
  * Parameters:
    * 4 hidden layers, but back to 100 epochs
	* 64, 32, 16, and 8 nodes respectfully
	* Rectified linear unit activation used on all hidden layers
  		* Accuracy: 73.60%

The model is designed to predict the success or failure of a project, with various features serving as inputs including affiliation, governmental industry classification, organization type, income, use case, amount requested, and special considerations. To streamline the model, irrelevant factors such as Name and EIN were excluded. Initially, I opted for three layers in the model to expand upon the original design, but also experimented with four layers to assess the potential optimization with a larger dataset. Despite adjustments made to the number of layers, neurons, and epochs, the desired model performance target of 75% accuracy remained elusive.


## Summary

Despite numerous attempts to optimize parameters, including those documented here and within the code, such as adjusting the number of epochs and incorporating additional input variables like amount, none proved effective in achieving the 75% accuracy threshold. Alongside these efforts, other optimization strategies were explored. However, given the dataset's limitations, I am convinced that attaining 75% accuracy is unfeasible. Therefore, I believe pursuing a different model type would not have yielded superior results.