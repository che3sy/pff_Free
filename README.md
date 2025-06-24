# Get all info from [PFF](https://www.pff.com/) 

They have 2 apis:
- https://www.pff.com/api/
- https://consumer-api.pff.com/
___
### First Api Endpoint:
Used for the projection and other things idk 
GET /api/fantasy/projections?scoring={scoringType}&weeks={number of weeks}
(their is prob more)

#### scoringType 
- Allowed values:
  - ppr
  - halfPPR
  - standard
  - pprSuperflex
  - halfPPRSuperflex
  - standardSuperflex

---

### Second Api Endpoints
(their is prob more enpoints)
This one is more intresting, it requieres a api key and gives all info for the rankings (including projection) 

Here is the key lol:<br>
``Api-Key: 0f6ca1f4-79d4-11ee-b962-0242ac120002``

GET /football/v1/fantasy/rankings?page={amount of pages duh}&leagueType={leagueType}d&scoringType={scoringType} 
#### scoringType 
- Allowed values:
  - REDRAFT_HALF_PPR
  - REDRAFT_IDP
  - DYNASTY_ROOKIE
  - BEST_BALL
  - REDRAFT_PPR
  - DYNASTY_STARTUP
  - DYNASTY_IDP_ROOKIE
  - REDRAFT_NON_PPR
  - REDRAFT_2QB_PPR
  - DYNASTY_2QB_ROOKIE
  - DYNASTY_IDP_STARTUP
  - DYNASTY_2QB_STARTUP

#### leagueType
standard is default, but anything works for some reason idk 
  

GET /football/v1/fantasy/weekly-rankings?position={position}&scoringType={scoringType}&page={amount of pages duh}
#### scoringType 
- Allowed values:
  - ppr
  - halfPPR
  - standard
  - pprSuperflex
  - halfPPRSuperflex
  - standardSuperflex
#### position 
- Allowed values:
  - QB
  - RB
  - WR
  - TE
  - FL
  - SFL
  - K
  - D
