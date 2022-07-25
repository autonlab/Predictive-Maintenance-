# MACHINE PMx CLASSIFICATION - DATASET DESCRIPTION:

This dataset contains synthetic data that has been created for the real Predictive Maintenance purposes in the industry field.

The purpose of this dataset is to predict machine failure and type.

We are given in the dataset with 10000 data points stored as rows with 14 attributes.
We can distinguish 10 different columns which provide the following information:
1) UID: unique identifier ranging from 1 to 10000;
2) ProductID: consisting of a letter L, M, or H for low (50% of all products), medium (30%), and high (20%) as product quality variants and a variant-specific serial number;
3) Type - which gives the information about the type of a product. It can M, L or other;
4) Air temperature [K]: generated using a random walk process later normalized to a standard deviation of 2 K around 300 K;
5) Process temperature [K]: generated using a random walk process normalized to a standard deviation of 1 K, added to the air temperature plus 10 K;
6) Rotational speed [rpm]: calculated from powepower of 2860 W, overlaid with a normally distributed noise;
7) Torque [Nm]: torque values are normally distributed around 40 Nm with an Ïƒ = 10 Nm and no negative values;
8) Tool wear [min]: The quality variants H/M/L add 5/3/2 minutes of tool wear to the used tool in the process;
8) Machine failure - indicates, whether the machine has failed in this particular data point for any of the following failure modes are true. 0 if no failure and 1 if failure occurred;
8) Failure Type - the last 5 columns provide an information about type of the failure. We can distinguish the following failure modes:
* Tool wear failure (TWF): the tool will be replaced of fail at a randomly selected tool wear time between 200 â€“ 240 mins (120 times in our dataset). At this point in time, the tool is replaced 69 times, and fails 51 times (randomly assigned). 
* Heat dissipation failure (HDF): heat dissipation causes a process failure, if the difference between air and process temperature is below 8.6 K and the rotational speed is below 1380 rpm. This is the case for 115 data points. 
* Power failure (PWF): the product of torque and rotational speed (in rad/s) equals the power required for the process. If this power is below 3500 W or above 9000 W, the process fails, which is the case 95 times in our dataset. 
* Overstrain failure (OSF): if the product of tool wear and torque exceeds 11,000 minNm for the L product variant (12,000 M, 13,000 H), the process fails due to overstrain. This is true for 98 datapoints. 
* Random failures (RNF): each process has a chance of 0,1 % to fail regardless of its process parameters. This is the case for only 5 datapoints, less than could be expected for 10,000 datapoints in our dataset. 

If any of the above failure modes is detected, the process fails and a value of 1 appears next to the "machine failure" label.




