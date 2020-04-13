#### Group - Get groups by groupName*, groupType, county
groupName* - The name of the group. Fuzzy search, so “Mandarin P” will return “Mandarin Pines”
groupType - the kind of group (“Block”, “Subdivision”, “Neighborhood”)
county - the county the group is in. Can be string (e.g. “Duval”) or the internal ID of the county (26)
https://api.jatsby.com/group?groupName=wolf%20creek
https://api.jatsby.com/group?groupName=copperleaf&groupType=subdivision
https://api.jatsby.com/group?groupName=3500%20Nightscape%20Circle
https://api.jatsby.com/group?groupName=sutton%20lakes&groupType=subdivision

#### Get Address - Get addresses by, well, address*, stateParcelId*, county
address* - search string for address, “3508 Night” will return “3508 Nightscape Circle Jacksonville FL 32224"
stateParcelId* - required if address is omitted and vice-versa
county - same as above, “duval” or 26
https://api.jatsby.com/address?address=3508%20Nightscape
https://api.jatsby.com/address?stateParcelId=C26-000-322-2259-8
https://api.jatsby.com/address?address=stanley%20steamer

#### Get Incident - Get incidents by groupName*, groupType* and county*, filter by startDate, endDate (basically hard-coded to last 30 days so just omit 'em)
https://api.jatsby.com/incident?groupName=Wolf%20Creek&groupType=2&county=duval
https://api.jatsby.com/incident?groupName=copperleaf&groupType=2&county=duval
https://api.jatsby.com/incident?groupName=sutton%20lakes&groupType=2&county=duval
