# credit-risk-classification
Module 20 challenge assignment

The purpose of this analysis is to use several criteria to determine whether a potential loan is likely "healthy" or "high-risk." A healthy loan is one where the lender can be reasonably secure in their lending. The party being lent to is reputable and will likely not default on their loan. A high-risk loan is the opposite, there is a reasonable chance that the party being lent to will default on this loan due to their history, financial status, and several other factors.

The criteria being considered are as follows: Loan size, interest rate,	borrower income, debt-to-income ratio, number of accounts, derogatory marks, and the borrower's total debt. These factors basically represent four things: the borrower's financial status, the borrower's past history, the borrowing amount of the loan, and the current financial market (interest rate). All of these criteria serve to inform a machine learning model about the loan status, basically whether it will likely be a healthy loan or a high-risk loan.

The data was split into training and testing, which was then fed into a logistic regression model. This model is binary in the sense that it is used to predict whether a particular data point is more likely to belong in one class or another. In this case, whether a loan is healthy or high-risk. After the training is complete, the model outputs a series of values to indicate how well it performed. 

The following is the list of some of the values that the model outputs: 

    - Precision score -- This value represents the ratio of of correctly predicted outcomes 
        to the total number of predicted outcomes (it does this for each class).

    - Recall score -- This value is more about the model's ability to recognize any
        particular data point as a certain class. It's the ratio of correctly predicted
        outcomes to the total number of data points that were actually in that class.

    - Accuracy -- Lastly, this value is an average of both classes (healthy vs high-risk
        loans) and how well the model did over all. It is the ratio of correctly predicted data points to the number of data points. It's essentially a general metric for the correctness of the model. 

The model performed very well. For healthy loans, it had a 100% precision score, meaning that for each loan the model predicted as healthy, it was correct. It had a 99% recall score for the same class, meaning that for all the loans the model saw that were in fact healthy, it recognized 99% of them as such. 

Conversely, for the high-risk loan class, the model performed well, but slightly worse. It had a 84% precision score, and a 94% recall score. While these values are lower, the overall accuracy of the model is still good enough that it can be used in a financial setting. However, in my opinion, it is more important to correctly predict the high-risk loans, since those are the ones that could cost a financial institution money. Because of that, it would be good to continue to train/test the model on independent sets of data to improve the values from the initial training/testing period. 

