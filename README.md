This project is part of a university assignment where we analyze real-world ship position data from the port of Piraeus and the Saronic Gulf, collected via the Automatic Identification System (AIS). The dataset includes information transmitted by ships and consists of three CSV files:

    Positions.csv: Contains ship position data (longitude, latitude, speed, etc.) for the period 01/08/2019 to 30/08/2019.
    Vessels.csv: Provides static information about the ships, such as their type and flag.
    VesselTypes.csv: Includes a short description of the various ship types.

Objectives

The goal of this project is to answer a series of queries using PostgreSQL, focusing on optimizing query performance. Some of the key tasks include:

    Data Analysis: Analyzing the ship position data to answer questions such as:
        The number of ship position entries per day.
        The number of ships of a particular type with the Greek flag.
        Identifying ships that exceeded 30 knots and their type.
        The number of passenger ship positions recorded over specific dates.
        Identifying cargo ships anchored at certain times.

    Performance Optimization: Improving the performance of these queries by:
        Adjusting PostgreSQL settings, such as increasing memory buffers and utilizing CPU parallelism.
        Creating appropriate indexes to enhance query execution speed.
        Partitioning the dataset into shards for more efficient query execution.

Queries and Performance Monitoring

For each query, the execution time is monitored and recorded after multiple runs to observe performance improvements. PostgreSQL’s EXPLAIN command is used to analyze the query execution plan and explain the performance changes.
