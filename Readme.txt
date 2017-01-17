Metadata information

FILE: FHA_FinalData_Acute.csv
GENERAL CONTENTS: This file tracks hospital inpatient (aka acute) activity. It shows the patient inflow, outflow, occupancy, and time in system for each day over a two year period.
FIELDS:
	ProgramGroup - One of the four main acute care types: Emergency (admitted patients), Maternity, Medicine, Surgery

	DateID - the date number of the record. 

	DayOfWeek - the day of the week of the record. Sunday is 1 and Saturday 7

	Admissions - the number of admissions on that particular date into that specific acute care type

	Discharges - the number of discharges on that particular date from that specific acute care type

	
	AverageLengthOfStay - the average number of days stayed in acute for patients discharged on that specific date by acute care type. A patient may have received more than one care type during their acute stay. They are categorized under the care type they had on discharge.
	
	AverageOccupancy - the average number of patients receiving that particular acute care type on that particular date. Note that if patients switched care types on a particular day, they would be counted in both care types on that date. 


FILE: FHA_FinalData_ER.csv
GENERAL CONTENTS: This file tracks hospital Emergency (aka outpatient) activity. It shows the number of patient visits to ER for each day over a two year period.
FIELDS:
	DateID - the date number of the record. 
	
	CTAS Group - the Canadian Triage and Acuity Score (CTAS) group. The scale goes from 1 to 5 in order of decreasing acuity. CTAS 1 and 2 are grouped together; CTAS 3 is not grouped; CTAS 4 and 5  are grouped together. 
	
	ER Visits - the number of patients visiting the ER on a particular date for a particular CTAS grouping. These patients may or may not be admitted into acute care. See the FHA_FinalData_Acute.csv file for patients admitted via ER on any particular date.  



GENERAL NOTES:

-Date ID numbers in the two files correspond to the same historical date.
-These files contain two years of historical data. 