## tCSVString

+ Version 1.0

Converts all the rows and their columns to a single csv formated string. The csv string is not in the output row. Use the component property CSV_TEXT to retrieve the value. 

---

### Overiew of job flow

![Alt text](/doc/job_overview.png?raw=true "Job - Flow Diagram")

### Retrieving the CSV string

1. Provide rows of data with columns as part of the flow (e.g.: database query)
+NOTE: The tCSVString component will pass through the rows of data so you can insert it in the middle of your flow.
2. Retrieve the CSV string after the flow has compelted by calling tCSVString component's CSV_TEXT property. 

![Alt text](/doc/tFixedFlowInput_01.png?raw=true "tFixedFlowInput - retrieve csv string")

### Save the CSV string as a *.csv file

3. Pass the csv string to a tFileOutputRaw component

![Alt text](/doc/tFileOutputRaw_01.png?raw=true "tFileOutputRaw - create csv file")

### CSV file content

![Alt text](/doc/output_csv.png?raw=true "CSV File - content")
