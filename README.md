# Project describtion
Data analysis of users behavior on "Data analysis in R" course on stepic.org platform.

We have two csv files at start  and we want to predict whether a user will graduate the course or not based on the same information but only about first two days after he enrolled. 

We will assume that user has graduated the course if he get at list 40 points.

# Data describtions
## [events_train.csv](https://stepik.org/media/attachments/course/4852/event_data_train.zip)
It contains data about acts users perform

* step_id - numeric step id
* user_id - numeric anonymous user id
* timestamp - unixdate time of an event occurence
* action - event type:  
  * discovered
  * viewed
  * started_attempt - it used to be that user had to press the button "start attempt" to have an ability to submit a solution for practical step
  * passed - successfuly solved practical step 

## [submissions_train.csv](https://stepik.org/media/attachments/course/4852/submissions_data_train.zip)
It contains data about times and statuses of user's submissions

* step_id - numeric step id
* user_id - numeric anonymous user id
* timestamp - unixdate time of an event occurence
* submission_status - sumission status
  * correct
  * wrong

# Files
* events_train.csv
* submissions_train.csv
* stepic_users.ipynb - notebook with solution
* sumissions_test.csv - test data that contains information about only first 2 days of activity for each user
* events_test.csv
* result.csv - predictions for the test dataset
