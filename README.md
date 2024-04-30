# User Data Collection and Analysis with Flask, MongoDB, and Data Visualization

This project is aimed at creating a simple web application using Flask to collect user data, store it in MongoDB, process the data using Python, and visualize it using data visualization techniques.

## Project Overview

The project consists of the following components:

1. **Web Development with Flask**: The web application is created using Flask, a lightweight WSGI web application framework. Users can input their data through a simple webpage.

2. **Data Storage with MongoDB**: Initially, user details, including age, gender, total income, and expenses, were intended to be stored in MongoDB, a NoSQL database. However, due to cost constraints, MongoDB was utilized only locally for development and testing purposes.

3. **Data Processing with Python**: User data is processed using Python. A class named "User" is created to handle the data. The collected data is then stored in a CSV file for further analysis.

4. **Data Visualization**: Data is visualized using Jupyter Notebook. Various visualizations are performed, including showcasing the ages with the highest income and the gender distribution across spending categories. The charts generated are exported for use in presentations.

5. **Deployment on AWS**: The Flask application is hosted on Amazon Web Services (AWS) to make it accessible over the internet.

## File Structure

- `application.py`: Contains the Flask application code for collecting user data and storing it in MongoDB.
- `index.html`: HTML file containing the form for collecting user data.
- `mongo_db_to_csv.py`: Python script to retrieve user data from MongoDB and write it to a CSV file.
- `user.py`: Python file defining the `User` class to represent user data.

## Usage

1. Ensure that MongoDB is running on your local machine.
2. Run the Flask application by executing `python application.py`.
3. Access the web application through the provided URL ([http://usercollectiondata-env.eba-zwtmdbkv.eu-north-1.elasticbeanstalk.com/](http://usercollectiondata-env.eba-zwtmdbkv.eu-north-1.elasticbeanstalk.com/)) and input user data.
4. Once user data is collected, run the `mongo_db_to_csv.py` script using `python mongo_db_to_csv.py`.
5. The script will retrieve data from MongoDB and write it to a CSV file named `user_data.csv` in the same directory.

## Technologies Used

- Flask
- MongoDB
- Python (for data processing and visualization)
- Jupyter Notebook
- Amazon Web Services (AWS)
