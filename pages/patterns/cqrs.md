---
title: Cloud Pattern Repository
tags: [architecture]
keywords:
summary: "Cloud Patterns: Data Management: CQRS"
sidebar: mydoc_sidebar
permalink: cqrs.html
folder: patterns
---

## The CQRS Pattern

Most users tend to adopt a CRUD approach when interacting with a database.

CRUD is: Create, Read, Update, Delete records.

However, interactions tend to become more complex. The user might require
a view of the data in a manner that differs from the structure in the store.
One might require collapsing multiple records into one.

The CQRS pattern attempts to address this issues.

## Motivation 

* One might want to update additional columns in the database, although those columns are not required as part of the operation.
* Read and write operations can have different performance requirements, being asymmetrical.
* As needs become more complicated, data might be read in one way, say by combining tables, for example. However, writing might not use the same representation.
Also, there may be validation rules that only allow certain combinations of data to be stored.

## Structure

The CQRS pattern aims to solve this problem.

The pattern simply allows for separate update and display object models, called the Command and Query.

### Commands

* Commands are task-based and not data centric.
* Commands can be processed asynchronously.

### Queries

* Queries never modify the database.
* A query simply returns a Data Transfer Object (DTO)

## Advantages

* CQRS fits well with event-based models.
* This is suited to complex domains.
* Scaling, optimization and architectural changes are easier to manage.
* A greater degree of predictability is afforded.
* The logic is cohesive and less interrelated.

## Disadvantages

* Troubleshooting is difficult due to multiple code paths.
* Some developers recommend using multiple databases - some for read and some for write. The overhead due to multiple databases can be huge.
* With multiple databases, the data can become stale.
* This can be incompatible with legacy systems.

## References
[1] https://docs.aws.amazon.com/whitepapers/latest/database-caching-strategies-using-redis/caching-patterns.html

[2] https://learn.microsoft.com/en-us/azure/architecture/patterns/cache-aside

[3] https://martinfowler.com/bliki/CQRS.html

[4] https://www.eventstore.com/cqrs-pattern