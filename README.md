# Risk-Factor-Identification-for-Dangerous-Commercial-Truck-Drivers

This project uses Big Data Hadoop Ecosystems for truck fleet data to refine and analyse trucking movement in order to meet the organizational goal of better understanding risk. 
The use case involves geographic data, vehicles, average mileage, gas consumption, events, risk factors, and other supporting information. 
Each truck has been equipped to with devices to log location and event data.


# Dataset
Project contains 3 CSV files:
1. Geolocation.csv
2. Trucks.csv
3. Trucks_mg.csv


# Risk thresholds
The thresholds for risk mitigation are determined by the requirements of the governing bodies for 
our industry combined with reasonable business needs and observed telematics data.
The following is a partial list of the current risk factors:
• Miles driven
• Speed
• Individual State highway law compliance
• Number of trailerstowed
• Freight weight (tonnage)
• Driverlogs
• Off hours, as per section 395.3 of the FMCSA regulations
• Drug test results as per section 382 of the FMCSA regulations
• Driving record per section 391.27 of the FMSCA regulations (e.g. DUIs, tickets, reported accidents)
• Recorded telematics sensor violations, e.g. unsafe following, speeding, lane departure.
• Road closures, rerouting
• Vehicle maintenance and inspection
• Driver qualifications persection 391 of the FMCSA regulations


# Steps
1. Loading data into Hadoop Distributed File System (HDFS).

2. Create a Hive Table for geolocation and load data from Geolocation file.
   Use the DDL document provided to create all tables.
   
3. Load the imported file into HIVE by utilizing “LOAD DATA INPATH”.

4. Integrating HDFS with Tableau via JDBC drivers for Impala and Hive.
   Download Impala ODBC Driver, URL: https://www.cloudera.com/downloads.html
   
5. Use RServe package in RStudio to connect with Tableau, and perform Multiple Regression.


# Output
Dashboard or report chart that shows the Riskfactor per driver and be able to highlight those who have exceeded the threshold 7.0


# Business Value
Accidents caused by large trucks remain one of the leading causes of injuries and deaths in the 
United States. The objective is identifying dangerous commercialtruck drivers nationwide.



   
                                  
                                  
