# DESCRIPTION FOR DATASET ABOUT: "CONDITION BASED MAINTENANCE OF NAVAL PROPULSION PLANTS"


The dataset consist of data records taken from a sophisticated simulator of Gas Turbines (mounted on a Frigate characterized by a Combined Diesel Electric and Gas propulsion plant).

For the purpose of this simulator, blocks have been carefully developed that together form the structure of the simulator, these blocks include the propeller, hull, gas turbine, gearbox and controller. In addition, it is also possible to take into account the situation where there is a decrease in performance over time of the components that make up the gas turbine structure (such as the turbine and the compressor).

The parameters describing the propulsion system are as follows:
- Vessel speed (linear function of lever position lp).
- Compressor degradation factor kMc.
- The degradation coefficient of the turbine kMt.
Having information about these 3 parameters, it is possible by their combination to make a description of the degradation state.

In order to discretize the compressor degradation state, the compressor degradation coefficient was studied in the [1; 0.95] domain, while the turbine degradation coefficient was studied in the [1; 0.975] domain.

The ship's speed was tested by sampling real speed from 3 knots (kt) to 27 kt with a granularity of representation equal to tree knots.

The dataset file saved in txt format consist of 18 column (16 column that contain Gas Turbine measures (features) that indirectly represents the state pf the system subject to the performance decay and 2 columns which represent the coefficient state).


The columns are as follow:
- Lever position (lp) [ ]
- Ship speed (v) [knots]
- Gas Turbine (GT) shaft torque (GTT) [kN m]
- GT rate of revolutions (GTn) [rpm]
- Gas Generator rate of revolutions (GGn) [rpm]
- Starboard Propeller Torque (Ts) [kN]
- Port Propeller Torque (Tp) [kN]
- Hight Pressure (HP) Turbine exit temperature (T48) [C]
- GT Compressor inlet air temperature (T1) [C]
- GT Compressor outlet air temperature (T2) [C]
- HP Turbine exit pressure (P48) [bar]
- GT Compressor inlet air pressure (P1) [bar]
- GT Compressor outlet air pressure (P2) [bar]
- GT exhaust gas pressure (Pexh) [bar]
- Turbine Injecton Control (TIC) [%]
- Fuel flow (mf) [kg/s]
- GT Compressor decay state coefficient
- GT Turbine decay state coefficient







