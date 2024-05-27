# nosql-challenge

This project leveraged the NoSQL database management system, MongoDB, to analyze data from the UK Food Standards Agency. The analysis focused on different types of ratings (including hygine) of various establishments across the United Kingdom. The insights derived from this analysis aimed to assist journalists and food critics in identifying areas of interest for future articles. 

## Tools Used
- **MongoDB**: Utilized for data storage and querying.
- **Jupyter Notebook**: Employed for performing data analysis and visualizations.

## Analysis Approach
The challenge was tackled in three distinct parts:

### Part 1: Database and Jupyter Notebook Setup
- **File Used**: `NoSQL_setup.ipynb`
- **Data Import**: Imported 'establishments.json' into MongoDB via terminal commands.
- **Database Configuration**: Created a MongoDB database `uk_food` and prepared a collection `establishments` for analysis.
- **Libraries Used**: Imported PyMongo and Pretty Print in Jupyter Notebook for MongoDB interaction and data readability enhancement.

### Part 2: Update the Database
Using the `NoSQL_setup.ipynb` notebook, the following updates were made:
- Added a new restaurant, 'Penang Flavours,' to the database.
- Updated the new restaurant with its respective `BusinessTypeID`.
- Excluded establishments in 'Dover' from the analysis.
- Converted 'latitude' and 'longitude' fields to decimal, and 'RatingValue' to integer for better analysis.

### Part 3: Exploratory Analysis
Conducted exploratory queries and transformed results into Pandas DataFrames using `NoSQL_analysis.ipynb`:
- Identified establishments with a hygiene score of 20.
- Found establishments in London with a `RatingValue` ≥ 4.
- Listed top 5 establishments with a `RatingValue` of 5, sorted by lowest hygiene score and proximity to 'Penang Flavours.'
- Calculated the count of establishments with a hygiene score of 0 by Local Authority area, ordered from highest to lowest.
