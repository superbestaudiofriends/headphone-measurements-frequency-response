# HPDB (Headphone Database) Background 

This repository is an effort to eventually make all https://superbestaudiofriends.org and http://www.Changstar.com headphone measurements data available to the general public. I am hoping there will be volunteers to make code available to compare and contrast the measurements.

This repository can be accessed as the easier to remember http://HPDB.io

## headphone-measurements

8/1/2020: I will be providing only SBAF compensated measurements for now using the MiniDSP EARS. One step at a time.


## File Naming Conventions

The file naming conventions will be as follows:<br><br>
<em>raw/comp|Coupler|CompensationVersion|-|Manufacturer|Headphone|<pad>|<sample>|Channel.txt</em><br>

Here are some examples:<br><br>
cEAR32-DanClarkAudio-EtherFlow-L.txt<br>
cEAR32-Sennheiser-HD650-R.txt            
cFPC02-Grado-SR225-L.txt    
cEAR32-ZMF-VeriteOpen-Univ-2-L.txt


## Measurement Systems

cEAR32 MiniDSP EARS with screws removed (better seal) with compensation 3.2<br>
cEAR30 MiniDSP EARS with screws intact (stock) with compensation 3.02<br>
cFPC21 Flat Plate Coupler (no pinna with foam and felt overlay)<br>

Note all all compensations for each system are made somewhat comparable to each other. There may be differences because of seal, inconsistencies in placement, etc.


## File Format

All frequency response data will be 1/6 octave smoothed. The file will have two columns, frequency Response and amplitude in db, separated by a space or tab character. There will be no headers. The columns will look like this:<br>

20.00   -43.43<br>
30.00   -42.32<br>
50.00   -21.33<br>
75.00   -23.23

Note that all data is normalized to the region between 500 to 1500Hz with the lower frequencies weighted more.

## Notes about SBAF compensation using a MiniDSP EARS and other stuff

This compensation is an attempt to have a straight line across as perceptive neutral. Read about it here:
https://www.superbestaudiofriends.org/index.php?threads/minidsp-ears-deriving-sbaf-compensations-from-minidsp-files.7067/
The SBAF curve should be not confused with the Harmon curve from Olive and Welti. The Harmon curve is a consumer preference target.

Here is a spreadsheet for anyone with a MiniDSP EARS to calibrate it to the SBAF compensation. 
Note that all EARS units are slightly different. The spreadsheet contains a delta from my unit's provided HEQ.
In theory, applying this delta to your HEQ files should end with the same results here.
https://docs.google.com/spreadsheets/d/1uUqkpD3EJMzpl8FeJbNOkjApvMKAIL3IP8Y1At_ldng/edit#gid=0

The 3.2 version with the removal of the screws is currently used as of 8/1/2020

As of August 20, 2020, I will begin to add the flat plate coupler measurements. These will be compensated as much
as possible to be comparable with the EARs. Note that there will be some slight differences as the flat plate
rig does have not an ear, e.g. pinna, concha, etc.

These will have filenames that start with cFPC21*


## Viewing datasets

Use this tool from Bill Pham to visualize the data: http://billp.site/projects/chart-tool/
Download the files first. Be sure to apply +90db offset or so because the datasets are normalized to 0db.
Enter 90 in the offset field and press the "+Offset"


## Use of these datasets

This work is licensed under"Creative Commons - Attribution 4.0 International
https://creativecommons.org/licenses/by/4.0/legalcode

