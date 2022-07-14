In this folder you can find a dataset and useful documentation regarding the following topic:
# "Air pressure system failures in Scania trucks".


The files contained here are a part of APS (Air Pressure System) Failure and Operational Data for Scania Trucks. The APS system generates pressurized air which is further utilized in various functions in a truck, such as braking and gear changes.
The dataset consist of 2 files saved in csv format.
The training set contains 60000 examples in which 59000 belongs to the negative class and 1000 is positive class.
* The positive class consists of component failures for a specific component of the Air Pressure System.
* The negative class consists of different trucks with failures which occurred in different components which are not belonging to the Air Pressure System.

Whereas the test set file consists of 16000 examples with 171 different attributes per one record of which we have 7 histogram variables. Where the values are missing, such places are denoted by "NA".
The exact names of the attributes of the data have been anonymized due to the proprietary reasons.
We are given here with both the single numerical counters and the histograms that consist of bins together with different conditions.
Mostly the histograms that are there have open-ended conditions at each end. For instance, at the moment when we measure the ambient temperature "T" - the histogram would be defined with 4 bins together with the following attributes:
- class
- anonymized operational data

Each of the bins collects values for different temperature ranges:
- Bin 1 collects values for the temperature "T" < -20
- Bin 2 collects values for the temperature "T" >= -20 and "T" < 0
- Bin 3 collects values for the temperature "T" >= 0 and "T" < 20
- Bin 4 collects values for the temperature "T" > 20

When it comes to the operational data - it consist of an identifier and a bin ID (example: Identifier_Bin).

License link: https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html