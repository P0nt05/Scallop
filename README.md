# Digital Experience Assessment via Cisco Umbrella
## Short Description:
### Cisco SecureX Action Orchestrator Workflow - Cisco Umbrella / Top Destination to ThousandEyes
This project is to start your Digital Experience Assessment. 
The primary Use case is to a assess the most used applications (Top Destinations) within your organization.
We leverage a Cisco SecureX Orchestration workflow to get the Top Destinations (Top 10) via the Cisco Umbrella Reporting API.
Finally we create for each domain a synthetic HTTP Page-load test in ThousandEyes.

For more informations about the API's
  Umbrella Reporting API - https://docs.umbrella.com/umbrella-api/docs/about-the-umbrella-api
  ThousandEyes API - https://developer.thousandeyes.com/v6/

**NOTE:**
  This is the first commit, please feel free to change or adopt the Use case to your requirements!


## Features:
  tbc
## Roadmap
  tbc
  
  
## How it works

# Extract Top Destination from Cisco Umbrella
We receive via an API request the Top 10 list of the most requested domains within your organization over the selected time period. (24 hours)
They are filtered by the content category - Business Services
![Umbrella Top Categories](https://files.readme.io/87c54e3-top_categories_dns_only.png)

# HTTP Page-Load test creation
The Top 10 list is the source for the creation of the HTTP Load-page tests in order to monitor the Digital Expirience inside ThousandEyes.
All tests are created via an API request with default Test metadata, like Intervall, Alert, ...
![TE HTTP page-load](https://gblobscdn.gitbook.com/assets%2F-M4QARF6s57qxMrOHDTZ%2Fsync%2Fc3d13233b3338ad0f75ba262e74a5a44c103ed93.png?alt=media)

# SecureX Orchestration workflow - Overview

Here a short overview of the SXO workflow:
![SXO workflows](https://github.com/P0nt05/Scallop/blob/main/IMAGES/workflow.gif)

# Installation
## Detailed installation instructions can be found [HERE](https://github.com/P0nt05/Scallop/blob/main/INSTALL.md)
