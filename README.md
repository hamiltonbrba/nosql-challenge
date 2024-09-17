# nosql-challenge
Module 12 Challenge - NOSQL

# Eat Safe, Love: UK Food Establishments Data Analysis

This project is an analysis of food hygiene ratings for various establishments across the United Kingdom, using data provided by the UK Food Standards Agency. The goal of the project is to help journalists and food critics at *Eat Safe, Love* decide where to focus their future articles.

## Table of Contents

- [Project Overview](#project-overview)
- [Setup Instructions](#setup-instructions)
- [Part 1: Database and Jupyter Notebook Setup](#part-1-database-and-jupyter-notebook-setup)
- [Part 2: Update the Database](#part-2-update-the-database)
- [Part 3: Exploratory Analysis](#part-3-exploratory-analysis)
- [Code Source and Attribution](#code-source-and-attribution)
- [Contact](#contact)

## Project Overview

This project involves setting up a MongoDB database named `uk_food`, importing a dataset of UK food establishments, and performing various updates and queries to explore the data. The analysis is designed to provide insights into the hygiene standards of establishments across the UK and identify areas of interest for future articles by *Eat Safe, Love*.

## Setup Instructions

1. **MongoDB Setup:**
   - Use the Terminal to import the data from the `establishments.json` file into MongoDB.
   - Run the following command in the Terminal to import the data:
   ```bash
   mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json

2. **Install Required Libraries:**
   - Ensure you have the necessary libraries installed:
   ```bash
   pip install pymongo pandas
   ```

3. **Run Jupyter Notebooks:**
   - Open the Jupyter notebooks `NoSQL_setup_starter.ipynb` and `NoSQL_analysis_starter.ipynb` to execute the required steps.

## Part 1: Database and Jupyter Notebook Setup

- This section covers setting up the MongoDB database, importing the data, and verifying that the data is correctly loaded.
- **Code Location**: `NoSQL_setup_starter.ipynb`
  - Import the data into MongoDB.
  - Verify database and collection setup.
  - Use `pymongo` and `pprint` to confirm data import and setup.

## Part 2: Update the Database

- The database is updated as per the magazine editors' requests:
  - Adding a new restaurant "Penang Flavours".
  - Removing all establishments within the Dover Local Authority.
  - Converting data types for latitude, longitude, and rating values.
- **Code Location**: `NoSQL_setup_starter.ipynb`
  - Update operations to modify the database contents.

## Part 3: Exploratory Analysis

- Conduct an exploratory analysis to answer specific questions posed by the magazine editors:
  - Establishments with a hygiene score equal to 20.
  - Establishments in London with a `RatingValue` greater than or equal to 4.
  - Top 5 establishments near "Penang Flavours" with a `RatingValue` of 5.
  - Count of establishments in each Local Authority area with a hygiene score of 0.
- **Code Location**: `NoSQL_analysis_starter.ipynb`
  - Perform queries, aggregation, and data analysis using `pymongo` and `pandas`.

## Code Source and Attribution

This project includes code and techniques from various sources:

- **Data Import Command**: The `mongoimport` command is used to import data into MongoDB.
- **MongoDB Query Examples**: Located in `NoSQL_setup_starter.ipynb` and `NoSQL_analysis_starter.ipynb`. These queries were developed using the MongoDB documentation as a reference.
- **Aggregation Pipeline Techniques**: Used for data analysis in `NoSQL_analysis_starter.ipynb`, inspired by community resources such as Stack Overflow.
  

## Contact

If you have any questions or need further information, feel free to contact:

- **Bryan Hamilton-Brown**: [bryan.hb.analytics@gmail.com](mailto:bryan.hb.analytics@gmail.com)
- **GitHub Profile**: [hamiltonbrba](https://github.com/hamiltonbrba)
```
