# NoSQL-Challenge
### Description
>The UK Food Standards Agency evaluates various establishments across the United Kingdom, and gives them a food hygiene rating. You've been contracted by the editors of a food magazine, *Eat Safe, Love*, to evaluate some of the ratings data in order to help their journalists and food critics decide where to focus future articles.

### Info / Credits

- Project by 
    * `jbarkle` 

- `REPO:` https://github.com/jbarkle/NoSQL-Challenge

## Introduction

This project consists of two technical products, including the following deliverables:

- Deliverable 1: Database and Jupyter Notebook setup

- Deliverable 2: Exploratory Analysis

## Part 1-1: Database and Jupyter Notebook setup

- Created an instance of the Mongo Client
- Confirmed that the database and the data were loaded properly
    - Listed the databases in MongoDB to confirm that "uk_food" is listed
    - Listed the collection(s) in the database to ensure that "establishments" is there
    - Found and displayed one document in the "establishments" collection using *find_one* and displayed with *pprint*.
- Assigned the "establishments" collection to a variable to prepare the collection for use

## Part 1-2: Update the Database

- Added information about a new halal restaurant that just opened in Greenwich to the database
- Found the *BusinessTypeID* for "Restaurant/Cafe/Canteen" and returned only the *BusinessTypeID* and *BusinessType* fields
- Updated the new restaurant with the *BusinessTypeID* found
- Removed any establishments within the Dover Local Authority from the database, and checked the number of documents to ensure they were deleted
- Used *update_many* to convert "latitude" and "longitude" to decimal numbers
- Used *update_many* to convert "RatingValue" to integer numbers
## Part 2: Exploratory Analysis

- Unless otherwise stated, the following format was used for each question:
    - Used *count_documents* to display the number of documents contained in the result
    - Displayed the first document in the results using *pprint*
    - Converted the result to a Pandas DataFrame, printed *X* rows in the DataFrame, and display the first 10 rows

- Analyzed the dataset by using Pandas functions to answer the following questions:
    >- Which establishments have a hygiene score equal to 20?
    >- Which establishments in London have a *RatingValue* greater than or equal to 4?
    >- What are the top 5 establishments with a *RatingValue* of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
    >- How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.
