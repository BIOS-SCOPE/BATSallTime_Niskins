# BATSallTime_Niskins
Niskin bottles from BATS cruises, back to the beginning of the BATS program\
updated 3 April 2025; Krista Longnecker

# Short answer
The CSV file (`BATSallTime_Niskins.csv`) is a comma-separated file with all the Niskin bottles back to the beginning of the BATS program.

## Details
The BATS data are available at https://bios.asu.edu/bats/bats-data (as of 3 April 2025). The file with all the bottle information is : `bats_bottle.txt`. I downloaded the file and then parse it into something that can more easily be handled in R/MATLAB/Python (using BATS_Niskins_KLv1.Rmd). 

### Some notes on time
All times are GMT, so if you want to know the local time you need to convert these while considering daylight savings time. There are a few columns with time information in the output file 
* yyyymmdd --> four digit year - two digit month - two digit day
* time --> this is 24 hour time with any *preceeding* zeros dropped. Hence, a time listed as 45 is actually 0045 (45 minutes after midnight). 
