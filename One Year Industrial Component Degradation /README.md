# ONE YEAR INDUSTRIAL COMPONENT DEGRADATION DATASET DESCRIPTION


The dataset consist of the machine data taken from the degrading component recorded from the sensors located on the component over the period of 12 months.

In total, the dataset consist of 519 files, each of them is saved in the following format:
MM-DDTHHMMSSNUMmodeX.csv
The MM applies to a month (from 1 to 12 month but not the calendar but the months when the data recordings has been taken).
DD applies to a day of the month
T starts the Time section, where HH(Hour) MM(minute) SS(Second) applies to the start time of a day of the recording.
NUM means the sample number
ModeX applies to a mode (which varies from 1 to 8, depending on the mode).
Each of the files Is more or less  seconds sample with a time resolution of 4ms which in total gives 204 time-samples for every file.
In this dataset you are given with  different modes and different speeds values that the machine might be operated in.

The purpose of this dataset is to enable an option to present the component degradation process over the course of the year. Based on such analysis you would be able to check if the component has been replaced at the some point or not, you might check if the wear can be accurately predicted and also you might make a prediction of the RUL (that stand for Remaining Useful Life) in order to determinate the maintenance windows (what is the part of predictive maintenance).

