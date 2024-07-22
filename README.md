# AI-Powered SQL Query Generator with Text

## Overview

This project demonstrates a web application built with Streamlit that leverages Google’s Generative AI (Gemini) to convert natural language questions into SQL queries. Users can interact with the app to ask questions about student data, which can be either pre-loaded or provided through an uploaded CSV file. The app dynamically adjusts to the schema of the uploaded data and generates SQL queries accordingly.

## Demo
#### Deployment Link: https://text-to-sql-llm-app.streamlit.app/

https://github.com/user-attachments/assets/551a3e8b-0bf0-484b-8950-6163ced4f753



## Features

- **Natural Language to SQL Conversion:** Uses Google Gemini to translate natural language questions into SQL queries.
- **CSV Upload:** Allows users to upload CSV files which are converted into an SQLite database.
- **Dynamic Schema Handling:** Adapts to different column names based on the uploaded CSV file.
- **Database Management:** Automatically handles and deletes temporary databases after use.
- **Interactive Interface:** Provides a user-friendly interface for querying and viewing results.

## Installation

1. Clone the repository:

   ```sh
   git clone https://github.com/yourusername/your-repository.git
   cd your-repository

2. Set up a virtual environment and install dependencies:

   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   pip install -r requirements.txt
   
3. Create a .env file in the root directory and add your Google API key:

   ```sh
   GOOGLE_API_KEY=YOUR_GOOGLE_API_KEY

