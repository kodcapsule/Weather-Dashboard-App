# WEATHER DASHBOARD APP

Day 1 of the 30 days of DevOps challenge . 

## Weather Data Collection

This is a Weather data collection application that collects weather data from OpenWeather for various cites and stores the data in an S3 bucket

## Project Details
This project uses the following services 
- OpenWeather API: An external API that has weather details of all cities in the world
- Amazon S3: This is a cloud storage that stores the collected Weather data
- Python: Python programming language is uthe language used to handle the logic behind this application 

### Project Requirements 
 * Prerequisites

Before starting this  project, make sure you have the following:

    1. An **AWS Account**: Create an AWS account if you haven't done so already.
    2. A **GitHub Account**: You will need a GitHub account to store your project code and track changes.
    3 An **IDE** (preferably Visual Studio Code): Use Visual Studio Code (VSCode) for easier development, or any IDE of your choice.
    4 An **OpenWeather API Key**: Register on OpenWeather to get your API key.
    5. A **Python virtual environment**: It’s highly recommended to use a virtual environment to isolate your dependencies.





### Steps to Set Up and Run the Application

* How to run the program
1. Set Up Virtual Environment: Open your terminal or command prompt and create a new Python virtual environment.

 ```
     python3 -m venv venv
```
 Then, activate the virtual environment:
 * For Windows:
 ```
     .\venv\Scripts\activate
```
* For macOS/Linux:
```
    source venv/bin/activate
```
2. Install Dependencies:
With the virtual environment activated, install the required Python packages listed in the requirements.txt file.

```
    python3 pip install -r requirements.txt
```

Note: If you don’t have a requirements.txt, you can create it with all the libraries

You can check if the packages have been installed correctly by running:

```
   pip freeze
```

Note Make sure all the neccessory python packages are install. you can check the packages install using this command.

pip freeze


3. Set Up AWS and S3 Bucket:

Before running the pyhton script , make sure that:

    * You have configured AWS CLI or the AWS SDK (boto3) on your system with the appropriate AWS credentials.
    * You have an S3 bucket created in your AWS account, or the script will create one automatically. Ensure the bucket name is unique and adjust the configuration in the script accordingly.

4. Run the Application:

Once everything is set up, run the app with the below command:

```
   python3  src/weather-dashboard.py
```
This script will fetch weather data using the OpenWeather API and store it in your S3 bucket.

Ensure your OpenWeather API key is properly set in your code or as an environment variable, and the application will use that key to collect weather data for various cities.




### Troubleshooting
    - Missing Dependencies: Ensure all necessary libraries (such as requests, boto3, python-dotenv) are installed in your virtual environment.
    - API Key Issues: Double-check that your OpenWeather API key is valid and properly configured.
    - AWS Permissions: Ensure your AWS credentials you are using have the necessary permissions for S3 operations (like s3:PutObject).

By following these instructions, you should be able to successfully execute your weather dashboard application that collects and stores weather data in an S3 bucket!