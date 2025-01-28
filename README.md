# HOMEWORK-DATACAMP-25

Docker & SQL
In this homework we'll prepare the environment and practice with Docker and SQL

## Question 1. Knowing docker tags
Run the command to get information on Docker

docker --help

Now run the command to get help on the "docker build" command:

docker build --help

Do the same for "docker run".

Which tag has the following text? - Automatically remove the container when it exits

--delete
--rc
--rmc
--rm
![image](https://github.com/user-attachments/assets/0cf08a22-555b-4d3a-b2e9-ce10dbc226d7)



## Question 2. Understanding docker first run
Run docker with the python:3.9 image in an interactive mode and the entrypoint of bash. Now check the python modules that are installed ( use pip list ).

What is version of the package wheel ?

0.42.0
1.0.0
23.0.1
58.1.0
Prepare Postgres
Run Postgres and load data as shown in the videos We'll use the green taxi trips from September 2019:

wget https://github.com/DataTalksClub/nyc-tlc-data/releases/download/green/green_tripdata_2019-09.csv.gz

You will also need the dataset with zones:

wget https://s3.amazonaws.com/nyc-tlc/misc/taxi+_zone_lookup.csv

Download this data and put it into Postgres (with jupyter notebooks or with a pipeline)




## Question 3. Count records
How many taxi trips were totally made on September 18th 2019?

Tip: started and finished on 2019-09-18.

Remember that lpep_pickup_datetime and lpep_dropoff_datetime columns are in the format timestamp (date and hour+min+sec) and not in date.

15767
15612
15859
89009

![image](https://github.com/user-attachments/assets/5869c13e-44ab-4045-8b5e-0ab8560cebb6)


## Question 4. Longest trip for each day
Which was the pick up day with the longest trip distance? Use the pick up time for your calculations.

Tip: For every trip on a single day, we only care about the trip with the longest distance.

2019-09-18
2019-09-16
2019-09-26
2019-09-21
![image](https://github.com/user-attachments/assets/084a78bc-676f-4a2c-ac36-cacab7815032)



## Question 5. Three biggest pick up Boroughs
Consider lpep_pickup_datetime in '2019-09-18' and ignoring Borough has Unknown

Which were the 3 pick up Boroughs that had a sum of total_amount superior to 50000?

"Brooklyn" "Manhattan" "Queens"
"Bronx" "Brooklyn" "Manhattan"
"Bronx" "Manhattan" "Queens"
"Brooklyn" "Queens" "Staten Island"
![image](https://github.com/user-attachments/assets/a50969ed-5d8c-422b-9cf3-41d5bf8c99ed)


## Question 6. Largest tip
For the passengers picked up in September 2019 in the zone name Astoria which was the drop off zone that had the largest tip? We want the name of the zone, not the id.

Note: it's not a typo, it's tip , not trip

Central Park
Jamaica
JFK Airport
Long Island City/Queens Plaza

![image](https://github.com/user-attachments/assets/39b466bd-a048-4d4d-a614-6e9e93c2eca7)





