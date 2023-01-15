# Hyperparameter-Tuning-GridSearch-Randomized-GridSearch
Performed Hyperparameter Tuning with Grid Search and Randomized Grid Search<break/>
Model was to predict whether a loan would end up being paid off or sent to collections<break/>
I used sklearn's ColumnTransformer() for imputing missing values for columns with missing values.<break/>
Target variable was broken into 3 categories PAIDOFF, COLLECTIONS, and COLLECTIONS_PAIDOFF<break/>
For simplicity in fitting the model, I used mapping to group COLLECTIONS_PAIDOFF with COLLECTIONS to make <break/>
The target variable binary.  As a result, the model didnt perform extremely well with just 71% accuracy<break/>
Next, I am going to re-run the model without engineering the target and also will use sklearn's pipeline with <break/> 
ColumnTransformer to see if the model's peformance improves.
