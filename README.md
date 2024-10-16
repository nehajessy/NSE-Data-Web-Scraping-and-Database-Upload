
# NSE Data Web Scraping and Database Upload

## Overview

This project demonstrates how to scrape historical equity data from the National Stock Exchange (NSE) of India and upload it into a MySQL database using Python. The code leverages various libraries to perform web scraping, data manipulation, and database interactions.

## Components

1. **Web Scraping**: 
   - **Requests**: Used to send HTTP requests to the NSE API to retrieve historical equity data.
   - **Pandas**: Employed to process and manipulate the data returned from the API.
   - **Data Cleaning**: Includes data type conversion and cleaning operations to prepare the data for database insertion.

2. **Database Interaction**:
   - **SQLAlchemy**: Used to create a connection to a MySQL database and manage data insertion.
   - **MySQL**: The target database where the cleaned data is uploaded.

## Installation

To set up the environment for this project, you need to install the following Python libraries:

```sh
pip install requests pandas sqlalchemy pymysql cryptography
```

## Usage

1. **Data Retrieval**: The code sends a GET request to the NSE API endpoint to retrieve historical equity data for a specified symbol (e.g., TCS).

2. **Data Processing**:
   - The data is loaded into a Pandas DataFrame.
   - Columns are normalized and cleaned.
   - Date columns are converted to `datetime` format.
   - Numeric values are cleaned of any extraneous characters.

3. **Database Upload**:
   - A MySQL database connection is established using SQLAlchemy.
   - The cleaned DataFrame is uploaded to the specified table in the database.

## Conclusion

This project demonstrates how to integrate web scraping with data processing and database management. The approach can be adapted for various types of data sources and databases. The methodology showcases how to handle real-time data extraction and storage efficiently.

