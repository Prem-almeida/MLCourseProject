How to run

Just run the mrmr_win32.exe on cmd by passing parameters mentioned below

Usage: 

mrmr -i <dataset> -t <threshold> [optional arguments]
	 
-i <dataset>    .CSV file containing M rows and N columns, row - sample, column - variable/attribute.

-t <threshold> a float number of the discretization threshold; non-specifying this parameter means no discretizaton (i.e. data is already integer); 0 to make binarization.

-n <number of features>   a natural number, default is 50.

-m <selection method>    either "MID" or "MIQ" (Capital case), default is MID.

-s <MAX number of samples>   a natural number, default is 1000. Note that if you don't have or don't need big memory, set this value small, as this program will use this value to pre-allocate memory in data file reading.

-v <MAX number of variables/attibutes in data>   a natural number, default is 10000. Note that if you don't have or don't need big memory, set this value small, as this program will use this value to pre-allocate memory in data file reading.

example: mrmr_win32.exe -i gene.csv -t 0 -n 400 -m MIQ -s 2000 -v 20000

note: data must be a csv file with samples as rows and features as columns

