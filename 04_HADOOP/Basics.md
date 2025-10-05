## LITTLE HISTORY

- In 2000s, there was a BIG problem of data not able to store in the traditional databases.
- To overcome this, **Google created 2 services**
    1. **Google File System (GFS)  =**  Storage Unit
    2. **Google Map Reduce (GMR) ==** Processing Unit.

## HADOOP

- The open source implementation of both the services were named as **"Hadoop"** ==> Doug Cutting and Mike Cafarella
- Hadoop is an open source framework designed to handle massive amount of data in a DISTRIBUTED & SCALABLE way and it solves -
    1. Massive Storage Problem.
    2. Slow Processing 

## PROPERTIES of Hadoop

1. **Scalability -** It can scale horizontally, i.e. we can add as many computers we want.
2. **Fault Tolerance -** Replicas are maintained to avoid failures if any single node fails.
3. **Distributed Processing -** Hadoop can process the data where it is stored.
4. **Cost Effectiveness -** Inexpensive hardware can too do the job.
5. **Open source -** Free to use and modify.

## ECOSYSTEM of 🐘

> Core components

1. **HDFS**

2. **MAP REDUCE**

3. **YARN (Yet Another Negotiator)**

> Add ons' components

4. **HIVE -** It's a query engine, not a Db. It **abstracts MR** in backend by **translating SQL queries** into MR Jobs (which are written in Java)

5. **PIG -** Created by Yahoo, **abstracted MR** converting PigLatin (high level scripting language) into MR jobs for performance.

6. **SQOOP -** Standalone component that **facilates IMPORT/EXPORT** between Hadoop and RDBMS.