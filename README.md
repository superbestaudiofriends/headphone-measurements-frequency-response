# headphone-measurements

8/1/2020: I will be providing only SBAF compensated measurements for now using the MiniDSP EARS. One step at a time.


## File Naming Conventions

The file naming conventions will be as follows:<br><br>
<em>Coupler|CompensationVersion|Channel|-|Manufacturer|Headphone|.txt</em><br>

Here are some examples:<br><br>
EAR31L-DanClarkAudio-EtherFlow.txt<br>
EAR31R-Sennheiser-HD650.txt            
FPC02R-Grado-SR225.txt         

## File Format

The file will have two columns, frequency Response and amplitude, separated by a tab character. There will be no headers. The columns will look like this:<br>

20.00   -43.43<br>
30.00   -42.32<br>
50.00   -21.33<br>


## Notes about SBAF compensation using a MiniDSP EARS

This compensation is an attempt to have a straight line across as perceptive neutral. Read about it here:
https://www.superbestaudiofriends.org/index.php?threads/minidsp-ears-deriving-sbaf-compensations-from-minidsp-files.7067/
The SBAF curve should be not confused with the Harmon curve from Olive and Welti. The Harmon curve is a consumer preference target.

Here is a spreadsheet for anyone with a MiniDSP EARS to calibrate it to the SBAF compensation. 
Note that all EARS units are slightly different. The spreadsheet contains a delta from my unit's provided HEQ.
In theory, applying this delta to your HEQ files should end with the same results here.
https://docs.google.com/spreadsheets/d/1uUqkpD3EJMzpl8FeJbNOkjApvMKAIL3IP8Y1At_ldng/edit#gid=0

The 3.1 version with the removal of the screws is currently used as of 8/1/2020



