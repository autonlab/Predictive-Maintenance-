This dataset is a collection of line currents and voltages for different fault conditions.

As the electrical powers system is getting in size, then also its complexity in such sectors as generetation, transmission, distribution and load systems changes.
Because of the faults that might occur, there can be detected some severe economic losses together with reduction of the reliability of the electrical system.
One of the most crucial parts in the power system is the transmission line, which role is to transmit electric power from the source area to the distribution network. 
The faults on electrical power system transmission lines are supposed to be first detected and classified correctly and should be cleared in the least possible time. 


The power system which was modeled for this simulate fault analysis consist of 4 generators. Then there is simulated the circuit under normal conditions as well as under various fault conditions. After it, the sensors values are collected and the measured Line Voltages and Line Currents at the output side of the power system is saved.

In the dataset folder we are provided with 2 datasets.
The first one, called classData, contains the data which further would be used to classify the types of fault. We are given here with Inputs and outputs data.
The inputs data consist of such columns with sensor recordings as: Ia,Ib,Ic (Each of these sensors present line current for the particular phase: A, B or C) and Va,Vb,Vc (Each of these sensors present line voltage for the particular phase: A, B or C
The Outputs data consist of the following columns which represent part of the fault line: G, C, B, A. Fot this output data we can receive 1 if failure occurred, else 0 occurs.
Example of reading this data:
For the Outputs [G C B A] if we have:
[0 0 0 0] - means that there is no fault
[1 0 0 1] - means that there is LG (Line to Ground) fault (between phase A and Ground)
[0 0 1 1] - means that there is LL (Line to Line) fault (between phases A and B)
[1 0 1 1] - means that there is LLG (Line to Line to Ground) fault (between phases A, G and Ground)
[0 1 1 1] - means that there is LLL (Line to Line to Line) fault (between all 3 phases)
[1 1 1 1] - means that there is LLLG (Line to Line to Line to Ground) fault (3 phases symmetrical fault)

Second dataset called detect_dataset is the file that contains the data to give the possibility to detect faults in a power system.
We are given here with the same inputs as in the classData which is [Ia,Ib,Ic,Va,Vb,Vc] and also we have here the outputs which gives us information about the failure occurence: the 0 value is shown when there is no fault and 1 when the fault occurred.

