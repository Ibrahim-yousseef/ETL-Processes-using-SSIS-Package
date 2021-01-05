# ETL-Processes-using-SSIS-Package  
ETL Processes for ITI DB Server

```
First package designed to transfer Student data from [ITI DB] to [Test DB] with the following Criteria:  
a-	If table Student Exists in [Test DB] delete all data. Use[Execute SQL Task Component]  
b-	Merge the first name and last name to be one field [Full name].use[Derived Column Component]  
c-	Make a ful backup for [Test DB]  
d-	On error  display message box “error occurred”  
```

---
```
second package designed to Split Course data from [ITI DB] into 3 files with the following criteria:  
a-	Select Course data with topic name From ITI DB  
b-	Sort Course data by Crs_name Descending. use [Sort Component]  
c-	Crs_name should appear in lower case. Use [Character Map Component]   
d-	Split Course data into 3 files:  
i.	File1.txt contains Course data with Course Duration<30 hours.  
ii.	File2.txt contains Course data with Course Duration=30 hours.  
iii.	File3.txt contains Course data with Course Duration>30 hours.  
Note: set columns name as first row in the files  
```
