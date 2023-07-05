# YouTube Data Harvesting and Warehousing using SQL, MongoDB, and Streamlit

**Introduction**

YouTube Data Harvesting and Warehousing is a project aimed at developing a user-friendly Streamlit application that leverages the power of the Google API to extract valuable information from YouTube channels. The extracted data is then stored in a MongoDB database, subsequently migrated to a SQL data warehouse, and made accessible for analysis and exploration within the Streamlit app.

**Table of Contents**

1. Installation
2. Usage
3. Features
4. Retrieving data from the YouTube API
5. Storing data in MongoDB
6. Migrating data to a SQL data warehouse
7. Data Analysis
8. Contributing
9. License
10. Contact

**Installation**

To run this project, you need to install the following packages:
```python
pip install googleapiclient.discovery
pip install pymongo
pip install pandas as pd
pip install psycopg2
pip install datetime
pip install streamlit as st
pip install plotly.express as px
```

**Usage**

To use this project, follow these steps:

1. Clone the repository: ```git clone https://github.com/gopiashokan/Youtube-Harvesting-and-Warehousing.git```
2. Install the required packages: ```pip install -r requirements.txt```
3. Run the Streamlit app: ```streamlit run app.py```
4. Access the app in your browser at ```http://localhost:8501```

**Features**

1. Retrieve data from the YouTube API, including channel information, playlists, videos, and comments.
2. Store the retrieved data in a MongoDB database.
3. Migrate the data to a SQL data warehouse.
4. Analyze and visualize data using Streamlit and Plotly.
5. Perform queries on the SQL data warehouse.
6. Gain insights into channel performance, video metrics, and more.

**Retrieving data from the YouTube API**

The project utilizes the Google API to retrieve comprehensive data from YouTube channels. The data includes information on channels, playlists, videos, and comments. By interacting with the Google API, we collect the data and merge it into a JSON file.

**Storing data in MongoDB**

The retrieved data is automatically stored in a temporary MongoDB database. Once stored, the data is transferred to the main database. If data already exists, it can be overwritten with user confirmation. This storage process ensures efficient data management and preservation.

**Migrating data to a SQL data warehouse**

The application allows users to migrate data from MongoDB to a SQL data warehouse. Users can choose which channel's data to migrate. To ensure compatibility with a structured format, the data is cleansed using the powerful pandas library. Following data cleaning, the information is segregated into separate tables, including channels, playlists, videos, and comments, utilizing SQL queries.

**Data Analysis**

The project provides comprehensive data analysis capabilities using Plotly and Streamlit. With the integrated Plotly library, users can create interactive and visually appealing charts and graphs to gain insights from the collected data.

**Channel Analysis:** Channel analysis includes insights on playlists, videos, subscribers, views, likes, comments, and durations. Gain a deep understanding of the channel's performance and audience engagement through detailed visualizations and summaries.

**Video Analysis:** Video analysis focuses on views, likes, comments, and durations, enabling both an overall channel and specific channel perspectives. Leverage visual representations and metrics to extract valuable insights from individual videos.

Utilizing the power of Plotly, users can create various types of charts, including line charts, bar charts, scatter plots, pie charts, and more. These visualizations enhance the understanding of the data and make it easier to identify patterns, trends, and correlations.

The Streamlit app provides an intuitive interface to interact with the charts and explore the data visually. Users can customize the visualizations, filter data, and zoom in or out to focus on specific aspects of the analysis.

With the combined capabilities of Plotly and Streamlit, the Data Analysis section empowers users to uncover valuable insights and make data-driven decisions.

**Contributing**

Contributions to this project are welcome! If you encounter any issues or have suggestions for improvements, please feel free to submit a pull request.

**License**

This project is licensed under the MIT License. Please review the LICENSE file for more details.

**Contact**

For any further questions or inquiries, please contact us at gopiashokankiot@gmail.com. We are happy to assist you.