# ROBOT EXECUTION FAILURES - DATASET DESCRIPTION:

These datasets were collected , define and evaluated in order to improve the classification accuracy.
The dataset folder consist of force and torque measurements on a robot after failure detection.


We are given with 5 different datasets, whereas each of them defines a different learning problem.

* LP1 --> failures in approach to grasp position
* LP2 --> failures in transfer of a part
* LP3 --> position of part after a transfer failure
* LP4 --> failures in approach to ungrasp position
* LP5 --> failures in motion with part

Each of the datasets consist of different number of instances:
For LP1 this is 88
For LP2 this is 47
For LP3 this is 47
For LP4 this is 117
For LP5 this is 164

Here are 90 features in each of the 5 datasets. Each of these features represents a torque or a force measured after failure detection.
Each failure is characterized by 15 force/torque samples collected at regular intervals starting immediately after the failure is detected.
Każdy z przykładów w danej bazie danych definiowany jest w następujący sposób:

Column 1 is the name of the class which is(in brackets are given percentages of instances per class in each dataset): 
- For LP1: normal(24%), collision(19%), obstruction(39%), fr_collision(18%);
- For LP2: normal(43%), back_col(15%), front_col(13%), right_col(11%), left_col(19%);
- For LP3: ok(43%), moved(32%), slightly_moved(19%), lost(6%);
- For LP4: normal(21%), collision(62%), obstruction(18%);
- For LP5: normal(27%), collision_in_tool(16%), collision_in_part(29%), bottom_obstruction(13%), bottom_collision.

Columns from 2 to 7 represents the following features:
Fx1	Fy1	Fz1	Tx1	Ty1	Tz1
Fx2	Fy2	Fz2	Tx2	Ty2	Tz2
....
Fx15	Fy15	Fz15	Tx15	Ty15	Tz15

* Fx, Fy and Fz from 1 to 15 is the evolution of force Fx Fy and Fz respectively
* Tx, Ty and Tz from 1 to 15 is the evolution of the torques Tx, Ty and Tz respectively.


 
