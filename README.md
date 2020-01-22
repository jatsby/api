*the API will be down for a couple of days (early September) for a db schema change...hang tight!*

# api
API for accessing crime data at the "neighborhood" and "community" (subdivision) levels.
*NOTE* The API is in beta and probably has bugs. Data automatically restricted to last 90 days and limited to Duval County, FL.

## GETs

### Report
Get an incident/crime report for the last 90 days by community name or address.  
https://api.jatsby.com/report?query=arlington%20shores  
https://api.jatsby.com/report?query=1230%20underhill%20dr  
Returns a community report if possible, and an address report if a community couldn't be matched to the query.  

### Search (GET)
Search for communities or addresses for which we have data. Results are guaranteed to return a report via the Report endpoint.  
https://api.jatsby.com/search?query=wolf%20creek  
https://api.jatsby.com/search?query=3500%20nightscape%20cir  
Returns up to 10 community and 10 neighborhood matches for the provided query.

## Reports
Reports use data directly from the Jacksonville Sheriff's Office (JSO) to provide detailed information at the *neighborhood* level- something never done before. 

Each report uses the incidents specific to that neighborhood or community to provide useful information not available anywhere else.

We provide specific details about _violent_ incidents- those that involve weapons or bodily injury. Patterns help identify bad neighbors by highlighting repeat incidents at the same address.

## Web App
There is a web app at https://jatsby.com!
