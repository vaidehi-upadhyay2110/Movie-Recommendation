Project Tile- Basic Content-Based Movie Recommendation System (CLI)

Project Overview - This project is a CLI application developed in Python meant to illustrate the concept of Content-Based Filtering. The system proposes a movie recommendation based solely on the genre attributes (content) of a selected movie and measures the overlap (similarity) of that movie with every other movie in the static, in-memory database. In response, the output is a scored-ranked title list of suggestions, based on the genre match score.

Features-

In-Memory Data Storage: All movie data (title and list of genres) is temporarily stored in a Python dictionary for rapid retrieval.
Scoring Genre Similarity: Each genre is processed as a Python set, employing Python’s efficient set intersection method for counting a number of total matching genre categories between two movies.
Sorted Recommendations: Recommendations (output) is sorted in descending order by genre match score.
Initialization Available Movies Display: The dataset of available movies is displayed on startup.
Robust Error Handling: The user is notified if the specified movie title is not present in the database. Technologies/Tools Used • Language: Python 3.x • Tools: Standard Python environment. • Core Data Structures: Python dict for the movie catalog, list as a placeholder for genres, and set as the core data structure.
Technological Solutions/Methods Utilized • Programming Language: Python 3.x. • Additional Implementation: Standard Python Environment. • Primary Data Structures: Python dict for the movie catalog, list for genres, and set for similarity calculations.

Installation and Usage Procedure

Store Code: Persist the provided code on a file named ME.py.
Locate Terminal: Utilize the command line or terminal to locate the directory where ME.py is located.
Execute Code: Run the file with Python's interpreter.
python ME.py
Obey Prompt: The script will launch with the movies available. Enter in the question the name of one of the movies displayed (Inception or Titanic, for example) for movie recommendations
Testing Directions- In order to test that the system runs correctly, use the following tests: 1.Test Case- Input Movie What to Expect 2.High Match- Inception Two matches in genres (sci-fi, action or thriller). Should recommend Tenet and Interstellar (if they match other the genre). 3.Low Match- The Dark Knight One match in genres (action or crime). Will recommend excluding Titanic. 4.No Match- Titanic Recommendations will include Notebook (score 2) and Interstellar (score 1). 5.Error Handling- A movie not in the list (avatar) Print: "Movie not found in"
