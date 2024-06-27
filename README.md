# Overview

I've been working on a project to learn web scraping and SQLite. For this, I scraped data for some of the top movies from IMDb. I gathered details like the title, release year, duration, age rating, score, and review count.

After collecting the data, I set up a SQLite database to store it all. I created a table with columns for each piece of information. Then, I practiced running basic queries: inserting new records, updating them, retrieving specific data, calculating averages, and grouping data by age rating.

[Code Walkthrough](https://youtu.be/bloZ9O9LKHk)

# Relational Database

I created a single table in the SQLite database to store information about the top 25 movies from IMDb. The table is structured as follows:

Table: movies_data

title (TEXT): The title of the movie.

release (REAL): The release year of the movie.

length_min (REAL): The duration of the movie in minutes.

age_rating (TEXT): The age rating of the movie (e.g., PG-13, R).

score (REAL): The IMDb score of the movie.

review_count (REAL): The number of reviews the movie has received.

This table allows me to store and manage the movie data efficiently, and it provides a foundation for running queries to analyze the data.

# Programming Language and Libraries

Programming Language: Python
Python was chosen for this project because it is simple to implement web scraping and database operations. Here are the key libraries I used:

BeautifulSoup: A library used for parsing HTML documents. It helps in searching the HTML structure to extract data.

Requests: A simple HTTP library for Python, used to send HTTP requests to IMDb and fetch the web page containing the movie data.

SQLite3: A built-in Python library that provides a disk-based database. It allows for interaction with SQLite databases directly from Python code.

# Useful Websites

- [Great Webscrapping Info](https://www.youtube.com/watch?v=QhD015WUMxE)
- [W3Schools](https://www.w3schools.com/sql/default.asp)
- [Python SQLite Documentation](https://docs.python.org/3/library/sqlite3.html)
- [Geeks For Geeks](https://www.geeksforgeeks.org/python-web-scraping-tutorial/)
- [Curl Converter](https://curlconverter.com/)

# Future Work

- Error Handling: Implement error handling to manage issues such as network errors during web scraping, invalid data formats, and database failures.
- Data Validation: Add data validation to ensure the accuracy of the data being scraped and stored in the database.
- Data Visualization: Add data visualization features to present the results of queries in a more visually appealing manner.