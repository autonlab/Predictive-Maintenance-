# DATASET DESCRIPTION

Below you can find a description for sensor that were chosen for the analysis purpose and which may have an impact on components failure:



Each of the three databases represents sensor data collected during flight tasks on the MIG-29 aircraft during a single flight. 
Each database consists of 5 sensor groups (there are vibration data, engine data, pilot data, pressure data and ARM, which stands for Autonomus Steering Machine).


The description of the groups is as follows:

Vibration data group - this is a group consisting of 12 sensors, and among them we distinguish:

- vibration level - the sensors included here are:
	- KSA vibration (Blocks of Airplane Units) vibration [mm/s], left BPK (Block of Limit Commands) and KSA vibration [mm/s], right BPK vibration of the aircraft carrier system;
	- Left and right engine vibrations


- Compressor stall - indicating steady/unsteady operation of the left and right engines (presence of vibrations on the engine blades)

- Overheat - sensor indicating possible overheating of the left or right engine 

- Reserve_L and Reserve_R - sensors indicating the status of the right and left engine reserve system

- Zmn_Obr_L and Zmn_Obr_P - sensors indicating reduced RPM of the left or right engine



Engine data group - consists of 17 sensors:

- DSS_L and DSS_R - indications expressed in degrees, relating to the engine control lever (revolutions) 

- Hb - a sensor giving values read from the barometric altimeter

- Nk_L and Nk_P - (WWC Rotation) are indications expressed in percentages giving the values of high-pressure rotor rotation for the left and right engines

- T4_L and T4_P - indications giving the values of the temperature behind the turbine for the left and right engines, expressed in degrees Celsius.

- U_27 - sensor reading DC voltage indications expressed in Volts.

- Vp - instrument speed indications

- Dopal_L and Dopal_P - indicators giving the values of direct injection of fuel after the turbine to increase the exhaust gas pressure 

- Kg_550 - sensor giving the value of emergency residual fuel

- Flaps_Prz and Flaps_Zas - indicators giving information about the swing of the front flaps and zaskrzydcrh flaps 

- DSS_MAX_L AND DSS_MAX_P - maximum indications, expressed in degrees, concerning the engine control lever (revolutions) 

- Landing gear - indicator giving information whether the landing gear is retracted or not.



Pilot data grape - consists of 19 sensors:

- Alpha - indicator giving information about the angle of attack, expressed in degrees

- Gamma - indicator giving information about the roll of the aircraft, expressed in degrees

- Hb - sensor giving values read from the barometric altimeter

- Vp - indications of instrument speed, expressed in knots

- Ma - indications of the current value of the achieved Mach speed of the aircraft

- Nk_L and Nk_P - (WWC Rotation) are indications given in percentage giving the values of high pressure rotor rotations for the left and right engines

- Nx - indications giving information about the longitudinal overload of the aircraft

- Ny - indications informing about transverse overload of the aircraft

- Nz - indications indicating the vertical overload of the aircraft

- Dopal_L and Dopal_P - indicators indicating the values of direct fuel injection behind the turbine to increase the exhaust gas pressure 

- Kg_550 - sensor giving the value of emergency residual fuel

- Flaps_Prz and Flaps_Zas - indicators giving information about the swing of the front flaps and the wing flaps 

- PB - indicator giving information about the activation of the combat button

- Undercarriage - indicator giving information whether the undercarriage is retracted or not

- Sh_Drop / Sh_Drop - indicator giving information whether the parachute has been released / dropped


Pressure data grape - consists of 17 sensors:

- Nk_L and Nk_P - (WWC Rotation) these are indications in percent giving the high pressure rotor rotation values for the left and right engines

- PmKSA_L and PmKSA_P - indicators giving the value of the pressure of the oil present in the oil system of the right or left engine of the aircraft (before feeding into the engine)

- Pm_L and Pm_P - these are indicators reporting the value of oil pressure located in the right or left engine

- Bpk_L and Bpk_P - indicators giving information about a possible break in the circuit of the left or right engine transmitters

- Hydr_Gł - indicator giving information about a possible malfunction of the aircraft's main hydraulic system

- Hydr_wzm - indicator giving information about a possible malfunction of the aircraft's booster hydraulic system

- Kg_550 - indicator giving the value of emergency residual fuel

- Pumpage_L and Pumpage_P - are otherwise Compressor stall. These sensors indicate the steady/unsteady operation of the left and right engines (the presence of vibrations on the engine blades)

- Reserve_L and Reserve_R - sensors indicating the status of the right and left engine reserve system

- Zmn_Obr_L and Zmn_Obr_P -sensors indicating the reduced speed of the left or right engine



ARM (Autonomus Steering Machine) data group, includes 9 sensors:

- Alpha - indicator giving information about the angle of attack, expressed in degrees
	
- ARM_APUS - an indicator giving the ARM-APUS displacement value in millimeters

- ARM_N - indicator giving in millimeters the displacement value of ARM-N

- ARM_T - indicator giving the ARM-T displacement value in millimeters

- Hb - sensor giving the values read from the barometric altimeter

- Vp - instrument speed indications, expressed in knots

- Flaps_Prz and Flaps_Zas - indicators giving information on the pivot of the front and wing flaps 

- Undercarriage - indicator giving information whether the undercarriage is retracted or not.
