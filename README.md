# MIT COVID-19 Challenge Datathon

## New York City Vulnerable Neighborhoods Based on Community Health Conditions & Connections to COVID-19

###  A. Methodology Overview

1. Cluster vulnerable neighborhoods based on pre-existing health conditions
2. Identify relationships between clusters and COVID-19 cases per capita
3. identify neighborhood clusters that should be the focus of greater testing/preventative public health measures
4. Determine high-need neighborhoods based on the ratio between cases per capita and tests per capita
5. Prioritize the allocation of COVID-19 resources

###  B. Data

#### Community Health Condition Statistics

* http://a816-dohbesp.nyc.gov/IndicatorPublic/Subtopic.aspx
* Run by the NYC Department of Health and Mental Hygiene
* The following conditions were chosen because they have been demonstrated by the CDC to put people at higher risk for severe illness from COVID-19:
  * Heart Attack
  * Chronic obstructive pulmonary disease (COPD)
  * Asthma
  * Obesity
* Has neighborhood codes in UHF34 or UHF 42 standards

Reference: https://www.cdc.gov/coronavirus/2019-ncov/need-extra-precautions/people-at-higher-risk.html

#### NYC COVID-19 Data
* https://github.com/nychealth/coronavirus-data
* Updated daily
* Assembled by the NYC Department of Health and Mental Hygiene
* Has data per modified ZIP Code Tabulation Area (MODZCTA)

###  C. Findings

#### NYC Clusters based on Health Condition Statistics
![NYC Clusters](https://github.com/nqtri/mit_covid19_challenge/blob/master/img/cluster.png)

![NYC Cluster Map](https://github.com/nqtri/mit_covid19_challenge/blob/master/img/nyc_clustermap.png)

All of Bronx and Staten Island neighborhoods are in Cluster 0. Most neighborhoods in Manhattan are in Cluster 1. Queens dominates Cluster 2.


#### Allocation of COVID-19 Resources for High Risk Clusters

![Cluser 0](https://github.com/nqtri/mit_covid19_challenge/blob/master/img/cluster0.png)

![Cluster 2](https://github.com/nqtri/mit_covid19_challenge/blob/master/img/cluster2.png)

Canerise - Flatlands and Southeast Queens in Cluster 0; Jamaica, Fordham - Bronx Park, and Rockaways in Cluster 2 seem to be under-tested.

###  D. Challenges & Limitations

* Finding datasets with consistent granularity
* Finding a large number of health indicator features in public datasets

###  E. Next Steps

* Build on our proof-of-concept by evaluating additional health conditions and
additional cities
* Allocate resources to high risk areas
* Build regression models that can potentially predict COVID-19 case rate
based on underlying health conditions
* Identify health factors that drive COVID-19 cases in certain neighborhoods

* Possible Expansion of Dataset:
 * https://www.cdc.gov/500Cities/
 * https://www.huduser.gov/portal/datasets/usps_crosswalk.html
 
