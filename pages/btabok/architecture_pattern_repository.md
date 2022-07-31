---
title: Architecture Pattern Repository
tags: [architecture]
keywords:
summary: "Developers must design clean, clearly designed code to avoid bug creep into the system, and avoid complexity."
sidebar: mydoc_sidebar
permalink: requirements_modeling.html
folder: btabok
---

> “All well-structured object-oriented architectures are full of patterns. Indeed, one of the ways that I measure the quality of an object-oriented system is to judge whether or not its developers have paid careful attention to the common collaborations among its objects.”

*Grady Booch, Design Patterns: Elements of Reusable Object-Oriented Software*


# Design Patterns

Developers must design clean, clearly designed code to avoid bug creep into the system, and avoid complexity. Designing a system is not easy.

However, it is not required to solve all problems “from scratch”. It is preferable to learn from and deploy the lessons from the captured experiences of other designers.

Design Patterns are reusable solutions to common problems in software system design.

## History of Design Patterns

Christopher Alexander and his colleagues were the first to discuss patterns in the context of building and construction (*The Timeless Way of Building*, 1979; *A Pattern Language—Towns, Buildings, Construction*, 1977). They had 253 patterns.

Over time, it has been observed that there are many similarities between software design and architectural design (as in the context of building construction).

This observation was used by different software design experts. The most well-known technical” work on this has been by Erich Gamma, John Vlissides, Ralph Johnson, and Richard Helm in “*Design Patterns: Elements of Reusable Object-Oriented Software*”, published in 1994. The four authors (famously known as the Gang of Four) applied the concepts of patterns to software design.

Over time, the library of patterns has grown. There are patterns spanning a range of topics in the software domain, like Cloud patterns, Microservice patterns, Enterprise systems patterns and general software design patterns.

How can Design Patterns Help?

Design patterns help to speed up the development process through the usage of proven and tested building blocks for the context under consideration. They provide a means to address common problems that frequent occur in the design of software development, irrespective of the category.

**Reusability**

The fundamental principle here is to avoid reinventing the wheel.

For example, consider the MVC (Model-View-Controller) pattern that was traditionally used in the design of desktop user interfaces. It was observed that web-based UIs had similar or related requirements and design principles; it led to the adoption of the MVC pattern in Web-based UI systems as well.

**Common Vocabulary**

Design patterns provide a common vocabulary for software engineers to communicate, through the usage of well-known and well-understood names for specific software interactions.

For example, when a designer refers to the usage of a singleton in a specific software design, it is immediately obvious to other designers and developers what is required.

**Reducing the amount of variability and increasing Cohesion**

Once the problem has been studied, designing with patterns will result in a cohesive solution with minimal coupling, built with “pre-fabricated” blocks. There will be fewer parts in the design that cannot be achieved with patterns.

**Specifying Design Patterns**

The specification of a Design Pattern is usually subjective. However, most specifications usually conform to the basic template below.

| **Term**               | **Description**                                                                                                                                                                       |
|------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Name                   | A short descriptive appellation for the pattern, usually indicative of its purpose.                                                                                                   |
| Functional description | A description of what the pattern does.                                                                                                                                               |
| Synonyms               | Other names for the pattern                                                                                                                                                           |
| Motivation             | A description of the problem for which this pattern could be the solution                                                                                                             |
| Usage scenario         | Where this pattern would be applicable                                                                                                                                                |
| Structure              |  How to construct an implementation based on this pattern                                                                                                                             |
| Stakeholders           | Other entities with whom the construct in question would interact, and how the interaction would take place. The individual responsibilities of all the actors in the given scenario. |
| Expected Behaviour     | The consequences of the usage of the pattern in a given situation                                                                                                                     |

Pattern Types and Catalog

| **Pattern Type** | **Architectural Relevance**        | **Patterns**                                                                     |
|------------------|------------------------------------|----------------------------------------------------------------------------------|
| Cloud            | Infrastructure, Software, Solution | [Cloud Patterns Library](https://btabok.iasaglobal.org/btabok_3/cloud-patterns/) |
| Microservices    | Infrastructure, Software, Solution | Microservices Patterns Library                                                   |
| Software Design  | Software, Solution                 | Software Patterns Library (example: Gang of Four                                 |

