# CouchDB

* NoSQL
* Impl in Erlang
  * seen lots of use telecomm (Erlang)
  * fault tolerant
* RESTful


## Document Model

* Document data: self-contained data
* CouchDB stores documents
* Each doc has everything that might be needed by an application that makes use of it
* No schema is enforced
  * Allow for natural modeling of domains
  * attributes can contian docs

## CAP Theorem
When dealing with distributed systems have to consider some issues.

Issues:
* Consistency: All clients see the same data even in the presence of concurrent updates
* Availability: All clients are able to read or write the data store when they want to
* Partition Tolerance: A database can be split acreoss multiple servers

CAP Theorem says: PICK ANY TWO

Characteristics:
1. Consistent and Available: What relational database provide
2. Availablility and Partition Tolerant: Provide scale, but not necessarily gives the same answer to everyone
3. Consistency and Partition Tolerance: Able to provide consistent and be across multiple database, but not always available

CouchDB choose 2

## Where magic happens

* Uses a B-tree as storage engine
* Employ MapReduce
* No Locking
  * always give back most recent as of start of read
* Validation: test for a valid doc before it writes
* Incremental Replication
  * you can choose to synchronize data
  * once replicated each copy independent (like git)
