☁️ Automated Weather Data ETL Pipeline
An end-to-end ETL pipeline built with Apache Airflow that extracts weather data from the Open-Meteo API, transforms it into a structured format, and loads it into a PostgreSQL database for further analysis and reporting.

🌟 Overview
Monitoring weather conditions is crucial for various industries, including agriculture, transportation, and event planning. The Automated Weather Data ETL Pipeline provides an efficient and automated solution to:

Extract weather data from the Open-Meteo API for a specific location.
Transform raw weather data into a structured, analysis-ready format.
Load transformed data into a PostgreSQL database for storage and analysis.
The pipeline runs daily, ensuring that weather data is always up to date and readily available for reporting or integration into decision-making systems.

🚀 Features
Dynamic Weather Data Extraction: Fetches current weather data based on latitude and longitude.
Automated Data Transformation: Converts API response into a structured format for easy querying.
PostgreSQL Integration: Stores transformed data in a relational database.
Scalable Architecture: Built with Apache Airflow for scheduling and workflow orchestration.
Daily Pipeline Execution: Ensures data is updated regularly without manual intervention.
🏗️ Architecture
Workflow
Extract:
Fetches weather data from the Open-Meteo API using Airflow's HttpHook.
Transform:
Extracts relevant weather attributes like temperature, wind speed, and wind direction.
Adds metadata such as latitude, longitude, and a timestamp.
Load:
Inserts transformed data into a PostgreSQL database, creating tables dynamically if required.
📊 Performance Highlights
Automates data collection for London (latitude: 51.5074, longitude: -0.1278) but can be adapted to other locations.
Processes and stores weather data daily, providing a continuous stream of real-time insights.
Optimized data load with PostgreSQL transactions to ensure data integrity.
⚙️ Tech Stack
Workflow Orchestration: Apache Airflow
Database: PostgreSQL
API: Open-Meteo API
Programming Language: Python
🛠️ Installation
Prerequisites
Python 3.8+
Apache Airflow
PostgreSQL
📂 Project Structure
weather-data-etl/  
├── dags/                 # DAG scripts for Airflow  
│   └── weather_etl_pipeline.py  
├── requirements.txt      # Python dependencies  
├── README.md             # Project documentation  
└── utils/                # Helper functions (if applicable)  
🔮 Future Enhancements
Add support for multiple locations with dynamic parameterization.
Integrate with BI tools like Power BI or Tableau for visualization.
Include historical weather data for trend analysis.
Implement alerting mechanisms for pipeline failures.
🏁 Conclusion
The Automated Weather Data ETL Pipeline is a robust and scalable solution to automate the collection, transformation, and storage of weather data. With Apache Airflow's scheduling power and PostgreSQL's efficient storage, this project empowers users to derive valuable insights from weather data with minimal manual effort.

About
No description, website, or topics provided.
Resources
 Readme
 Activity
Stars
 0 stars
Watchers
 0 watching
Forks
 0 forks
Report repository
Releases
No releases published
Packages
No packages published
Languages
Python
99.7%
 
Dockerfile
0.3%
Footer
