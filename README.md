# DomesticViolencePortugal
 Project involving Data Integration Analysis

This project consists on the creation of a Pentaho Data Integration transformations and the storage of spatial information in a PostGIS database. 

# Problem Statement

We have a list of Districts (Cities) of Portugal to geocode. This list is stored in a csv file and in each line, we have those Districts with other attributes such as the Ano (Year), the Entidade (Entity) and the Valor (Value).

We wish to create a transformation using Google's geocoding service (http://maps.googleapis.com/maps/api/geocode/json?address=...&sensor=false) to obtain the coordinates of these districts. 
Therefore, a JSON document will be obtained, the nodes of the document will be processed, and the information of interest is selected. 
Next, we create a geometry and generate not only a table output but also a GIS file to represent the spatial information in PostGis.

# Data Analysis

The Data in question is about the number of Domestic Violence occurrences in Portugal Continental and their Autonomous Regions registered by the Security Forces (GNR and PSP) between 2008 and 2014.

Relatively to the data of the Autonomous Regions, there is some data about the GNR that appears in the file with a 0 (zero) occurrences and ND (not available).

The source of this data was provided by DGAI (Internal Administration of General Direction).

The data is stored in a csv file and can be found here: http://centraldedados.pt/violencia_domestica/.
