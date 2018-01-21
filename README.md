# SUDS Fire Commercial
This project is to further previous work on Fire Risk Modeling for Metro 21 and the Pittsburgh fire department.

## How to set up

Download data files into /datasets:
* pittdata.csv, parcels.csv, pli.csv from getdata.py
* Fire_Pre14, Fire_New from Google Drive


## Run_Model.sh
Runs all three python scripts listed below in succession.


## getdata.py

Scrapes [WPRDC](wprdc.org) for:
* City of Pittsburgh property data ("pittdata.csv")
* City of Pittsburgh parcel data ("parcels.csv")
* Permits, Licenses, and Inspections data ("pli.csv")

## riskmodel.py

Runs the risk prediction model, using:
* the three datasets from WPRDC
* Fire Incident data from PBF

## merger.py

Takes the output of the risk model, and merges each property's risk score with the rest of the property data in pittdata and parcels, sending the output to the BEV directory

## requirements.txt

All of the packages you'll need to install for these scripts to run
