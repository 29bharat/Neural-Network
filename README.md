# Neural-Network
  
## Objective
  
Import, analyze, clean, and preprocess a “real-world” classification dataset.
  
Select, design, and train a binary classification model of your choosing.
  
Optimize model training and input data to achieve desired model performance.
  
## Resources
  
Dataset provided: charity_data.csv (https://github.com/29bharat/Neural-Network/blob/master/Resources/charity_data.csv)
  
### Data Preprocessing
  
The data from the csv file is read into charity_df dataframe and a bunch of proprocessing steps are applied. Preprocessing on the data is appllied where we drop the EIN and Name column as they do not qualify/impact the target. Application_type and Classification are bucketed using OneHotCoder. This is then merged with the original charity_df and then application as well as classification columns are dropped
  
![alt_text](https://github.com/29bharat/Neural-Network/blob/master/OneHotEncodere.PNG)
  
### Setting up the Deep Learning Model
  
The Deep Learning Neural model has two hidden layers. First layer has 80 neurons and second has 30 Below is the model summary.

![alt_text](https://github.com/29bharat/Neural-Network/blob/master/model%20summary.PNG)
  
  
### Training and testing the model - Accuracy
  
Accuracy score is 0.73 i.e 73% with 100 epochs
  
![alt_text](https://github.com/29bharat/Neural-Network/blob/master/Loss_Accuracy.PNG)
    
## Summary
  
### How many neurons and layers did you select for your neural network model? Why?
  
A good rule of thumb is to take 2 - 3 times the number of input features so here we have taken 80 neurons in the first hidden layer and 30 in the second layer.
  
### Were you able to achieve the target model performance? What steps did you take to try and increase model performance?
  
the number of epochs were increased to 200 and then to 400 but in both cases the target accuracy wasnt achieved. We can try to add a third hidden layer and see if that helps. but teh attempt on increasing the number of epochs did not help. the accuracy remained at about 73%.
  
### If you were to implement a different model to solve this classification problem, which would you choose? Why?
  
Random Forest will be a good model to apply since thsi is tabular data. It requires less preprocessing and training process is simpler and faster. 
  
  
## Link to the jupyter notebook file: https://github.com/29bharat/Neural-Network/blob/master/AlphabetSoupChallenge.ipynb

