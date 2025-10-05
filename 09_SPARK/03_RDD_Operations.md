# Spark RDD Operations: Customer Data Processing

This document outlines a basic workflow for processing customer data using Apache Spark's RDD (Resilient Distributed Dataset) API. The steps include initializing the RDD, extracting the header, and filtering the data.

---

## 1: Creating the RDDs - parallelize()

We begin by creating an empty list to hold customer data and parallelizing it into an RDD using Spark's context.

```python
customer_data = [
    "CustomerID,Name,Age,Country",
    "1,Alice,34,USA",
    "2,Bob,45,Canada",
    "3,Charlie,29,USA",
    "4,Diana,40,UK",
    "5,Evan,23,India"
]

# Convert the list into an RDD
data_rdd = spark.sparkContext.parallelize(customer_data)
```

## 2: first() and filter() Operation

We separate the header from the data to avoid processing it in transformations.

```python
# Extract header
header = data_rdd.first()

# Filter out the header
data_rdd_no_header = data_rdd.filter(lambda row: row != header)
```



