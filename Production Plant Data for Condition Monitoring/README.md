# Production Plant Data for Condition Monitoring - DATASET DESCRIPTION

The dataset has been created in order to give the possibility to predict the condition of an important component within the production lines. This condition is essential for the function of the plant and the resulting product quality.

The dataset consist of 8 run-to-failure experiments (we can distinguish files: C8, C9, C7, C16, C15, C13, C14 and C11, whereas C7 and C13 are divided into 2 parts. The results in each of the files listed relate to a different experiment that consists of a running until failure process for the particular studied machine). In this data we are given with  previously properly selected features that are related to the component. The machine studied in all of the experiments is the same but not all the experiments have recorded the same signals.
Each of the files is divided into 2 types of the columns: the first one is the timestamp and the second is the sensor part. The second part consist of 25 signals (each file gives the signals records for a different component)

Fo the purpose of the conducted experiment, the following steps were taken with the data obtained:
* By using the leave-one-out method of selections (this method is a special case of cross-validation where the number of folds equals the number of instances in the data set), the training and prediction data were selected.
* Ultimately, it was decided to select data from the component under test for prediction.
* The training data for the "new" condition was created by selecting and combining a certain amount of data e all other components.
* Self-Organizing Map was trained on the learning data to present the "new" condition.
* Visualization and calculation of the degradation of the component under test was performed. 
* The same procedure was carried out for all experiments, in order to obtain degradation predictions for all tested components.

