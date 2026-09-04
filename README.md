# service-nav-pbi
Power BI project for visualizing and exploring [gcperformance/service-data](https://github.com/gcperformance/service-data)

## What is this for?
This Power BI project is designed to help explore service and performance data from the GC Service Inventory, the inventory of services offered by the Government of Canada. Service data is stored in the [Open Government Portal](https://open.canada.ca/data/en/dataset/3ac0d080-6149-499a-8b06-7ce5f00ec56c), then processed with a Python (Pandas) script in [gcperformance/service-data](https://github.com/gcperformance/service-data).

## Who is this for?
Originally designed as an internal tool for the Service and Digital Performance team with Treasury Board of Canada Secretariat, Office of the Chief Information Officer, to assist analysts in answering ad-hoc questions, revealing data quality issues, exploring connections between services, their associated standards, and the programs that deliver them. Shared for the benefit of anyone who is interested in detailed or summary information relating to the GC Service Inventory.

## How to use this resource
1. Download and install [PowerBI Desktop](https://www.microsoft.com/en-us/power-platform/products/power-bi/desktop)
2. Download the code as a .zip file
3. Extract the files from the .zip file 
4. Open the **si-nav.pbip** file
5. Refresh the data

## Contents
The Power BI dashboard structures service data through queries designed in Power Query, then divides and presents the information in a series of tabs.

### Tabs
#### Service Navigator
The original tool designed to find connections between services, standards and programs. Three linked tables that filter one another through clicking on the row-level records, one table for services, one for service standards, and another for programs.

#### Summary
An at-a-glance summary of GC Service Inventory data.

#### Service Details
Information specific to a single service. Can be filtered using the filter pane, or used as a destination for drill-through from any service-level visual, such as the Service Identification and Metrics table in the **Service Navigator** tab.

#### Service Comparison
Compares some basic information for two services, selected individually.

#### Snapshot Comparison
Compares the current state of the GC Service Inventory (as of the latest refresh of the tool) to a specific data snapshot taken to fix annual corporate reporting results. Displays changes to fields, added records, and records removed.

#### Data Quality Summary
Summary of data quality issues identified by the [gcperformance/service-data](https://github.com/gcperformance/service-data) script, broken down by organization and severity.

#### Data Quality Details
Detailed descriptions of every data quality issue identified in [gcperformance/service-data](https://github.com/gcperformance/service-data) for services and standards. Functions as a target for drill-through from the **Data Quality Summary** tab.

#### Reference
Data dictionary for field names.

## Troubleshooting
If pop-ups regarding "Access Web Content", privacy labels, or information sensitivity appear during a data refresh, select "Anonymous" or ignore the popup. All data referenced are public.

There can be an issue with the file path length if extracted within a user's documents. It may be possible to solve this by extracting to the C:\ drive directly.
