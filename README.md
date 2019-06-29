# api
API for accessing neighborhood data
*NOTE* The API is in beta and probably has bugs. Data automatically restricted to last 90 days and limited to Duval County, FL.

## GETs

### Report
Get an incident/crime report for the last 90 days by community name or address.  
https://api.jatsby.com/report?query=wolf%20creek%20townhomes  
https://api.jatsby.com/report?query=3500%20nightscape%20circle  
Returns a community report if possible, and an address report if a community couldn't be matched to the query.  

### Search
Search for communities or addresses for which we have data. Results guaranteed to return a report via the Report endpoint.  
https://api.jatsby.com/search?query=wolf%20creek  
https://api.jatsby.com/search?query=3500%20nightscape%20circle  
Returns up to 10 community and address matches for the provided query.
