The project is about turbofan engine degradation process.
There is collected dataset from engine degradation simulation experiments conducted at NASA using C-MAPSS.
We can distuinguish 4 different sets further divided into training and test subsets. Each time series from the sets is from a different engine. Each od the engines starts working in normal conditions (no fault condition noticed). 
Important note: the engines have different degrees of initial wear and manufacturing variation.
There are also 3 operational settings with a substantial effect on engine performance.
The data is contaminated with sensor noise.
The engines operate normally in the beginning but develop a fault over some time.
In the training set, the engines are run to failure, while in the test sets the end comes sometime before failure.
The main goal is to predict RUL (Remaining Useful Life) of each engine.
Each of the columns contained in the data provides the following information (starting from the left column):
1: Engine unit number
2: Time (in cycles)
3-5: Three operational settings
6-26: Sensor readings