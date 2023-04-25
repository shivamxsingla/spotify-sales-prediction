# Spotify Sales Prediction using Apache Spark

![image](https://user-images.githubusercontent.com/95306965/234356265-d8cdaf43-a611-4af3-8950-621c3ab773dc.png)


## About Apache Spark
Apache Spark, written in Scala, is a general-purpose distributed data processing engine. Or in other words: load big data, do computations on it in a distributed way, and then store it.

Apache Spark contains libraries for data analysis, machine learning, graph analysis, and streaming live data. Spark is generally faster than Hadoop. This is because Hadoop writes intermediate results to disk (that is, lots of I/O operations) whereas Spark tries to keep intermediate results in memory (that is, in-memory computation) whenever possible. Moreover, Spark offers lazy evaluation of operations and optimizes them just before the final result; Sparks maintains a series of transformations that are to be performed without actually performing those operations unless we try to obtain the results. This way, Spark is able to find the best path looking at overall transformations required (for example, reducing two separate steps of adding number 5 and 20 to each element of the dataset into just a single step of adding 25 to each element of the dataset, or not actually doing operations on part of the dataset which will eventually will be filtered out in the final result).

This makes Spark one of the most popular tools for big data analytics currently.

PySpark is an interface for Apache Spark in Python. It not only allows you to write Spark applications using Python APIs, but also provides the PySpark shell for interactively analyzing your data in a distributed environment.

In this Notebook, we have the data of a music streaming website with the following fields: Definitions:

- Email ID of the user
- Address of the user
- Average Session Length of the user
- Time spent by the user on the app
- Time spent by the user on the website
- Length of the membership of the user
- Yearly amount spent by the user
<br>
We used Pyspark API of Apache Spark to handle this data to bring out meaningful inferences and try to predict the Amount spent by users using this data
