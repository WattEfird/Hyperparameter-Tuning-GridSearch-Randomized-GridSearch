# Hyperparameter-Tuning-GridSearch-Randomized-GridSearch
The dataset used was for customers who either paid off or defaulted on their loan <br>
Target variable was broken into 3 categories PAIDOFF, COLLECTIONS, and COLLECTIONS_PAIDOFF<br>
I merged the loans that were COLLECTIONS_PAIDOFF into COLLECTIONS, since they did enter collections at some point<br>
I had to convert some features to datetime and then further engineered them into new numerical columns in the dataset<br>
I broke out and separated due_date, paid_off_date and effective date into columns for day of week, month and hour<br>
Model was to predict whether a loan would end up being paid off or sent to collections<br>
I used sklearn's Simple Imputer for imputing missing values--imputing by the median instead of the mean as the median would be a better representation,since<br>
the data was skewed.  
Next, I then fit the imputer on train data and then transformed the train data<br>
I transformed the validation and test data using the imputer train data.  Finally, I used Random Forest to build the model.<br>
For hyperparameter tuning I used GridSearchCV first, which took awhile to run (38 minutes approximately).  Last I used Randomized Grid Search.  <br>
The model scored an accuracy of approximately 97% after hyperparameter tuning using Grid Search and also scored an accuracy of 97% after using Randomized Grid Search.  

