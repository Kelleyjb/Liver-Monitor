# Liver Monitor
 Performs K-Cluster Analysis With Limited User Interface
 The code for this program will be broken into three sections: UI for import/selection, interl k-cluster creation/analysis, and a final UI to examine results.

***THIS PROGRAM ASSUMES THAT THE CSV VALUS HAVE BEEN NORMALIZED/SCALED PRIOR*** 
 
 *K-clusters rely heavily on Euclidean Distance*
 ## Initial UI
  The initial user interface (UI) will allow for the user to select their csv file, filter any unwanted columns from consideration, and select desired settings for the K-Cluster.
  It will be broken into two Stages "Import" and "Settings".
  The settings will include toggles for: 
  - Graph 
  - Table (Outliers) 
  - Table (Full)
  
 ## K - Cluster
  K clusters will be made from designated file and fields according to selected settings.
 
 ## Final UI
  This interface will be responsible for displaying K-cluster results as well as holding options for reloading/manipulation of data.
  
 ## Work-In-Progress Features
- Auto-Filtering/Identifying Columns of the Data
- Adjusting k-cluster to work with any # of fields
- Toggles
- Finall UI
- Normalize/Scaling
  _ Issue with using data from different sources so it needs to be normalized for comparision
  - If there are fields which are more important, they should be scaled appropriately. Hopefully there will be a feature to  adjust the scaling values for each field
- Strategy for Tackling Null Values
  _ There are many null values spread through the data and they need to be handled 
	 - Discard
		  _ Discard the entire record
	 - Replace
		  _ Replace the value with the most common value 
		  - Replace the value with an average of all the present values
    - Replace the value with a 'ideal' value, if one exists
