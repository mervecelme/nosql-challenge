# nosql-challenge


**GitHub Repository:** [nosql-challenge](https://github.com/a-dhil/nosql-challenge)

## Project Structure

- **Resources:** Contains the dataset file `establishments.json`.
  - `NoSQL_analysis_starter.ipynb`
  - `NoSQL_setup_starter.ipynb`

## Project Overview

The challenge focuses on evaluating food hygiene ratings provided by the UK Food Standards Agency. 

**Required Skills:** MongoDB, Python

### Part 1: Database Setup

mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json
The NoSQL_setup_starter.ipynb file is dedicated to setting up the database. 
It includes tasks such as importing the dataset, introducing a new restaurant ("Panang Flavours"), and deleting specific documents per client requirements.

### Part 2: Exploratory Analysis

In this phase, an exploratory analysis was conducted using the `NoSQL_analysis_starter.ipynb` notebook. The notebook addresses the following questions:

#### Q1: Which establishments have a hygiene score equal to 20?

For this question, the notebook employs MongoDB to query establishments with a hygiene score of 20.

#### Q2: Among London establishments, which have a `RatingValue` greater than or equal to 4?

The analysis focuses on identifying highly-rated establishments in London, specifically those with a `RatingValue` greater than or equal to 4.

#### Q3: What are the top 5 establishments with a `RatingValue` of 5, sorted by the lowest hygiene score, closest to "Panang Flavours"?

This query seeks to find the top-rated establishments in proximity to "Panang Flavours." The results are sorted by the lowest hygiene score.

#### Q4: How many establishments in each Local Authority area have a hygiene score of 0?

For this question, the analysis identifies areas where establishments have a hygiene score of 0.


