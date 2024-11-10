# SmartCourseFinder-HMI

SmartCourseFinder-HMI is an intelligent web application for university course search, built using Python (Flask), SQLite, JavaScript, HTML, and CSS. This app interprets both explicit and implicit queries, using advanced vectorization techniques and word mapping to deliver precise and relevant course search results.

 #Features
•	Natural Language Query Parsing: Supports both explicit and implicit queries.
•	Flexible Search Operators: Allows using operators like `title:`, `instructor:`, `AND`, `OR`, and more.
•	Synonym Mapping: Recognizes alternative terms to improve query accuracy.
•	Weighted Similarity: Uses cosine similarity with weighted facets for accurate result ranking.
•	Translation Support: Provides options to translate course details between English and German.
•	File Downloads: Allows users to download PDF course files if available.

#Installation

 Prerequisites
•	Make sure you have the following installed:
•	Python 3.8+
•	Flask (for the web application framework)
•	SQLite (for the database)
•	Sentence Transformers (for vectorization)
•	spaCy(for natural language processing)
•	Googletrans(for language translation)

 #Libraries
Install the necessary libraries using `pip`:
	pip install Flask sqlite3 numpy sentence-transformers googletrans==4.0.0-rc1 spacy

Make sure to install the English language model for spaCy:
	python -m spacy download en_core_web_sm

#Setting Up the Database
Place your `courses.sqlite` file in the specified database directory (`E:/HSM/project_hmi/webappcoursespot/db/`)
 
 #Starting the Application
Run the following command to start the Flask application:
	python app.py

#Querying Courses
You can search for courses using either explicit operators or natural language queries. Examples of supported queries:
•	Explicit Queries: Use operators like `title:`, `instructor:`, `credit:`, etc., to narrow down results.
•	Implicit Queries: Enter natural language queries (e.g., "courses on AI taught by Smith in summer term") to get results through the system's NLP parsing.

#Accessing Course Details
Click on any course in the search results to view detailed information, including learning objectives, course content, prerequisites, etc. You can also translate the details between English and German.

#Downloading Course Files
If a course has an associated PDF file, you can download it by clicking the “Download Course PDF’ button in the course details section.

#Directory Structure

•	app.py: Main backend application file with route handlers and query processing.
•	index.html: Frontend HTML file for rendering the user interface.
•	mappings.py: Contains mappings and synonyms used for converting implicit queries to explicit ones.

#Future Enhancements
- Add more languages for translation.
- Improve the parsing for more complex natural language queries.
- Extend synonym mappings for additional terms.

