# Project description
This capstone project is to give a chance to combine what I've learned throughout this programme. The project is to create the ETL pipeline to create a database for useful insights and analysis.For example, UK immigration age distribtuion. 

# Data sources
In this project, I am using the datasets that are provided by Udacity. 

1. I94 Immigration Data: This data comes from the US National Tourism and Trade Office. A data dictionary is included in the workspace. This is where the data comes from. There's a sample file so you can take a look at the data in csv format before reading it all in. You do not have to use the entire dataset, just use what you need to accomplish the goal you set at the beginning of the project.

2. World temperature Data: This dataset comes from Kaggle Source. Includes temperature recordings of cities around the world for a period of time.

# Describe and Gather Data
The I94 immigration data comes from the US National Tourism and Trade Office. It is provided in SAS7BDAT format which is a binary database storage format. Some relevant attributes include:

* i94yr = 4 digit year
* i94mon = numeric month
* i94cit = 3 digit code of origin city
* i94port = 3 character code of destination USA city
* arrdate = arrival date in the USA
* i94mode = 1 digit travel code
* depdate = departure date from the USA
* i94visa = reason for immigration

The temperature data comes from Kaggle. It is provided in csv format. Some relevant attributes include:

* AverageTemperature = average temperature
* City = city name
* Country = country name
* Latitude= latitude
* Longitude = longitude

# Projet Steps
To help guide reading this project, I've broken it down into a series of steps.

## Step 1: Scope the Project and Gather Data
Since the scope of the project will be highly dependent on the data, these two things happen simultaneously. In this step, you’ll:

* Identify and gather the data you'll be using for your project (at least two sources and more than 1 million rows). See Project Resources for ideas of what data you can use.
* Explain what end use cases you'd like to prepare the data for (e.g., analytics table, app back-end, source-of-truth database, etc.)

## Step 2: Explore and Assess the Data
* Explore the data to identify data quality issues, like missing values, duplicate data, etc.
* Document steps necessary to clean the data

## Step 3: Define the Data Model
* Map out the conceptual data model and explain why you chose that model
* List the steps necessary to pipeline the data into the chosen data model

## Step 4: Run ETL to Model the Data
* Create the data pipelines and the data model
* Include a data dictionary
* Run data quality checks to ensure the pipeline ran as expected
- Integrity constraints on the relational database (e.g., unique key, data type, etc.)
- Unit tests for the scripts to ensure they are doing the right thing
- Source/count checks to ensure completeness

## Step 5: Complete Project Write Up
* What's the goal? What queries will you want to run? How would Spark or Airflow be incorporated? Why did you choose the model you chose?
* Clearly state the rationale for the choice of tools and technologies for the project.
* Document the steps of the process.
* Propose how often the data should be updated and why.
* Post your write-up and final data model in a GitHub repo.
* Include a description of how you would approach the problem differently under the following scenarios:
- If the data was increased by 100x.
- If the pipelines were run on a daily basis by 7am.
- If the database needed to be accessed by 100+ people.