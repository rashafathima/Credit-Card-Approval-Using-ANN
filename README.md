# Credit Card Approval Using ANN
<br>

## Background

For many years banks used credit scoring techniques to determine which loan applicants they should lend money to. They do this by considering the applicants credit score. Credit score in simple words can be defined as the score that represents the credit worthiness of individual; better the credit score of the applicant, greater is the chance of his/her loan application to get accepted. 
<br> The decision whether the applicant is eligible for loan can be calculated by considering various instances/variables of an individual such as the monthly installment rate, credit card score(fico), purpose of loan , debt to income ratio, the number of times the borrower has been late etc.
<br> <br> 

## Case Study

The purpose of this research is to examine how well neural networks can work in providing accurate and reliable results for credit card approval. Using NN for credit scoring is actually utilizing a model or a method for evaluating the variables in order to kmow the credit worthiness of the applicant. Through this research we are trying to find to what level of accuracy NN can be used as a tool for credit card approvals in banks. 


## Data

### Note : The dataset concerns credit card applications. All attribute names and values have been changed to meaningless symbols to protect confidentiality of the data.

### Software Used

Name : Matlab (Gave greater emphasis on the nntool in matlab) <br>

### Datasets 

Name : Australian Credit Card Approval <br>
Resource : <a href = "http://archive.ics.uci.edu/ml/datasets/statlog+(australian+credit+approval)">http://archive.ics.uci.edu/ml/datasets/statlog+(australian+credit+approval)</a><br>

### Instances 

Total : 690

### Attributes 

Total :  15 <br> 
Input :  14 (8 categorical and 6 numerical: A1 - A14) <br>
Target : 1 Class Attribute (A15) <br><br><br>
A1: CATEGORICAL <br>
A2: continuous <br>
A3: continuous <br>
A4: CATEGORICAL <br>
A5: CATEGORICAL <br>
A6: CATEGORICAL <br>
A7: continuous.<br>
A8: CATEGORICAL <br>
A9: CATEGORICAL <br>
A10: continuous.<br>
A11: CATEGORICAL <br>
A12: CATEGORICAL <br>
A13: continuous.<br>
A14: continuous.<br>
A15: class attribute <br>
<br>

## Missing Cases 

There were a total of 37 missing cases in the datasets(5% of 690). The missing cases were replaced by the mean of the column if the column had continuous data type in the dataset and mode of the column if the column had categorical datasets.

## Model Used

The application has been implemented using artificial neural networks. <br>
A total of 10 experiments was conducted ; with 3 experiments conducted using three hidden layers and the rest 7 experiments using two hidden layers. 
<br>

<strong> Experiment Conducted using 3 Hidden Layers</strong><br>
Training Algorithm : trainlm
<br>
Transfer Function : Logsig-tansig-tansig-purelin(1 hidden layer-2nd hidden layer-3 hidden layer- output layer)<br>
Accuracy :  Ranged between 67.05% and 83.72% <br>
Performance Function : Mean Squared Error<br>

<strong> Experiment Conducted using 2 Hidden Layers</strong><br>
Training Algorithm : trainlm(5 experiments) and traingd(2 experiments)
<br>
Transfer Function : Logsig-tansig-purelin(1 hidden layer-2nd hidden layer- output layer)<br>
Accuracy :  Ranged between 76.02% and 84.16% <br>
Performance Function : Mean Squared Error<br>

<strong>OVERALL BEST ACCURACY: 84.16%</strong>


## Observations

From the experiment conducted the overall accuracy level ranged from 67.05% to 84.16%, with the highest accuracy (84.16%) being attained at epoch 4 of total epochs 75; when the model was trained with two hidden layers. 

