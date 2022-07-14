

The whole BackBlaze dataset is available to download from BackBlaze.com website, available under the following link: https://www.backblaze.com/b2/hard-drive-test-data.html

I will be adding systematically new datasets to the repository.

For providing the example dataset taken from the BackBlaze website, the Prediction HDD Failure folder is given with the dataset that comes from 2013 and contains the following columns:

* Date - this is the information about the date when the file was created.
* Serial Number - This is the column that provides us with the information about the manufacturer-assigned serial number of the drive
* Model - This is the column that provides us with the information about the manufacturer-assigned model number of the drive
* Capacity - This column is about the drive capacity given in bytes
* Failure - that column contains the information about the possible failure of the drive. If it is "0", then it means that the drive does not have any failures, but if it contains "1", it means that it was the last day the drive was operational before failure occurred.
* Based on the year from which the dataset come from, the amount of the columns with data is as follows:
    - from 2013 to 2014 -  we are given with 80 columns of data, where we can distinguish the Raw and Normalized records are taken for 40 different SMART stats (as was reported by the given drive). Each value presents the number reported by the drive 
    - from 2015 to 2017 - we are given with 90 columns of data, where we can distinguish the Raw and Normalized records taken for 45 different SMART stats (as was reported by the given drive). Each value presents the number reported by the drive 
    - 2018 (Q1) -  we are given with 100 columns of data, where we can distinguish the Raw and Normalized records taken for 50 different SMART stats (as was reported by the given drive). Each value presents the number reported by the drive 
    - 2018 (Q2) -  we are given with 104 columns of data, where we can distinguish the Raw and Normalized records taken for 52 different SMART stats (as was reported by the given drive). Each value presents the number reported by the drive 
    - 2018 (Q4) -  we are given with 124 columns of data, where we can distinguish the Raw and Normalized records taken for 62 different SMART stats (as was reported by the given drive). Each value presents the number reported by the drive 