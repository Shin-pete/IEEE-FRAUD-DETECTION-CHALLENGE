# IEEE-FRAUD-DETECTION-CHALLENGE
![Fraud_img](https://www.finance-monthly.com/Finance-Monthly/wp-content/uploads/2018/07/Fraud-Epidemic-Costs-£3.2-Trillion-Globally-750x430.jpg)

## Notebook

[Here's my Notebook](https://nbviewer.jupyter.org/github/Shin-pete/IEEE-FRAUD-DETECTION-CHALLENGE/blob/master/Final_Notebook.ipynb)

Problem: 

Fraud costs businesses and consumers millions of dollars a year. One potential solution is to create a system that can predict transactions that appear to be fraudulent. However this comes with a few problems of it's own: Most transactions aren't fraudulent, and yet treating them as such will cost companies billions. We need to devise a system that captures as much of the possible fraudulent transactions as we can without also flagging legitimate transactions as that would get in the way of commerce itself. So, we need to develop a model that minimizes false positives as well as false negatives as they both have negative effects for our target audience. 

Methodology: 

We first begin by gathering up our data [here](https://www.kaggle.com/c/ieee-fraud-detection/data)

Upon examination we learned many interesting things like the fact that .mail and .gmail when used as primary and secondary email addresses together, represented a large percentage of fraudulent transactions. We learned similar things about android devices. Some of the data is anonymized and doesn't offer up much in the way of information at face value, however going back and visualizing it might prove to be a useful intervention. 


We then attempted a variety of modeling techniques, the one in the notebook is a LIGHT-GBM model and our hyperparameters were tuned by gridsearch already. 


Results: 

The model has an AUC-ROC score of .9073. We successfully predicting very large percentage of the fraudulent activity without compromising performance on non fraud cases too much. 

![Celebration_gif](https://acegif.com/wp-content/uploads/funny-celebrate-40.gif)


Conclusion: 

While some good work has been done on this model, it can be further improved by doing further analysis on the anonymized features as well as gaining a deeper understanding of fraudulent transactions in the first place. 
