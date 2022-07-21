# DIESEL ENGINE FAULTS - DATASET DESCRIPTION:

The main purpose for this dataset is the fault diagnosis in Diesel engines in order to assist the predictive maintenance, through the analysis of the variation of the pressure curves inside the cylinders and the torsional vibration response of the crankshaft.

A fault simulation model based on a thermodynamic model was developed, from which certain feature vectors were selected, which were first obtained from processing signals such as pressure and temperature inside the cylinder and torsional vibration of the engine flywheel. These vectors were then used as a form of input data for machine learning which aimed to discriminate several operating states of the machine:
- normal (without faults) --> 250 scenarios;
- lowering of intake manifold pressure --> 250 scenarios;
- compression ratio in the cylinders --> 1500 scenarios;
- Reduction of the amount of fuel injected into the cylinders --> 1500 scenarios.

Łącznie cała baza danych liczy 3500 różnych scenariuszy awarii dla 4 opisanych powyżej stanów eksploatacyjnych.
Ze względu na najniższy wspólny poziom błędu w oszacowaniu średnich i maksymalnych ciśnień cyklu spalania, pomiędzy danymi eksperymentalnymi a danymi symulowanymi, na etapie walidacji modeli termodynamicznych i dynamicznych, częstotliwość obrotów silnika ustawiona została na 2500 RPM dla wszystkich scenariuszy.

