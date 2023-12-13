# Squadcast Assignment - By Ishika Gupta
This repository contains the code for the assignment provided by Squadcast for Data Engineer Position. The assignment is present in the file titled **"Data Engineer Assignment.pdf"**.

## Implementation Process

### Importing Data
1. Create an account on Render (if not signed up already).
2. Create a new postgresql instance.
3. Download a postgresql client (pgAdmin 4) and connect it to the postgresql database using appropriate credentials.
4. Create 2 new tables "movies" and "ratings" keeping in mind the column headers and their data types using the following commands in SQL query tool:
  ```
CREATE TABLE movies (
	id INT,
	title VARCHAR(255),
	year INT,
	country VARCHAR(255),
	genre VARCHAR(255),
	director VARCHAR(3000),
	minutes INT,
	poster VARCHAR(255)
);
```
and
  ```
CREATE TABLE ratings (
	rater_id INT,
	movie_id INT,
	rating INT,
	time INT
);
```
5. Import data from "movies.csv" and "ratings.csv" to the tables created.
6. Verify if the data is imported successfully in both the tables using the following commands in SQL query tool:
```SELECT * FROM movies;```
and
```SELECT * FROM ratings;```

### Connecting jupyter notebook to postgresql database for accessing the tables and performing Data Analysis

The **Python** implementation code for connecting jupyter notebook to postgresql database for accessing the tables and for performing data analysis with comments for explanation is present in the jupyter notebook titled **"Ishika - Assignment - Squadcast.ipynb"**.
Note: For executing the cells upload data to your postgresql database and connect using your respective credentials.
