# NC_Capstone
Capstone project for Code:YOU. Analyzing U.S. employment by sector over time versus U.S. Business A.I. sentiment. 

# AI Usage by U.S. State — Analysis Dataset

This dataset tracks reported adoption of Artificial Intelligence (AI) technologies by businesses across U.S. states over time, using public data from the U.S. Census Bureau's Business Trends and Outlook Survey (BTOS).

This repository brings together two key sources of labor and AI adoption data by U.S. state:

Bureau of Labor Statistics (BLS) Occupational Data

U.S. Census Bureau Business Trends and Outlook Survey (BTOS)

These datasets are joined by state acronym (PRIM_STATE / State) to support analysis of how AI usage may be impacting employment patterns across states and time.

# Running the Program:

The following is a guide to running the project files locally:

Fork the repository    
Clone the repository to your Github account 
    ```bash
    git clone https://github.com/username/NC_Capstone.git
    cd NC_Capstone
Access the repository from your command line or preferred CMD software  
Install a virtual environment. The command in Gitbash is python -m venv venv  
Activate the virtual environment. The command in Gitbash is source venv/scripts/activate  
Install the requirements.txt file to install necessary packages by running pip install requirements.txt  

# Data Summary
BLS Occupational Data  
Rows	185,755  
Columns	33  
Time Period	Annual (2020–2024 across files)  
Source Files	state_M2020_dl.xlsx through state_M2024_dl.xlsx

BTOS AI Adoption Data  
Rows	5,036    
Columns	82  
Time Period	Biweekly, 2022–2025  
Source Files	State.xlsx, State_v1.xlsx

# Data Dictionary
https://github.com/ncamic/NC_Capstone/blob/main/capstone_data_dictionary.ipynb


# Data Sources
BLS Occupational Employment and Wage Statistics (OEWS):
[https://www.bls.gov/oes/](https://www.bls.gov/oes/tables.htm)

Census Bureau Business Trends and Outlook Survey (BTOS):
[https://www.census.gov/econ/bfs/](https://www.census.gov/hfp/btos/data_downloads?utm_source=chatgpt.com)


# Project Objective:
Track adoption of AI by state over time (using sentiment as a proxy.) 
Compare employment trends across occupations and states.
Join both datasets by State to assess possible displacement or complementarity of labor and AI.

# Summary Notes for Module 3 Submission:

I intend to look primarily at tech related occupational data by U.S. State (using job codes) and compare that with the more qualitative Census Business Outlook survey questions which pertain to A.I. to compare at a State and occupational level over time how A.I. business sentiment has correlated with employment figures. I plan to also explore other occupational job codes outside of tech but will start there. 

I plan to graph on time-series charts employment trends in comparison to business A.I. sentiment in Tableau (using cleaned and curated Python data) to be able to dynamically look for interesting trends in the relationship between business A.I. sentiment and employment by State and occupational groups to see if there is an effect from A.I. "enthusiam" (perhaps a proxy for adoption) on employment in any particular occupational areas (again particulary interested in tech but will look elsewhere as well.)

I will need to bucket the numerous job codes into higher level occupational categories and that work is not completed yet but I intend to do so for ease of analysis and will publish those groupings within this repository. 

# Technologies Used

Python — The main programming language used for data processing.
Pandas — For cleaning, joining, and manipulating large datasets.
NumPy — For numerical operations and handling large data arrays efficiently.
Matplotlib & Seaborn — For creating initial visualizations and exploring trends in the data.
pandasql — For using SQL queries directly on Pandas DataFrames during data exploration.
SQLite3 — For lightweight database operations during development.
Jupyter Notebook — For combining code, explanations, and results in an easy-to-follow format.

# Overall Project Summary

My primary goal with this analysis was to explore the relationship between business A.I. sentiment as tracked by the U.S. Census Bureau against employment trends over the same period as tracked by the U.S. Bureau of Labor Statistics. Ultimately, at a regional level there appeared to be a strong negative correlation between A.I. sentiment and tech labor employment, however, at a state level this correlation became much less strong. To me this suggested that so far there is likely not much of a relationship between A.I. sentiment and tech employment, but the issue may worth watching given the high level correlation that the data presented. Some challenges I faced during this project were that BLS only publishes data annually, so while full year 2024 is not bad to have, we are missing 6 months of data in 2025 effectively - and with A.I. change occurs rapidly. I also found the data to be very rich in terms of what was available, and originally I would have liked to break down the relationship of A.I. to non-tech jobs in several categories, but that could go in many directions, and in the interest of time and applicability I chose to focus on tech jobs.  


