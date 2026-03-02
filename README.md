<img width="698" height="109" alt="image" src="https://github.com/user-attachments/assets/e18d3700-729a-4b5a-a073-3ab09ec939fc" />

# ArcGIS Online (AGOL) Field Metadata Updater

## Overview
This script streamlines the process of updating a feature service's field metadata (alias/description/value type) on ArcGIS Online (AGOL) thereby eliminating the need for manual entry using AGOL's interface. For this script to run successfully, it is recommended that you already have field metadata information ready for your service. This script was inspired by Lisa Berry's Hosted Feature Service Alias Updater script:https://github.com/lisaberrygis/AliasUpdater/tree/main. 

Created by: Farah Hoque, Esri Canada (2026)

## Why was this script created?
This script was created as a way to quickly update field metadata of feature services with multiple layers and many fields (30+) which would be cumbersome to do manually through AGOL's interface. The saved lookup table can also be used to recover a service's field metadata after it gets wiped out during an overwrite.  

## Who is this script for?
Anyone who wants to make their feature service more user-friendly and AI compatible.

## What can this script do?
The AGOL Field Metadata Updater has 2 main functions:
1. **Extracts** existing alias, description, and value type of fields in a feature service containing one or more layers and saves as a lookup table inside a folder. For a feature service with multiple layers, the lookup table will save each layer as a sheet with the layer name and layer ID. The user then needs to fill out the lookup table (see the attached SampleLookupTable.xlsx)
2. **Updates** the service on ArcGIS Online using the lookup table.

## Instructions
Download the AGOL_FieldMetadataUpdater_FH.py script and run it using any python IDEs (i.e., PyCharm, Visual Studio Code) that is configured with ArcGIS Pro.

## Requirements
- You must have ArcGIS Pro installed on your computer
- You must own the service you are trying to update


