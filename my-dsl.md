# Language

For this assignment I'm looking at the Hive Query Language (HQL), which is described in detail [here](https://cwiki.apache.org/confluence/display/Hive/LanguageManual).

HQL the interface to the [Hive](https://en.wikipedia.org/wiki/Apache_Hive) pseudo-database. It allows for users to specify the storage of large amounts of data and do analysis on that data. It inherited its syntax and most of its semantics from SQL, with the exception of features added to support larger datasets.

# Domain
*Big Data Analysis* and Storage


# Computational model

An HQL query is executed in the following steps:
  1. The query is translated into one or more Hadoop MapReduce.
  2. Those jobs are queued
  3. They are executed by a Hadoop cluster

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

# Benefits

Hive and the HQL were developped at Facebook to allow for the analysis of extremely large datasets.
Amazon and Netflix (among others) now use Hive/HQL for similar purposes.

Some benifits inclue:
  - The Hadoop backbone of Hive allows for this analysis to scale very well to large datasets
  - It's similarity to SQL allows it to be more easily used by data scientists who have familiarity with SQL


# Drawbacks

Problems include:
  - HQL queries usually have very high latency, as the system is entirely focussed on maximizing throughput
  - The execution engine is somewhat naive in a few regards
    - It always translates into sequential MapReduce jobs (Map -> Reduce -> Map -> Reduce) even if a different flow wouuld be more optimal (Map -> Reduce -> Reduce)
    - It always uses the MapReduce framework, even if a more complex model of parallelism would be more optimal
  - While HQL is very similar to SQL, it differs in ways which are unclear to users. These differences range from syntatical to semantic differences, the semantic differences being most problematic
