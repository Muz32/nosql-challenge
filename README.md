# nosql-challenge

I utilized MongoDB, a NoSQL database management system, to analyze data from the UK Food Standards Agency.  The analysis focused on ratings (such as hygiene) of various establishments across the United Kingdom. The insights derived from this analysis aimed to assist journalists and food critics in identifying areas of interest for future articles. 

## Tools Used
- **MongoDB**: For storing and querying the data.
- **Jupyter Notebook**: For conducting data analysis and creating pandas dataframes.
- 
## Analysis Approach
This assignment challenge was completed in three parts: 

### Part 1: Database and Jupyter Notebook Setup
- **File Used**: `NoSQL_setup.ipynb`
- **Data Import**: The 'establishments.json' file was imported into MongoDB using terminal commands.
- **Database Configuration**: A MongoDB database named 'uk_food' was created, and a collection named 'establishments' was prepared for data analysis.
- **Libraries Used**: Imported **PyMongo** and **Pretty Print** libraries in Jupyter Notebook for MongoDB interaction and data readability.
- 
### Part 2: Update the Database
In this phase, several modifications were made to the MongoDB database using Jupyter notebook file `NoSQL_setup.ipynb`:
- Added a new restaurant, 'Penang Flavours,' to the database.
- Updated the new restaurant's 'BusinessTypeID'.
- Excluded establishments in 'Dover' from the analysis.
- Converted ‘latitude’ and ‘longitude’ fields to decimals, and ‘RatingValue’ to an integer to ensure precise analysis outcomes.

### Part 3: Exploratory Analysis
Conducted exploratory queries and transformed results into Pandas DataFrames using `NoSQL_analysis.ipynb`:
- Identified establishments with a hygiene score of 20.
- Found establishments in London with a `RatingValue` greater than equal to 4.
- Listed top 5 establishments with a `RatingValue` of 5, sorted by lowest hygiene score and proximity to 'Penang Flavours.'
- Calculated the count of establishments with a hygiene score of 0 by Local Authority area, ordered from highest to lowest.

## Files
- `NoSQL_setup.ipynb`: code for part 1 and part 2.
- `NoSQL_analysis.ipynb`: code for part 3.
  - `Resources`
    - `establishments.json`: Raw data file.
   
## Source of Data
The data was provided by edX Boot Camps LLC and sourced from the UK food hygiene rating data API (https://ratings.food.gov.uk/open-data/en-GB).
