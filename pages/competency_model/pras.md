---
title: "Performance, Reliability, Availability, Scalability"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: pras.html
folder: competency_model
summary: "The architect needs to be able to describe what each quality attributes represents."
tags:
  - quality_attributes
---

# Description

Code does not live in isolation. Once it is deployed to production the system needs to fulfill the expected level of performance. It needs to be reliable, available based on the SLA (Service Level Agreement) and scale if needed. It does not matter how good a program is in terms of UI or features, it is useless if it is too slow and it lacks availability when the user needs it. Performance, Reliability, Availability and Scalability (PRAS) are all run-time quality attributes that need to be carefully design and implemented in order to make a system usable. Any component, small or large, can impact the behavior of a system directly or indirectly by its effect on other components.

# Overview

## Why does an architect need this skill?

No software product can exist without a solid foundation. The Quality Attributes provide the solution for this foundation. Since the architect is the key person in building the software, they need to be the master of the QAs.

## Common tasks involved in this skill?

The architect needs to be able to describe what each quality attributes represents, how to measure each attribute and how the attributes affect each other. They need to be able to prioritize the importance of the Quality Attributes and its effect on the project since inception to production and throughout maintenance.

## What is their ownership in this skill?

The architect is the main owner of the Quality Attributes (also knows as non-functional requirements).

## Name an example of how an architect would use this in daily activities?

They need to be able to measure the attributes for an existing software application.

They need to be able to identify the risks and recommend the most optimal solution.

## Describe why an architect should be involved in this skill at a corporate level

Since no one else owns the non-functional requirements, aka Quality Attributes, the Architect needs to be the master and identify these attributes as well as be responsible for their implementation.

## Primary push back and/or challenges for architects

The functional requirements usually take priority. No one except the Architect owns the quality attributes. Therefore, it is the Architect 's job to make sure all the stakeholders understand how important is to spell out the non-functional requirements, prioritize them, and allocate the time and resources to take care of the QAs throughout the life cycle of the project.

## How would a stakeholder engage an architect for assistance utilizing this skill?

During the early stages of a project the Architect needs to be involved in the discussions that shape the definition of the project. This is to help identify the constraints and spell out the trade offs between the Quality Attributes.

# Sub-Capabilities


## Performance

Performance is the driving factor for any system architecture.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will be able to define Performance
| | -   Learner will be able to describe the difference between perceived performance and actual performance
| | -   Learner will be able to describe the difference between latency and throughput
| **CITA -- Associate** | -   Learner will be able to measure the performance of an existing application, its throughput and latency
| | -   Learner will know how to use dedicate tools to measure: profilers, code analysis, etc
| | -   Learner will be able to identify and document scenarios and use cases that negatively impact Performance
| **CITA -- Specialist** | -   Learner will be able to design a system that is easily measurable in terms of Performance and has built in ways to assist troubleshooting, e.g. logging, instrumentation, etc.
| **CITA -- Professional** | -   Learner will be able to design and implement tests that can predict the Performance breaking points of a system
| | -   Learner will be able to describe and predict the negative impact on a business if the Performance is not achieved as expected

## P.R.A.S. -- Knowledge Overlap

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Know the concepts related to Performance, Reliability, Availability and Scalability as well as the application of their trade offs during the whole system life cycle.
| | -   Be able to describe the differences between PRAS and how they affect each other as well as how they affect other Quality Attributes
| | -   Know the definition of Reliability.
| | -   Know the definition of Availability. Be able to explain what SLA stands for.
| | -   Know what DoS (Denial of Service) attack is
| | -   Know the difference between High Availability vs. Disaster Recovery
| | -   Know how much downtime you can afford with N 9s (99%, 99.9%, 99.99%, etc.)
| | -   Know the definition of scalability. Be able to explain the difference between scaling horizontally (scale out) and vertically (scale up).
| | -   Describe how state-ness/statelessness affects horizontal scalability
| **CITA -- Associate** | -   Understand the difference between SLA and OLA.
| | -   Know the Fallacies of Distributed Computing
| | -   Know the CAP Theorem. Be able to choose 2 of the 3 in CAP
| | -   Be able to use instruments and tools to detect DoS
| | -   Be able to identify and document scenarios and use cases that negatively impact PRAS.
| **CITA -- Specialist** | -   Be able to design a system that is easily measurable and has built in ways to assist troubleshooting, e.g. logging, instrumentation, etc.
| | -   Be able to engage the proper stakeholders and explain to them the trade-offs required when choosing a higher priority for a Quality Attribute over other QAs.
| | -   Be able to design systems that prevent and minimize DoS.
| | -   Understands Business Continuity Planning (BCP)
| | -   Know how to measure scalability as opposed to load
| | -   Know how to build a recoverability plan.
| | -   Know how to plan the right capacity.
| | -   Know how to plan for unpredictable capacity growth.
| | -   Know how to reach the availability target.
| | -   Understand that Architectural Styles like REST are about Quality Attributes
| **CITA -- Professional** | -   Be able to use the Quality Attributes perspective when designing and architecting a complex system to make Performance part of the initial design and implementation. Be able to identify the risks early on.
| | -   Can provide guidance for scalability rather than absolutes.
| | -   Be able to balance the quality attributes.
| | -   Be able to provide trade-offs between the Quality Attributes.
| | -   Has a habit for extracting and defining the requirements for the Quality Attributes.
| | -   Create and deliver the strategy for maintaining the QAs.
| | -   Work with other stakeholders like IT and Information Security to have a plan to keep an eye on the architecture drift and erosion.

# Resources

**Articles**

-   [IASA BTABoK](https://btabok.iasaglobal.org)
-   CITA-S Overview Manual
-   [Fielding's Dissertation about REST](https://www.ics.uci.edu/~fielding/pubs/dissertation/top.htm)
-   [SLA vs. OLA](http://itsm.certification.info/slavola.html)
-   [MSDN: Quality Attributes](https://msdn.microsoft.com/en-us/library/ee658094.aspx)
-   [MSDN: Understanding Availability, Reliability, and Scalability](https://technet.microsoft.com/en-us/library/aa996704(v=exchg.65).aspx)
-   [MSDN: Overview of System Performance](https://msdn.microsoft.com/en-us/library/ms978391.aspx)
-   [A plain English introduction to CAP Theorem](http://ksat.me/a-plain-english-introduction-to-cap-theorem)
-   [CAP Twelve Years Later: How the "Rules" Have Changed](http://www.infoq.com/articles/cap-twelve-years-later-how-the-rules-have-changed)
-   [SEI Quality Attributes](http://resources.sei.cmu.edu/library/asset-view.cfm?assetid=12433)
-   [SEI Reasoning about Quality Attributes](http://www.sei.cmu.edu/architecture/tools/establish/qaw.cfm)

**Blogs/Webcasts/News/Reference sources**

-   [The Eight Fallacies of Distributed Computing](https://blogs.oracle.com/jag/resource/Fallacies.html)
-   [SEI Blog "Evolutionary Improvements of Quality Attributes: Performance in Practice"](http://blog.sei.cmu.edu/post.cfm/evolutionary-improvements-quality-attributes-251)

**Training** --

**Certifications** --

**Books**

-   Less Bass, Paul Clements, Rick Kazman, "Software Architecture in Practice", Third Edition, Addison-Wesley, 2013
-   Richard N. Taylor, Nenad Medvidovic, and Eric M. Dashofy, "Software Architecture: Foundations, Theory, and Practice", 2008

# Author

![Danut Prisacaru](media/d_prisacaru.jpg)
**Danut Prisacaru**
*Sr. Principal/Engineer V (Integration Architect) -- The Advisory Board Company*

Danut Prisacaru has been a Software Engineer for over 20 years and a Software Architect for over 7 years serving in different roles: Application Architecture, Integration and Solutions Architecture. His current focus is SOA with Web APIs and Lightweight ESBs and API Management tools to serve the business integrate complex parts and components in an efficient manner.

Danut has BS in CS from the Technical University "Gh. Asachi" Iasi Romania and holds a certification from IASA as well as other industry organizations.

Danut's hobby is Philosophy that helps him be a better software architect.



