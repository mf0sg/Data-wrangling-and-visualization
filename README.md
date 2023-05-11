# IUCNRedList
Cleaned, wrangled, queried, and visualized data from IUCN Redlist of Threatened Species public data.
Designed a conceptual model for a relational database using ER diagrams, ER diagram constraints, requirements and 
description of enterprise, and a relational schema.

# About
This project was completed to design and implement a database using public data from the IUCN Redlist of 
Threatened Species. The database schema and table structures I designed were used to implement a MySQL
database. I first wrote SQL DDL instructions for defining the relations in the database. Python (pandas) was
then used to wrangle the data into csv files generated to populate the relational databases defined in MySQL. 
Two queries were then defined and executed from the database. Matplotlib was used to visualize the data 
from the queries. 

# Introduction
The database enterprise for Marine Mammals Global Species Database was created using data from the International Union of Conservation of Nature (IUCN) Red List of Threatened Species. The Red List is created by groups of scientists who assess species under standardized, scientific criteria for their relative risk of extinction, expressed as a Red List Category2. Assessments of the species are performed using informative data from the database including taxonomy, distribution (maps and GIS analysis), population information and status, habitat, ecology and life history, major threats, conservation measures, trade and use, and livelihoods2. It is used by governments, wildlife departments, conservation-related organizations, non-governmental organizations (NGOs), and natural resource planners1. 

The Marine Mammals Global Species Database captures the taxonomy, extinction risk, categorization, and country occurrences of each of the 187 species of marine mammals known to this planet. The taxonomy of the marine mammals in the database are identified using the hierarchy of biological organization. The taxonomy hierarchy includes kingdom, phylum, class, order, family, genus, and species. Quantitative criteria are applied to the species, and each species is assigned a Red List Category from 1-8 ranging from data deficient to extinct. In order, the risk assessment goes from data deficient > least concern > near threatened > vulnerable > endangered > critically endangered > extinct in the wild > extinct2. For a species to be considered threatened, it must be classified as either vulnerable, endangered, or critically endangered2. 

Marine mammals are regarded as highly intelligent creatures and unfortunately face many risks that threaten their populations. Major threats to marine animals include over-fishing, bycatch, trade, climate change, invasive species, coastal development, and more1. The IUCN Red List is a powerful tool to measure the different pressures threatening species and is used to guide and inform on conservation actions. The subsets of data from the IUCN Red List, such as the Marine Mammal Global Species Database, allows for a variety of analyses and potential queries. 

# ER Diagram
![image](https://github.com/mf0sg/Data-wrangling-and-visualization/assets/88119103/4d5ccb20-98da-4aa7-b60b-03fd6ae2dbfb)



