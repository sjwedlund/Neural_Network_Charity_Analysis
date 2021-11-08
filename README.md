# Neural Network Charity Analysis

## Overview
The purpose of this analysis is to use machine learning and neural networks to use the features in a  dataset containing 34,000 organizations funded by Alphabet Soup, to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. 

## Results
### Data Preprocessing
- The column IS_SUCCESSFUL is the variable that is considered the target for the model. 
- The columns APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT are considered to be the features for the model. 
- The columns EIN, and NAME are variables that were removed from the input data, because they are neither targets or features and are not necessary. 

### Compiling, Training, and Evaluating the Model
- I used two hidden layers in my neural network model, one with 80 neurons and the other had 30 neurons. I used two different activation functions: relu and sigmoid. Relu was used in the first and second hidden layer, and sigmoid was used for the output layer because it is a binary classification. 
- I did not acheive target model performance of 75% accuracy. The accuracy was 61.71%
- I made three attemps to try to increase model performance.
  - In the first attempt, I added more neurons to the hidden layer, with 100 neurons on the first layer, and 30 neurons on the second layer. The accuracy improved to 72.58%.  
  - In the second attempt, I added a third hidden nodes layer. I went back down to 80 neurons in layer 1, kept 30 neurons in layer 2, and added 10 neurons to layer 3. After having run the notebook a couple of times, the accuracy went down to only 41.9%.
  - In the third attempt, I changed the number of neurons in the second hidden layer to 35 but kept the other layers the same, and the accuracy stayed at 41.9%. 
  
## Summary
The most successful attempt with the highest accuracy was when I used 100 neurons in the first hidden layer and 30 neurons in the second hidden layer. It wasn't quite 75%, but it was pretty close at 72.5%. I suggest trying the Random Forest Classifier because of its ranking of Feature Importance Classification. Some of the variables might be more important than others when determining whether an organization will be successful. 
