# LI-ION BATTEY AGING --> DATASET DESCRIPTION:

The dataset originally is from NASA Ames Prognostics Center of Excellence. 
The dataset can be used in order to develop the prognostic algorithms. In particular, due to the differences in depth-of-discharge (DOD), the duration of rest periods and intrinsic variability, no two cells have the same state-of-life (SOL) at the same cycle index. The aim is to be able to manage this uncertainty, which is representative of actual usage, and make reliable predictions of Remaining Useful Life (RUL) in both the End-of-Discharge (EOD) and End-of-Life (EOL) contexts.
The Remaining useful life is the length of time a machine is likely to operate before it requires repair or replacement. By taking RUL into account, engineers can schedule maintenance, optimize operating efficiency, and avoid unplanned downtime. For this reason, estimating RUL is a top priority in predictive maintenance programs

In order to simulate the dynamic operation conditions in real applications, 18 650 LiCoO2 batteries were cycled under a series of random currents rather than the constant discharge currents. In the Datasets folder you can find data from 4 batteries: B0005, B0006,B0007 and B0018. These datasets has been downloaded from the GitHub repository of which the creator is VaibhavBhujade (the link to the repository is added to the Sources file which is located in the Documentation folder).
Each of the batteries were cycled under a series of random currents and each loading period lasted for 5 mins.
Charging and discharging test was performed after every 1500 periods in order to measure the battery capacity. The failure threshold for 4 of the batteries are considered as the capacities at the end of the test and the capacities are plotted against the test time (days).

For each of 4 battery datasets, the number of charge, discharge and impedance cycles is 616.
The dataset contained in the Documentation folder is already divided into the testing set and training set (each of them contains data of 4 batteries ) and Input n Capacity dataset files.


The data consist of the following structure:
- cycle --> this is the top level structure array which contains 3 types of operations: charge, discharge and impedance operations.
- type --> it provides an information about the type which can be charge, discharge or impedance
- ambient_temperature --> this is the column that gives an information about the ambient temperature (which for this data is considered to be as 24 Celsius degrees).
- time --> this is the column about the date and time of the start of the cycle (in MATLAB date vector format)
- data --> data structure which contains the measurements



Parameters for charge cycles are as follow:
- voltage
- current
- temperature
- current charge
- voltage charge
- time


Parameters for charge cycles are as follow:
- voltage
- current
- temperature
- current load
- voltage load
- capacity
- time

Parameters for impedance cycle are as follow:
- Voltage_measured
- Current_measured
- Temperature_measured
- Current_charge
- Voltage_charge
- Time
- Capacity

For charge operation we are given with the following fields:
* Voltage_measured --> Battery terminal voltage (Volts)
* Current_measured --> Battery output current (Amps)
* Temperature_measured --> Battery temperature (degree C)
* Current_charge --> Current measured at charger (Amps)
* Voltage_charge --> Voltage measured at charger (Volts)
* Time --> Time vector for the cycle (secs)

For discharge operation we are given with the following fields:

* Voltage_measured: Battery terminal voltage (Volts)
* Current_measured: Battery output current (Amps)
* Temperature_measured: Battery temperature (degree C)
* Current_charge: Current measured at load (Amps)
* Voltage_charge: Voltage measured at load (Volts)
* Time: Time vector for the cycle (secs)
* Capacity: Battery capacity (Ahr) for discharge till 2.7V

For impedance operation we are given with the following fields:
* Sense_current: Current in sense branch (Amps)
* Battery_current: Current in battery branch (Amps)
* Current_ratio: Ratio of the above currents
* Battery_impedance: Battery impedance (Ohms) computed from raw data
* Rectified_impedance: Calibrated and smoothed battery impedance (Ohms)
* Re: Estimated electrolyte resistance (Ohms)
