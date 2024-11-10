# SmartCourseFinder-HMI 🎓

This project was built by [Joshua Porunnedath Biju](https://github.com/JOSHUAPBIJU) and [Joyel Porunnedath Biju](https://github.com/joyelpbiju).

SmartCourseFinder-HMI is an intelligent web application for university course search, built using Python (Flask), SQLite, JavaScript, HTML, and CSS. This app interprets both explicit and implicit queries, using advanced vectorization techniques and word mapping to deliver precise and relevant course search results.

![Python](https://img.shields.io/badge/python-v3.8%2B-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen)

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Setting Up the Database](#setting-up-the-database)
- [Starting the Application](#starting-the-application)
- [Querying Courses](#querying-courses)
- [Accessing Course Details](#accessing-course-details)
- [Downloading Course Files](#downloading-course-files)
- [Directory Structure](#directory-structure)
- [Future Enhancements](#future-enhancements)
- [License](#license)

## Features
- 🔍 **Natural Language Query Parsing**: Supports both explicit and implicit queries.
- 🔗 **Flexible Search Operators**: Allows using operators like `title:`, `instructor:`, `AND`, `OR`, and more.
- 🗣️ **Synonym Mapping**: Recognizes alternative terms to improve query accuracy.
- 📊 **Weighted Similarity**: Uses cosine similarity with weighted facets for accurate result ranking.
- 🌐 **Translation Support**: Provides options to translate course details between English and German.
- 📂 **File Downloads**: Allows users to download PDF course files if available.

## Installation

### Prerequisites
Make sure you have the following installed:
- Python 3.8+
- Flask (for the web application framework)
- SQLite (for the database)
- Sentence Transformers (for vectorization)
- spaCy (for natural language processing)
- Googletrans (for language translation)

### Libraries
Install the necessary libraries using `pip`:

```bash
pip install Flask sqlite3 numpy sentence-transformers googletrans==4.0.0-rc1 spacy
