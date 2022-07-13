The dataset added to this folder in the repository originally comes from Signals, Multimedia, and Telecommunications Laboratory and is available under the following link: http://www02.smt.ufrj.br/~offshore/mfs/page_01.html



DATASET DESCRIPTION:


We are given in this dataset with 1951 time-series data from different sensors taken by using a SpectraQuest's Machinery Fault Simulator Alignment-Balance-Vibration.
We can distinguish in this dataset 6 different states:
 	- normal function;
	- imbalance fault;
	- horizontal misalignment faults;
	- vertical misalignment faults;
	- inner bearings faults;
	- outer bearing faults.

Each of the datasets consist of  columns for each sensor, and the columns are as follow:
	COLUMN 1 --> tachometer signal in order to estimate rotation frequency,
	COLUMNS 2-4 --> underhang bearing accelerometer (axial, radial tangential direction),
	COLUMNS 5-7 --> overhang bearing accelerometer (axial, radial tangential direction),
	COLUMN  --> consist of the microphone sensor readings.


States description:

	1) Normal function - we have here 49 sequences without any fault. Each of the sequences is with a fixed rotation speed that ranges between 737 RPM and 3686 RPM with the steps of approximately 60 RPM.

	2) Imbalance Fault - this state of the dataset is simulated with load values within the Ange from 6 g to 35 g. For the load values that are below 30 g, the rotation frequency was assumed in the same values in which it is adopted for the normal state sequence. For load equal or above 30 g., the resulting vibration makes it impracticable for the system to achieve the rotation with a frequencies above 3300 RPM, thus limiting the number of distinct rotation frequencies.

	3) Horizontal Parallel Misalignment - this is the state which present a type of a fault that was induced into the Machinery Fault Simulator by shifting horizontally of 0.5mm, 1mm, 1.5mm and 2mm. By using the same range for the rotation frequency as in the case of the normal operation for each horizontal shift, depending on the misalignment, the measurements are as follow: for 0.5mm it is 50, for 1mm, 1.5mm and 2 it is 49 what in total gives 197 measurements.

	4) Vertical Parallel Misalignment - this is the state which present a type of a fault that was induced into the Machinery Fault Simulator by shifting vertically of 0.51mm, 0.63mm, 1.27mm, 1.40mm, 1.7mm and 1.90mm. By using the same range for the rotation frequency as in the case of the normal operation for each vertical shift, depending on the misalignment, the measurements are as follow: for 0.51mm it is 51 and for 0.63mm, 1mm, 1.27mm, 1.40mm, 1.7mm, 1.90mm 2 it is 50 what in total gives 301 measurements.

	5) inner and outer bearing faults - the rolling bearings find to be the most susceptible elements to fault occurence. By Alignment-Balance-Vibration manufacturer, we are provided with 3 defective bearing. Each of it is with a distinct defective element (outer track, rolling elements, and inner track) and placed one at a time in 2 different positions in the Machinery Fault Simulator experimental stand:
	* Underhang position: between the rotor and the motor
	* Overhang position: this is the external position having the rotor between the bearing and the motor. This type of a faults is practically imperceptible when there is no imbalance. So to solve it, 3 masses of 6 g, 20 g, and 35 g were added to induce a detectable effect, with different rotation frequencies as before.
		
 