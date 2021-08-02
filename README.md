# ETL Operations and Data Pipelines
__Extract, Transform, Load__ (__ETL__) is the general procedure of copying data from one or more sources into a destination system which represents the data differently from the source or in a different context than the source.
# Modern Data Integration Complexieties
* No System of record
* Synchronization is hard
* Scaling ETL is hard
* Processing is error-prone
# Apache Kafka
__Apache Kafka__ is a __Distributed Stream Processing System__ developed by __LinkedIn__ and written in __Scala__ and __Java__, now open source project maintained by __Confluent__.
## Why Apache Kafka?
* Distributed, resilient architecture, fault tolerant
* Horizontal scalability:
    - can scale 100s of brokers
    - can scale to millions of messages per second
* High performance (latency of less than 10ms) - real time
* used by the 200+ firms, 35% of the Fortune 500 
## Kafka Fundamentals
* Messaging system semantics
* Clustering is core
* Durability and Ordering guaranteed
## Use cases for Apache Kafka
* Messaging system
* Activity Tracking
* Gather metrics from many different locations
* Application Logs gathering
* Stream processing (with the Kafka Streams API or Spark for example)
* De-coupling of system dependencies
* Integration with Spark, Flink, Storm, Hadoop and many other Big Data technologies (i.e., Big Data Ingest)
* Modern ETL/CDC
* Data Pipelines

## Use Cases - Examples
* __Netflix__ uses __Kafka__ to apply recommendations in real-time while watching a TV Show
* __Uber__ uses __Kafka__ to gather user, taxi and trip data real time to compute and forecast demand, and compute surge pricing pricing in real-time.
__LinkedIn__ uses __Kafka__ to prevent spam, collect user interactions to make better connection recommendations in real time.

# Characteristics of Records in Kafka
* Key, Value, Timestamp
* Immutable 
* Append only
* Persisted

# Features of Kafka
* Log compaction
* Disk not Heap for efficiency
* Pagecache to Socket
* Balanced Partitions and Leaders
* Producer and Consumer Quotas
* Heroku Kafka

# References
1. [Tutorial 1](https://www.youtube.com/watch?v=UEg40Te8pnE)
2. [Definitive Guide to Kafka](https://www.confluent.io/resources/kafka-the-definitive-guide-v2/?utm_source=Drift&utm_medium=Digital&utm_campaign=General)
3. [The Quick and Dirty Guide to Building Your Data Platform](https://towardsdatascience.com/the-quick-and-dirty-guide-to-building-your-data-platform-2f21dc4b7c94)