AI-Powered SQL Query Generator
Overview
This project is a Streamlit application that leverages Google’s Generative AI to convert natural language questions into SQL queries. The app supports querying an SQLite database, either using a predefined student dataset or a user-uploaded CSV file. It dynamically adjusts to the schema of the uploaded data, ensuring accurate SQL query generation based on the actual database schema.

Features
Natural Language to SQL Query: Convert natural language questions into SQL queries using Google’s Generative AI.
Dynamic Schema Handling: Automatically adjust SQL queries based on the columns of the uploaded CSV file or the default student dataset.
CSV Upload: Users can upload their own CSV files, which are converted into an SQLite database for querying.
Database Cleanup: Automatically delete the temporary SQLite database after the task is completed to avoid clutter.
Technologies
Streamlit: For creating the interactive web application.
Google Generative AI: For generating SQL queries from natural language.
SQLite: For database management.
Pandas: For handling CSV files and converting them into SQLite tables.
Python-dotenv: For managing environment variables securely.
Setup
Clone the Repository:

sh
Copy code
git clone https://github.com/your-username/ai-sql-query-generator.git
cd ai-sql-query-generator
Install Dependencies:

sh
Copy code
pip install -r requirements.txt
Create a .env File:
Create a .env file in the project directory and add your Google API key:

plaintext
Copy code
GOOGLE_API_KEY=YOUR_GOOGLE_API_KEY
Run the Application Locally:

sh
Copy code
streamlit run app.py
Deployment
Streamlit Cloud
Go to Streamlit Cloud and log in or sign up.
Create a new app and connect your GitHub repository.
Set the environment variable GOOGLE_API_KEY in the app settings.
Deploy the app by clicking on Deploy.
Heroku (Alternative)
Create a requirements.txt file and a Procfile as described in the Setup section.
Create a new app on Heroku.
Deploy the app using Git:
sh
Copy code
heroku create
git push heroku master
Set the environment variable GOOGLE_API_KEY on Heroku:
sh
Copy code
heroku config:set GOOGLE_API_KEY=YOUR_GOOGLE_API_KEY
Usage
Open the app in your browser.
Upload a CSV file or use the default student dataset.
Enter your natural language question and click Retrieve.
The app will display the generated SQL query and the query results.
Contributing
Feel free to open issues or submit pull requests if you have suggestions or improvements. Please follow the contribution guidelines for details.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments
Thanks to Google Cloud for providing the Generative AI API.
Streamlit for making it easy to build and share interactive applications.
