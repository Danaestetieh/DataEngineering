# DataEngineering
# Q1: build a flow to extract CSV file and convert it to json file then load it to mongoDB database


## Use docker compose to run the following images: 
mongodb: to load the data
Apache Nifi: to build the flow
Postgres: to load the data but I used mongodb

- Save CSV file called data2 in the container and I renamed it to “data” which contains random data (faker library was used)

- to run the container use docker-compose up command.

- Use http://localhost:8080 to run Apche NiFi


## 4 processors have been used as following:
```
1- Get CSV File: extract CSV file called data.
2- Add Schema Name Attribute: build the schema to enable read the file
3- ConvertRecord - CSVtoJSON: convert CSV file  to JSON
4- PutMongoRecord: build the schema to enable read the file
```

## MongoDB Compass was used it to visualize and understand the content of the data database

