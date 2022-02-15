# Procedure 
We will have a  3 step process  Data Pre-Processing, Model Building and Model Evaluation
We will use IMDB dataset to build bag of word model
First, we will import the training dataset
We will explore the data analysis 
Then we will use some cleanse data methodology 
After that, we will build a linear Support Vector classic model
Finally, we  are going to make performance metrics to determine accuracy, recall, precision, and f-1 score. 
# Data Pre-Processing 	
We are going to get our datasets from kaggle. 
https://www.kaggle.com/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews
This is a dataset for binary sentiment classification containing substantially more data than previous benchmark datasets. They provide a set of 25,000 highly polar movie reviews for training, and 25,000 for testing!
# Cleaning data
![image](https://user-images.githubusercontent.com/99052999/153985326-cbd3969e-bfa9-4146-9a84-b039ccdcfab5.png)
![image](https://user-images.githubusercontent.com/99052999/153985333-aeeeeaa2-925b-47f7-9ea6-88701a58f67d.png)

# Before
![image](https://user-images.githubusercontent.com/99052999/153985392-5a7f7d3d-8c99-48bc-a84f-a917afa80e4e.png)
# After
![image](https://user-images.githubusercontent.com/99052999/153985400-d12fb171-9a55-477f-b2b2-2c3e783139c9.png)
# Model Building 
We used Linear Support Vector Classifier to classify our data
The objective of a Linear SVC (Support Vector Classifier) is to fit to the data you provide, returning a "best fit" hyperplane that divides, or categorizes, your data. From there, after getting the hyperplane, you can then feed some features to your classifier to see what the "predicted" 
![image](https://user-images.githubusercontent.com/99052999/153985248-09792c6d-cc8c-4735-a400-6d34a581f035.png)
# Mode evaluation
![image](https://user-images.githubusercontent.com/99052999/153985453-c6975bc6-2d04-401e-bf36-5de7fd0b806d.png)
 Code: from sklearn.model_selection import train_test_split
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.33, random_state=42)
Since we used 33% of data for prediction and based on confusion matrix:
We concluded that:
---The classifier made a total of 16863 predictions ( 16863 comments )
---There are two possible predicted classes: "positive" "Negative"
---Out of those 16863 comments, the classifer predicted "positive" 8347 times, and "negative" 8516 times
--- In reality, 8181 comments are positive, and 8182 comments are negative. 
# Suggestions/insights 
***We believe this model will help them save money, time to determine which comment is positive or negative. 
***Since IMDB has paid membership for professionals, this model will help them increase the membership because professionals will save more time to figure out how many sentiment is positive or negative. 
***This model will improve their AI system, help them to grow their business advertising, will expand  more products and services. 




