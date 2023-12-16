
 
  Title: ETL and Analysis of Airline Baggage Complaints

A.  Dataset Details:
	 No of rows:252
	 No of columns:8
	 File Size:13KB
	 File format:CSV
	 Column definitions:
	    Airline: Name of Airline
	    Date: The date used to report data for each of the airlines   
	    Month: The month used to report data for each of the airlines   
	    Year: The year used to report data for each of the airlines   
	    Baggage:The total number of passenger complaints for theft of baggage contents, or for lost, damaged, or misrouted luggage for the airline that month
	    Scheduled:The total number of flights scheduled by the airline that month
	    Cancelled:The total number of flights cancelled by the airline that month
	    Enplaned:The total number of passengers who boarded a plane with the airline that month

B.  Business requirments:
    Client (user) needs answers to the following questions  (using visuals) to aid their decision-making:
	-Total baggages (with passenger complaints for theft, loss, damage, or misrout) over the whole period
	-Total baggages (with passenger complaints for theft, loss, damage, or misrout) by year
	-Total baggages (with passenger complaints for theft, loss, damage, or misrout) by airline name
	-Total flight scheduled over the whole period
	-Total flight scheduled by year
	-Total flight scheduled by airline name
	-Total cancelled flights over the whole period
	-Total cancelled flights by year
	-Total cancelled flights by airline name
	-Total enplaned over the whole period
	-Total enplaned by year
	-Total enplaned by airline name
	-Percentage total cancelled flights to total flights scheduled
	-Ratio of uncancelled flights to baggages 

C.  Solution Steps: 
   	 -create ETL pipeline that copies data from On-premise SQL Server to Azure Data Lake in parquet file format
   	 -extract data from data lake into Databricks cluster for cleaning and transformation
   	 -clean and tranform the data in Databricks
   	 -load the cleaned and tranformed data back into the file storage system (Data Lake) from Databricks
   	 -perform data modeling (normalizing the source dataset table and setting relationships for the fact and dimension tables) using Power BI Desktop
	 -perform data analysis using Power BI Desktop
	 -report the analysis result via visuals using Power BI Desktop

D.  Tech tools: 
   	 -On-premise SQL Server (as On-premise data store)
   	 -Azure Data Factory (to copy data from On-prem SQL Server to Azure Data Lake using self-hosted integration runtime)
   	 -Microsoft Azure Data Lake service (as cloud-based data source and final store for the analytics solution)
   	 -Databricks (for data cleaning and transformation)
   	 -Microsoft Power BI Desktop (for data analysis and reporting)
  