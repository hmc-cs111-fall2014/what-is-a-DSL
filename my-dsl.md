# Language

For this assignment I'm looking at the Hive Query Language (HQL), which is described in detail [here](https://cwiki.apache.org/confluence/display/Hive/LanguageManual).

HQL the interface to the [Hive](https://en.wikipedia.org/wiki/Apache_Hive) pseudo-database. It allows for users to specify the storage of large amounts of data and do analysis on that data. It inherited its syntax and most of its semantics from SQL, with the exception of features added to support larger datasets.

# Domain
*Big Data Analysis* and Storage


# Computational model

An HQL query is executed in the following steps:
  1. The query is translated into one or more Hadoop MapReduce jobs.
  2. Those jobs are queued
  3. They are executed by a Hadoop cluster

For reference, MapReduce is a framework provided by Hadoop (A distributed filesystem ecosystem) which allows users to specify how a task they have can be executed in parallel during a mapping stage, and then in semi-serial as the results for the mapping stage are combined during the reducing stage.
This framework is used when dealing with large amounts of data because it allows for parallel computation on data that is too large to process quickly in serial, or is even too large to store on one computer.
Many DB queries can be executed in parallel across different parts of the tables they examine, and for that reason MapReduce is somewhat appropriate for DB-like interactions.

One item of note is that sequential jobs transfer information by writing it to the cluster's distributed filesystem (so the next job can read the data out of the file system and use it for its computation).

# DSL-ness

I would place HQL pretty far to the 'DSL' side of the spectrum for the following reasons:
  - Its syntax is very declarative, and only provides functionality for data analysis
  - It provides no looping constructs and very limited conditional constructs
  - It includes a number of features that cater directly to the needs of big data

# Internal or external?

It is an external DSL - it exists in its own files and is parsed, translated, and executed by an external execution engine.

# Host language

The HQL execution engine is written in Java. This is largely because HQL queries are ultimately executed as Hadoop MapReduce jobs, and Hadoop is dominantly Java (for better or worse).

The Hive repository (in which HQL lives) can be found [here](https://github.com/apache/hive).

# Benefits

Hive and the HQL were developped at Facebook to allow for the analysis of extremely large datasets.
Amazon and Netflix (among others) now use Hive/HQL for similar purposes.

Some benifits inclue:
  - The Hadoop backbone of Hive allows for this analysis to scale very well to large datasets
  - It's similarity to SQL allows it to be more easily used by data scientists who have familiarity with SQL


# Drawbacks

Problems include:
  - HQL queries usually have very high latency, as the system is entirely focussed on maximizing throughput/scalability
    - The reason for this hyper-focus on throughput is that Hive/HQL is ultimately designed to be scalable above all else. If you're going to crawl through huge amounts of data, even tiny increases in throughput are worth taking huge latency hits for
  - The execution engine is somewhat naive in a few regards
    - It always translates into sequential MapReduce jobs (Map -> Reduce -> Disk -> Map -> Reduce) even if a different flow wouuld be more optimal (Map -> Map -> Reduce)
    - It always uses the MapReduce framework, even if a more complex model of parallelism would be more optimal
  - While HQL is very similar to SQL, it differs in ways which are unclear to users. These differences range from syntatical to semantic differences, the semantic differences being most problematic
  - HQL also doesn't support features from SQL in some cases.
    - For example `SELECT * FROM my_table` generally doesn't work as partition column values must be specified in a WHERE clause.
    - Hive 'Partition Columns' are columns which the user has flagged as 'Partition' columns as a way of indicating that they will generally only analyze batched of data with the same value in this column. This allows for the data to be stored more optimally for that use pattern.
    - HQL then also prevents users from analyzing data across values in that column unless they explicitly say that want to in a WHERE clause by doing something like `WHERE part_column in ['val1', 'val2']`
