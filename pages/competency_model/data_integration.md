---
title: "Data Integration"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: data_integration.html
folder: competency_model
summary: "Most companies use a mixture of in-house developed systems, 3rd party “off the shelf” and cloud hosted systems."
tags:
  - information_architecture
---

# Description

Data integration involves combining data from disparate sources so that business users and downstream systems can utilize the data in a unified way. This may sound simple but in reality data integration architecture is a broad and complicated discipline, one which requires a solid understanding of several areas including the business domain, the data models involved and the various data integration technologies and products which are available.

# Overview

Integration Architecture is a specialization with many dedicated integration architects however all IT architects should have a good understanding of the basic design principles involved in data integration.

Most companies use a mixture of in-house developed systems, 3rd party “off the shelf” and cloud hosted systems. In order to get the most value from the data within these systems it must be consolidated in some way. For example, the data within a cloud hosted system could be combined with the data in an in-house system to deliver a new product or service. Another example is where the data in a legacy system is combined with the data in a newer system to facilitate analysis and to deliver insights which were previously unattainable. Mergers and acquisitions are also big drivers of data integration, data from multiple systems must be consolidated so that the various companies involved in the merger can work together effectively.

Depending on the data integration requirements, the data must first be extracted from the various sources, then it is generally filtered, aggregated, summarized or transformed in some way and finally delivered to the destination user or system.

As an architect it is inevitable that you will become involved in many data integration projects throughout your career. Data integration is also becoming more complex as the IT landscape is ever expanding to include in-house systems, cloud hosted systems, 3rd party services and big data.

Data integration is closely related to system integration which deals more specifically with services and API’s.

For any data integration project you will need a good understanding of:

*   the data models within each data source
*   the mappings between the source and destination data models
*   any data contracts mandated by the destination system
*   the data transformations required

Functional requirements generally include:

*   data transformation
*   delivering a defined level of data quality
*   capturing a history of changes
*   monitoring changes

Non-functional requirements for consideration include the following:

*   system performance
*   the load on both source and destination systems
*   data volumes and the network latency affecting data transfer
*   timeliness of data updates
*   event based notifications (real-time)
*   job schedules (near real-time or batch)
*   security
*   data transport methods and protocols

Categories of Data Integration:

*   Operational Data Integration – integration of data across operational applications and databases.
*   Analytic Data Integration – integration in the context of business intelligence or data warehousing.

Scope of Data Integration:

*   Data Migration, a once off exercise
*   from a legacy system to a new system.
*   when companies merge and need to consolidate data.
*   Data Synchronization, continuous data integration
*   continuously maintaining data consistency between two or more systems.
*   may be between applications within the same company, often referred to as “Application to Application” or “A2A” integration or integrating with external parties, also known as Business to “Business” or “B2B” integration.

# Proven Practices

*   Data integration projects generally take longer than expected due to unforeseen complexities, plan carefully and try not to underestimate the effort involved.
*   Get a clear understanding of the data mapping requirements as early as possible in a project.
*   Data integration projects are often prerequisites for larger projects, ensure that all stakeholders are kept up to date on progress as any delays will have knock on affects.
*   Usage of application integration patterns such as those defined by EAI generally result in better architecture.

# Sub-Capabilities

## Data Mapping & Transformation

One of the most important parts of any data integration project is the data mapping exercise. The source and destination data stores will usually have different data models, a data mapping defines how the source data elements map to the destination data elements.

A clear understanding of the business requirements is essential if all stakeholder expectations are to be met. The data mapping exercise is usually carried out near the beginning of a project and it is important to identify any gaps at this early stage as they will have an impact on downstream decisions and processes.

While analyzing the data models you should identify:

*   the direct one-to-one mappings.
*   the primary, alternate or composite keys, i.e. keys used to uniquely identify records in both source and destination systems.
*   the elements which need to be transformed, i.e. unit conversions, lowercase to uppercase or other formatting.
*   any gaps where a required element in the destination has no equivalent element in the source.
*   any bad data which should be excluded, i.e. orphaned records.

Other things to watch out for:

*   duplicate records.
*   non unique keys.
*   null values.
*   loss of numeric precision, i.e. when transforming floating point numbers.
*   differences in character encoding.
*   trailing spaces, i.e. when transforming fixed length strings to a variable length type.
*   **Iasa Certification Level** **Learning Objective** **CITA- Foundation** Learner will be able to discuss the process of data mapping.
*   **CITA – Associate** Learner will be able to complete a data mapping exercise.
*   Learner will be able to identify gaps between source and destination data models.
*   **CITA – Specialist** Learner will be able to validate the output of a data mapping exercise.
*   Learner will be able to identify problems areas such as differences in character encoding and design an appropriate transformation.
*   **CITA – Professional** Learner will be able to mentor others is data mapping.
*   Learner will be able to review the output of a data mapping exercise, highlighting any problem areas.

## Extract, Transform and Load (ETL) Design

The ETL process involves the extraction of data from a source data store or stores, transforming the data into the desired data model and finally loading the data into the destination data store.

*   The Extract process involves extracting the source data into a staging data store which is usually a separate schema within the destination database or a separate staging database.
*   The Transform process generally involves re-modelling the data, normalizing is structure, unit conversion, formatting and the resolution of primary keys.
*   The Load process is quite simple in the case of a once off data migration but can be quite complex in the case of continuous data integration where the data must be merged (inserts, updates & deletes), possibly over a defined date range, there may also be a requirement to maintain a history of changes.

A variation on the ETL process is the ELT process where the data is loaded into the destination store before transformation occurs.

**Types of ETL Data Integration**

In order to fully integrate two databases there are three main types of data integration which need to be in place; reference / master data, bulk load and incremental integration.

**Master & Reference Data Integration**

Assuming that referential integrity has been implemented appropriately, the destination database must be primed with master data before any operational data can be imported. For a new implementation, the first integration job to be run will load the master data, this generally includes various codes and types such as cities, countries and time zones etc. This data is often governed by a Master Data Management (MDM) process.

**Bulk Data Integration**

Once the master data has been loaded successfully; a bulk load of the operational data can be loaded either by querying the source database directly or by importing a data extract from the source database.

**Incremental Data Integration**

Incremental integration or data synchronization can be any one of the following methods depending on what is available from the source system:

*   Running the bulk load integration at more frequent intervals for a narrow time range i.e. extract plus / minus one day’s data on an hourly schedule, analyzing the extracted data and merging any changes found.
*   Querying the source database at frequent intervals for changes based on a last updated time-stamp or transaction identifier, also referred to as Delta Detection.
*   Update Notification from the source system, indicating that a change has occurred and what has changed, also referred to as Event Driven.

Update Notification is the preferred method (if available) when near real time performance is required however there is generally a need to run the bulk load job on occasion (on an off-peak schedule) to ensure that the data is fully synchronized. There are always cases where notifications cannot be processed, are received in the wrong order or are lost for some reason so running the bulk load integration brings the data back in sync.

## Other ETL Design Considerations

**Merging Data**

In order to successfully merge data during the load process there must be a common key which identifies records in both the source and destination, this may be a composite key (concatenation of two or more data elements) and it must be unique.

**Maintaining a History of Changes**

A history of changes can be maintained at a record level or at a data element level, it can also include details of who made the changes, when they were made and why.

Maintaining a history at a record level can result in a high level of data duplication if the data has a denormalized structure. Maintaining a history at an element level can result in a large amount of records if several elements are usually modified as part of a single transaction. Choose your approach carefully as using the wrong method can cause your data store to grow substantially over time.

**Soft versus Hard Deletes**

A hard delete is when a record is removed so that it cannot be retrieved again, a soft delete sets a flag or a time-stamp on a record to indicate that the record is virtually deleted and should no longer be used by the system for operational purposes, it is kept for historical or audit purposes.

**Testing**

The output of an ETL must be tested to ensure the data fulfills all of the business requirements and is of acceptable quality.

**Monitoring & Alerting**

ETL jobs are usually run on a schedule and they will fail from time to time, unusual data, network issues, server reboots all happen at unexpected times. It is important to have sufficient monitoring and alerting in place to ensure that system can be returned to a stable state in a timely manner.

*   **Iasa Certification Level** **Learning Objective** **CITA- Foundation** Learner will be able to explain the ETL process.
*   Learner will be able to describe the different types of ETL data integration.
*   **CITA – Associate** Learner will be able to design an ETL to meet customer requirements.
*   Learner will be able to examine the destination data to verify that it meets the customers requirements.
*   **CITA – Specialist** Learner will be able to design an ETL with advanced features such a maintaining a history of changes.
*   Learner will be able to performance tune an ETL.
*   **CITA – Professional** Learner will be able to scope and plan an ETL project.
*   Learner will be able to mentor others in ETL design.

## Enterprise Application Integration Design

While the ETL process is about consolidating data from many sources into one, Enterprise Application Integration, or EAI, is about distributing data between two or more systems. Data exchanged using EAI is often transactional and related to an event in a business process or the distribution of master data. EAI includes message broker and [enterprise service bus (ESB)](https://en.wikipedia.org/wiki/Enterprise_service_bus){:target="_blank"} technologies.

**Why is it needed?**

As the number of data exchanges or data integration points in a company grows so does the need for a structured approach to the design of the data integration. If data integration is implemented in an ad hoc manner with many point-to-point implementations, it will create unwanted dependencies between applications which in turn makes changing the application landscape a painful and expensive exercise.

A loosely coupled approach to data integration is preferable as it minimizes application dependencies in terms of availability, location, technology and data format. A loosely coupled architecture can be achieved by using a combination of [EAI design patterns](http://www.enterpriseintegrationpatterns.com/eaipatterns.html){:target="_blank"} and middle-ware products as implementation building blocks.

## Design Considerations

**Messaging**

Asynchronous Messaging is the core concept behind loosely coupled data integration. Asynchronous Messaging means that data is transported from sender to receiver in packages, usually with some metadata and usually via some middle-ware. Asynchronous in the messaging context means that the message is put on a queue by the sender and the sender then resumes processing. The message is transported to the recipient under the management of the messaging middle-ware which guarantees the safe delivery of the message to the receiver.

Using asynchronous messaging shields the sender from the receiver in the following ways, thus leading to looser coupling between applications:

*   Availability_,_ the sender does not have to concern itself with the availability of the receiver, the receiver can pick up its messages from a queue on the middle-ware when it is available.
*   Location, the sender does not have to know about the location of the receiver, this can be configured in the messaging middle-ware.
*   Technology, sender and receiver can run on different technology platforms. Most messaging middle-ware will support multiple platforms via APIs.

**Usage of EAI Patterns**

For an architect who is designing an integration solution, the usage of EAI Patterns act as a language in which to express the architecture. Patterns assist with component selection, this helps to prevent over engineering while meeting the requirements of the solution. EAI patterns can be combined with functionality in middle-ware platforms to form the solution.

For example, a common approach to minimizing dependencies between application data models is to use the [Canonical Data Model pattern](http://www.enterpriseintegrationpatterns.com/CanonicalDataModel.html){:target="_blank"} which is implemented using two Message Translators. A Message Translator can be implemented in a number of ways, on most technology platforms and by most middle-ware products.

**External Integration (B2B / EDI)**

Along with data integration between applications within the same company (Application to Application, or “A2A”) another common type of data integration is between business partners. This is known as Business to Business, B2B or Electronic Data Interchange (EDI).

Due to the nature of this data exchange there is a natural focus on communication security and also on the standardization of the message formats.

Middle-ware products typically support one or more EDI standards such as ODETTE or EDIFACT along with secure communication protocols such as SFTP or OFTP.

A typical use case for EDI is when an external supplier sends an Advance Shipping Notice to provide detailed information about a shipment in advance of delivery to the customer.

*   **Iasa Certification Level** **Learning Objective** **CITA- Foundation** Learner can explain what Messaging and EAI Patterns are.
*   Learner can describe A2A and B2B integration.
*   **CITA – Associate** Learner can distinguish between EAI Patterns and understands how Asynchronous Messaging can contribute to a loosely coupled architecture.
*   Learner can give examples of scenarios for A2A and B2B integrations.
*   **CITA – Specialist** Learner can use EAI Patterns to describe complex integration scenarios.
*   Learner can judge when messaging should be applied or not.
*   Learner can combine middle-ware products to implement both A2A and B2B integrations.
*   **CITA – Professional** Learner uses EAI Patterns to design integration solutions.
*   Learner can distinguish between different messaging middle-ware.
*   Learner can select middle-ware products for A2A and B2B integration.

## Data Virtualization & Data Federation

Data virtualization is the process of offering data consumers a data access interface which hides the technical aspects of stored data, such as location, storage structure, access language, and storage technology.

Data federation is a form of data virtualization where the data stored in a heterogeneous set of autonomous data stores is made accessible to data consumers as one integrated data store by using on-demand data integration.

With a federation server, multiple data stores can be made to look as one. Consuming applications submit queries which are decomposed into subqueries, these subqueries are submitted to the individual data stores and when the data is retrieved it is transformed and composed into a single dataset before being returned to the consumer. Therefore, integration takes place at runtime and not in batch which is unlike other approaches. The data is not stored in its integrated form (although it may be cached), it remains at its original location in its original format.

**Advantages of Data Federation**

*   Reduce system and network workload by not moving data around which may never be used.
*   Reduced risk of stale data by delivering more real-time data access.
*   Reduction of data storage requirements.

**Disadvantages of Data Federation**

*   Operational system performance can be affected by spikes in heavy on-demand queries.
*   Change management is critical as any changes must be accepted by all consuming applications and users of the shared data resources.
*   **Iasa Certification Level** **Learning Objective** **CITA- Foundation** Learner will be able to discuss data virtualization.
*   Learner will be able to discuss data federation.
*   **CITA – Associate** Learner will be able to identify scenarios where data federation could be applied.
*   Learner will be able to discuss the advantages and disadvantages of data federation.
*   **CITA – Specialist** Learner will be able to evaluation data federation products.
*   Learner will be able to design a data federation solution.
*   **CITA – Professional** Learner will be able to mentor others in data federation.

# Related Capabilites

*   [Information Management](information_management.md){:target="_blank"}
*   [Information Modeling](information_modeling.md){:target="_blank"}
*   [Information Usage](information_usage.md){:target="_blank"}

# Resources

*   [Extract, Transform, Load](http://en.wikipedia.org/wiki/Extract,_transform,_load){:target="_blank"} (Wikipedia)
*   [http://www.dataintegration.info/](http://www.dataintegration.info/){:target="_blank"}
*   [http://www.dataacademy.com/files/ETL-vs-ELT-White-Paper.pdf](http://www.dataacademy.com/files/ETL-vs-ELT-White-Paper.pdf){:target="_blank"}
*   [http://www.enterpriseintegrationpatterns.com/eaipatterns.html](http://www.enterpriseintegrationpatterns.com/eaipatterns.html){:target="_blank"}
*   [http://www.enterpriseintegrationpatterns.com/CanonicalDataModel.html](http://www.enterpriseintegrationpatterns.com/CanonicalDataModel.html){:target="_blank"}
*   [http://www.enterpriseintegrationpatterns.com/docs/EDA.pdf](http://www.enterpriseintegrationpatterns.com/docs/EDA.pdf){:target="_blank"}
*   [http://en.wikipedia.org/wiki/Comparison\_of\_business\_integration\_software](http://en.wikipedia.org/wiki/Comparison_of_business_integration_software){:target="_blank"}
*   [http://en.wikipedia.org/wiki/Advance\_ship\_notice](http://en.wikipedia.org/wiki/Advance_ship_notice){:target="_blank"}
*   [Federated database system](https://en.wikipedia.org/wiki/Federated_database_system){:target="_blank"} (Wikipedia)
*   [Clearly Defining Data Virtualization, Data Federation, and Data Integration](http://www.b-eye-network.com/view/14815){:target="_blank"}

# Authors

![Declan Bright](media/declan_bright.jpg)
**Declan Bright**
*Chief Software Architect*

Declan Bright is a Chief Software Architect based in Dublin, Ireland. He has worked in the IT industry since 1999, primarily within the aviation, telecommunications and financial services sectors and has extensive experience in the design and implementation of enterprise solutions. Areas of specialisation include system integration, system evolution, user experience and analytics.  [www.declanbright.com](http://www.declanbright.com){:target="_blank"}

**John Kaber**
*IT Architect – Volvo IT*