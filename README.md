# deep-learning-challenge
Module 21 Challenge

# Report 

## Overview 
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, you have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as:

EIN and NAME—Identification columns
APPLICATION_TYPE—Alphabet Soup application type
AFFILIATION—Affiliated sector of industry
CLASSIFICATION—Government organization classification
USE_CASE—Use case for funding
ORGANIZATION—Organization type
STATUS—Active status
INCOME_AMT—Income classification
SPECIAL_CONSIDERATIONS—Special considerations for application
ASK_AMT—Funding amount requested
IS_SUCCESSFUL—Was the money used effectively

## Results 
### Data Processing 
 “*”Target Variable: "IS_SUCCESSFUL" 
<img width="827" alt="Screenshot 2023-10-04 at 9 33 11 PM" src="https://github.com/alexxisrangel/deep-learning-challenge/assets/129305054/843d4ad5-ab84-4f0e-a2bb-a395de349db5">

 
 “*”Feature Variable: 'STATUS','APPLICATION_TYPE','AFFILIATION',"CLASSIFICATION", "USE_CASE","INCOME_AMT","ORGANIZATION", "SPECIAL_CONSIDERATIONS"
 <img width="1105" alt="Screenshot 2023-10-04 at 9 32 43 PM" src="https://github.com/alexxisrangel/deep-learning-challenge/assets/129305054/83f04192-9db8-4ad4-afad-d6f4a8249bbe">

 “*”Varibles neither target or features: 'EIN', 'NAME', 'ASK_AMT'
<img width="784" alt="Screenshot 2023-10-04 at 9 37 49 PM" src="https://github.com/alexxisrangel/deep-learning-challenge/assets/129305054/e1d8303f-b23f-44ea-b7d7-58c284aa8fcc">

### Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why?
  “*”For my model I had a total of 28 nuerons. 10 for the first hidden layer, 8 for the seccond hidden layer and 8 for the third hidden layer. I decided on this since it was the maximum amount of nuerons I could work with before I ran out of RAM. The more nuerons that I added the better my accuracy got. 
  “*”Unfortunately I was unable to reach the accuracy goal of 75. I believe if I had more computing power i'd be able to reach that goal. 
  “*”Steps taken to reach 75% accuracy: Initially I started by just adding another hidden layer but that only led to a longer run time with a similar accuracy score. Then I increased the nuerons for all three layers but again I got a similar result. Lastly I noticed that the AMT_ASK column had over 8000 unique values which I thought was only confusing the model. This column represented the amount asked by applicants which in my opinion doesn't really correlate to if a funding would be successful. After doing so I did get to 73% accuracy which meant that my theory had some truth behind it. 
  

## Summary 

Overall I got the model to a 73% accuracy. Although it was below target, I was able to improve the initial accuracy from my first attempt. One approach I can take is not encoding all columns and instead just leaving them as they are. 
