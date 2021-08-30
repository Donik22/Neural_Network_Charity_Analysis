# Neural_Network_Charity_Analysis
## Overview
In this project we will be helping non-profit organization determine elegibility for funding. Using Machine leaning and neural networks we'll be using the features in the data set to help create a binary classifier to help guide our customers decision.

## Results

### Data Preprocessing

- IS_SUCCESSFUL Column Is our target for this module
- All columns except IS_SUCCESSFUL was considered as features.
- Columns such as EIN and NAME Where neither target nor feature due to its having no relevant to our data.

### Compiling, Training, and Evaluating the Model

- In AlphabetSoupCharity file we used 2 hidden layers. In the first hidden layer we used 80 neurons and with the second hidden layer we used 30.

![Deliverable 2 ](https://github.com/Donik22/Neural_Network_Charity_Analysis/blob/main/Resources/Deliverable%202%20Module.PNG)

- We werent able to achieve our target model performance which is 75%. on our first attempt we got 54 %.

![deliv2 accur](https://github.com/Donik22/Neural_Network_Charity_Analysis/blob/main/Resources/Accuract%20delv2.PNG)
### Steps taken to increase module performance

To increase our performance we removed an extra features, Changed Activation Functions, Remove a hidden layer and increase number of epochs.

#### First attempt
Removed an extra column in addition to `EIN`, `NAME`, `SPECIAL_CONSIDERATION` was removed. Additional modification had to be done to get a better results.

#### Second Attempt 
We changed the activation function to tanh --> tanh --> tanh --> Sigmoid this resulted in an accuracy score of 73%.

![Moduleatt2](https://github.com/Donik22/Neural_Network_Charity_Analysis/blob/main/Resources/Deliverable%202%20Module%20attempt%202.PNG)

![Accuracy 2](https://github.com/Donik22/Neural_Network_Charity_Analysis/blob/main/Resources/Accuracy%20score%20attempt%202.PNG)

#### Third Attempt
We removed a hidden layer but this proved to be counter productive with an accuracy score of 73%.

![Module final](https://github.com/Donik22/Neural_Network_Charity_Analysis/blob/main/Resources/Deliverable%202%20Module%20attempt%203.PNG)
![accuracy final](https://github.com/Donik22/Neural_Network_Charity_Analysis/blob/main/Resources/Accuracy%20score%20attempt%203.PNG)



## Summary 

Our model didnt meet the Accuracy level of 75% but it came close with a final accuracy score of 73%. Intially we were at 54% and our final result is a big improvment from that. A good Model to use for this data is the Random Forest Classifier. Having the properties of being more accurate and faster performance. The Random Forest classifier Is also a good Module to prevent overfitting.
