# capston-Sparkify-Project


<h3>Python libreries</h3>
his project uses the following software and Python libraries:


-Python

-Spark

-Pyspark

-pandas

-Matplotlib

-Seaborn


<h3>Files</h3>
-Sparkify.ipynb Notebook is main file of the project.

-It demonstrates the process of using pyspark to explore the data and build the model.


<h3>The project consists of three part :</h3>
<h4>*Part-1:
Load and Clean Dataset</h4>
the mini-dataset file is mini_sparkify_event_data.json. Load and clean the dataset, checking for invalid or missing data - for example, records without userids or sessionids.
<h4>*Part-2:
Exploratory Data Analysis</h4>
perform EDA by loading a small subset of the data and doing basic manipulations within Spark. In this workspace, you are already provided a small subset of data you can explore.
<br><b>Define Churn</b?
Once you've done some preliminary analysis, create a column Churn to use as the label for your model. I suggest using the Cancellation Confirmation events to define your churn, which happen for both paid and free users. As a bonus task, you can also look into the Downgrade events.
<br><b>Explore Data</b>
Once you've defined churn, perform some exploratory data analysis to observe the behavior for users who stayed vs users who churned. You can start by exploring aggregates on these two groups of users, observing how much of a specific action they experienced per a certain time unit or number of songs played.

<h4>*Part-3:
Observations:</h4>
<br>This gives us already a good indicator for the churn definition: we could define churned users as those users who have visited the ‘Cancelation Confirmation’ page. Further, we could take the ‘Submit Downgrade’ column into account.
<br>
<h4>*Part-4
Feature Engineering</h4><br>

For now we will derive feature which we think mostly good predicter of target ie. churn and will use those feature to test/train our model

<h4>*Part-5:
Modeling</h4><br>
Preparing data and to push to the model Lets use VectorAssembler which is transformer that combines a given list of columns into a single vector column
Here we will going to implement logistic regression and RandomForest classifer and see how these model perform. Since the churned users are a fairly small subset, we using F1 score as the metric to optimize.


<h3>Conclusion</h3>
<br>
A model is implemented to predict coustemer churn. Cleaned the rows with no userId and converted gender into binary form. For the model 10 featuers were built. Three predicting algorithm were tried which is logistic regression, Random Forest and GBTClassifier in which GBTClassifier is selcted as final model as its resultis better than other models. VectorAssembler is used to prepare and push the data to the model, which combines a given list of columns into a singel vector column. F1 score is used as the metric optimize.
