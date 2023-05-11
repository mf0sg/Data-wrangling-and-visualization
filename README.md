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
The database enterprise for Marine Mammals Global Species Database was created using data from the International Union of Conservation of Nature (IUCN) Red List of Threatened Species. The Red List is created by groups of scientists who assess species under standardized, scientific criteria for their relative risk of extinction, expressed as a Red List Category. Assessments of the species are performed using informative data from the database including taxonomy, distribution (maps and GIS analysis), population information and status, habitat, ecology and life history, major threats, conservation measures, trade and use, and livelihoods. It is used by governments, wildlife departments, conservation-related organizations, non-governmental organizations (NGOs), and natural resource planners. 

The Marine Mammals Global Species Database captures the taxonomy, extinction risk, categorization, and country occurrences of each of the 187 species of marine mammals known to this planet. The taxonomy of the marine mammals in the database are identified using the hierarchy of biological organization. The taxonomy hierarchy includes kingdom, phylum, class, order, family, genus, and species. Quantitative criteria are applied to the species, and each species is assigned a Red List Category from 1-8 ranging from data deficient to extinct. In order, the risk assessment goes from data deficient > least concern > near threatened > vulnerable > endangered > critically endangered > extinct in the wild > extinct. For a species to be considered threatened, it must be classified as either vulnerable, endangered, or critically endangered. 

Marine mammals are regarded as highly intelligent creatures and unfortunately face many risks that threaten their populations. Major threats to marine animals include over-fishing, bycatch, trade, climate change, invasive species, coastal development, and more. The IUCN Red List is a powerful tool to measure the different pressures threatening species and is used to guide and inform on conservation actions. The subsets of data from the IUCN Red List, such as the Marine Mammal Global Species Database, allows for a variety of analyses and potential queries. 

# ER Diagram
![image](https://github.com/mf0sg/Data-wrangling-and-visualization/assets/88119103/b7617773-70ef-4fb6-b15e-94cb75739e8f)

# Requirements Description
The Marine Mammals Global Species Database stores information on all 187 species of marine mammals taken from the IUCN Red List. This database contains data about every species’ taxonomic ranking and their country (or countries) of occurrence. 
•	Each species is given a Latin name consisting of the organism’s genus and species. A genus is made up of more than one species, a family is made up of more than one genus, an order is made up of more than one family, a class is made up of more than one order, a phylum is made up of more than one class, and a kingdom is made up of many phyla. 
•	Marine mammals all share the same kingdom (Animalia), phylum (Chordata), and class (Mammalia). Several different orders make up the shared Mammalian class, and several different families make up an order. Families are made up of many different genera, and each genus can refer to one or more species. 
•	Each unique species is given a two-word Latin name comprised of its genus and species, sometimes called a Friendly Name. Each species has a name, a unique taxonomic identification number, a friendly name, and an assigned Red List category. The same species may exist in more than one country. Every country has a unique occurrence lookup value and the associated taxon identification number.
•	The database keeps a current record of all 187 known marine mammals. Information kept on each unique species includes their country of occurrence, habitats, threats, and population trends. 

# ER Diagram Uncaptured Constraints
The following is a list of constraints that are not captured by the ER diagram of Marine Mammal Biological Organization, Country Occurrence and IUCN Red List Category:
•	A specie’s taxon identification number must be a positive integer.
•	A specie’s category must be a two character combination specifically defined from the Red List species assessment. Options include EX (extinct), EW (extinct in the wild), CR (critically endangered), EN (endangered), VU (vulnerable), NT (near threatened), LC (least concern), or DD (data deficient). 

# Relational Schema: Syntax Summary and Table Details
![image](https://github.com/mf0sg/Data-wrangling-and-visualization/assets/88119103/36f37656-1d44-4c59-a60b-6f2bd3d65adf)

![image](https://github.com/mf0sg/Data-wrangling-and-visualization/assets/88119103/a02e4237-5a8b-4761-81ba-1a4714563bac)


