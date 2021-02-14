# Neural_Network_Charity_Analysis

## Overview
This analysis uses a neural network model to predict the potential success of organizations requesting funding from AlphabetSoup.

## Results

#### Data Preprocessing
  - Target: IS_SUCCESSFULL
  - Features: Application type, Affiliation, Classification, Use Case, Organization type, Special Considerations, Ask Amount
  - Removed Variables: Name and Identification number were removed as neither targets or features. Status and Income Amount were also removed to reduce noise and attempt to improve model accuracy.
  
![Orig_Application_df](https://github.com/hkoivisto/Neural_Network_Charity_Analysis/blob/main/Resources/Orig_Application_df.png)
  
#### Compiling, Training, and Evaluating the Model
  - Neurons: The input layer was initiated with 80 nuerons, approximately double the number of features. Each subsequent layer used half as many neurons as the previous layer.
  - Hidden layers: The model was intialized with 2 hidden layers, and a third hidden layer was added to attempt to optimize the model.
  - Activation Functions: The Relu activation function was selected because the model is not recieving any negative inputs. All numerical inputs are in positive dollars.
  
  ![Orig_model](https://github.com/hkoivisto/Neural_Network_Charity_Analysis/blob/main/Resources/Orig_model.png)
  
  - Target Performance: 75%
  - Success: The model was not able to acheive target performance. With 5 variations of potential optimization, the best performance acheived was 73%
  
  ![model_report](https://github.com/hkoivisto/Neural_Network_Charity_Analysis/blob/main/Resources/model_report.png)
  
  - Optimization attempts: In an attempt to improve model accuracy, additional features were removed, the number of neurons in the hidden layers were increased, additional hidden layers were added, and the activiation functions were changed to Sigmoid functions.
  
  ![model_op5](https://github.com/hkoivisto/Neural_Network_Charity_Analysis/blob/main/Resources/model_op5.png)
  
## Summary
The neural network model was determined to be 73% accurate in predicting the success or failure of organizations requesting funding from AlphabetSoup. To improve model performance, more understanding of the features would be recommended, such as determining the importance of features like Status and Income Amount.

A Random Forest Classifier would also be recommned to give the model creator greater visibility in the decision process.
  
  
