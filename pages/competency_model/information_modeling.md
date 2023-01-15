---
title: "Information Modeling"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: information_modeling.html
folder: competency_model
summary: "As enterprises attempt to create value from their information assets."
tags:
  - information_architecture
---

# Description 

Information modeling is the set of practices that determine the structure, lifecycle and accessibility requirements of the information in the domain of a business. It  is required in today's businesses to enable information flow throughout the organization. Much like the modeling during software development, where designers create models of the class structure, database schemas, and systems architecture, developing an information model that is flexible enough to absorb future changes is an art that requires balancing functionality, performance, resilience, security, and flexibility.

An Information model is a design aid and an artifact referenced throughout the lifecycle of information as it relates to systems and processes. It is used by architects to represent something in a given context needed to drive business value. Building design blueprints, maps, and organization charts are all examples of using an agreed upon format to communicate ideas and represent something in the environment.

# Overview

As enterprises attempt to create value from their information assets, information modeling provides an important tool to communicate the design, standards and key aspects of the entities in the context of the domain being represented to all involved throughout the lifecycle of the information.

Since information resides and is accessed in many disparate formats and structures (files, relational databases, non-relational databases, services, block chains) the need to be able to query, relate, organize, format, report, store, update and alter the schema of entities requires coordination and planning. Information modeling is a tool for information management, supports creating trustworthy/quality data while maintaining the integrity of the data, thus allowing architectures to be robust and scalable.

Modeling is a particular challenge when data resides in unstructured sources such as spreadsheets, text documents, wikis, document collaboration sites, etc. At best, the medium is actually semi-structured providing known meta-data. Alternatively, vendors provide tools that can assist with searching document content, or mining content for data and meta-data. However, the costs, quality, performance issues and risks are high when it comes to changing business process and gaining information value around these sources.

Models are mostly thought of as being created during requirements gathering and further refined in design phases, referenced during implementation and kept as an artifact to be referenced thereafter. However, there are significant efforts in developing them for other Information Management capabilities, such as Data Governance, Master Data Management, Information Integration, Analytics and Information Security.

Information modeling in IT Architecture takes many forms, all of which have representations of entities and their relationships to one another:

-   Class diagrams: model the information required to build or maintain a system or component
-   ER diagrams: data modeling specific for database design
-   Information flow diagrams: indicates origin of data and its uses (process or systems) throughout either the enterprise, line of business (LOB) or system, depending on the context
-   Data models: depending on level of detail, describes the entities and its relationships detailing attributes, types and multiplicity of an entity to other entities
-   Data lifecycles: how data is created, used and retained (archived or destroyed)

Models will vary depending on a number of factors: usage (whether analytical or transactional), focus (global, enterprise, LOB or system) and level of detail (conceptual, logical, or physical). For example, customer data from an online application will differ from the data used to gather statistics on customer location, where the model of the former would have a normalized structure and the latter a star or snowflake schema. Modeling also can indicate boundaries showing the limits of the information flow needed for regulatory compliance or business access restrictions having audit trails and tight security around authentication and authorization. Models may be relevant either for only a small group of individuals for a specific business process need, or it could be recognized as a global industry-standard.

A model provides a formalized format that aids conversations between architects and users, stakeholders, other architects and analysts. Modeling languages standardize the notations conveying the meanings of entities, attributes, transitions, relationships, identifiers and others. A modeling session with subject matter experts will assist in translating real-world concepts (a business scenario/process) to the correct entities and information for the business needs. The notation helps ensure the meaning is not lost during design and implementation phases. Therefore, it is important to have session participants understand the notations being used. Improper analysis and understanding of the usage of the data will lead to performance, reliability, availability and scalability issues.

# Proven Practices

Information models and modelling is useful for the IT Architects as follows:

-   Business architects: Important to aid in gathering and determining requirements of a business process
-   Information architects: Will use to communicate storage, retrieval and integration of critical enterprise information. May be required to produce models top-down (design target state for gap analysis) or bottom-up (reverse engineer legacy system impacts).
-   Solution and Software architects: Assists with aspects of information that effects their systems such as flow of information, structure of data to be received or created
-   Infrastructure architects: Will use physical models to guide specifications to build out components of architecture

Though this artifact can be a powerful tool, it is nothing without the support to see through Information Management initiatives, such as EAI, Data Governance and/or Master Data Management, through funding and leadership.  Additionally, the notion that models are sometimes thought of as unnecessary documentation needs to be challenged.

# Sub-Capabilities

## Discover and Analyze Domain Information Requirements

Similar to Requirements Discovery capability, the focus here is to discover the domain information model requirements to aid in the creation of the information model.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** |

-   Learner will be able to understand the  requirements and model discovery sessions

 |
| **CITA -- Associate** |

-   Learner will be able to participate in requirements and model discovery sessions

 |
| **CITA -- Specialist** |

-   Learner will be able to conduct requirements and model discovery sessions, which includes involving determining entities and relationships by asking key probing questions.

 |
| **CITA -- Professional** |

-   Learner will be able to mentor key individuals to conduct requirements and model discovery sessions

 |

## Design Information Model to support requirements

Different approaches in developing models and to understand the business process:

-   KISS: Keep it simple and straight-forward
-   Top-down: sit with business, SME or user brainstorming/defining needs
-   Bottom-up: reverse engineer a legacy system
-   Many Lean Six Sigma techniques can be employed to discover domain model

This with discovery sessions, will lead to a conceptual information model: a high-level business architecture / basic, critical elements. Used for communication between architects and SMEs, stakeholders or users.

The following lists what is generally captured in models:

Entities

-   Important nouns depend on context whether global, enterprise, LOB or specific to an area
-   Include entities' attributes (location depends on model, usage, level of abstraction. For example, Customer Phone attribute placement will differ in a conceptual model, 3NF data model and star schema model)
-   Special attributes:
    -   Identifiers -- used for matching and fuzzy matching; determining uniqueness. Can be a single attribute or a combination of attributes that are unique.
    -   Foreign Keys -- Identifiers that create relationships to other entities
    -   State -- state or lifecycle models highlight transitions
-   Learn the correct level of granularity to allow for agility and re-use by multiple and varied consumers
-   If required, include historical and/or versioning entities or attributes

Relationships

-   Describe the relationship between two entities using multiplicity/cardinality notation
-   Describes referential integrity: business rules to ensure data quality
-   Learn the correct level of granularity to allow for agility and re-use by multiple and varied consumers
-   Is-a/Has-a relations

Specific to Information Management, models represent the data classified as:

-   Meta-data
-   Master Data
-   Operational Data
-   Unstructured Data
-   Analytical Data

Common Modeling Notations

-   [Information Engineering (IE) Crow's Foot notation](https://en.wikipedia.org/wiki/Entity%E2%80%93relationship_model#Crow.27s_foot_notation)
-   [IDEF1X](https://en.wikipedia.org/wiki/IDEF1X)
-   [Unified Modeling Language (UML)](https://en.wikipedia.org/wiki/Unified_Modeling_Language)
-   [Object-Role Modeling (ORM)](https://en.wikipedia.org/wiki/Object-Role_Modeling) [not to be confused with Object-Relational Mapping]
-   [State machines](https://en.wikipedia.org/wiki/Finite-state_machine)

A wide variety of tools are available to assist architects with the creation and management of model artifacts.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will know the relationship patterns (1:1, 1:m, m:m) and their implications for keys and associative entities
| | -   Learner is aware of the normalization rules for data models
| | -   Learner understands significance of the entities in business domain being modeled
| | -   Learner able to follow model logic
| **CITA -- Associate** | -   Learner will be able to discover detailed cardinality and optionality of relationships
| | -   Learner will be able to normalize and de-normalize structures
| **CITA -- Specialist** | -   Learner will be able to conduct sessions to discover data models
| **CITA -- Professional** | -   Learner will be able to optimize model for usage and purpose
| | -   Learner will be able to ask key questions of SMEs to aid in discovery, translating answers to model notation

## Analyze Information Models

Look to optimize entities and relationships depending on usage: searches, transactional, or reporting. Provide flexibility relative to current needs of consumers versus anticipated future changes.

This will lead to a logical and physical models. This is where considerations are needed to ensure performance, scalability, reliability, availability of data depending on usage.

These models differ in the level of detail due to their differing purposes:

-   Logical Information Model: detailed but technology-independent (architect to architects, developers or analysts)
-   Physical Information Model: detailed view that specifies technology (architect to infrastructure architect, vendors, MSPs or analysts)

Conceptual and Logical Modeling represent information in an agnostic format unrelated to the storage and usage of the entities. Logical models are designed with correct approach depending on usage (entity relationship modeling or dimensional data modeling)

Physical models provide technology detail to be able to spec and build out the structure of the information.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will be able to understand the that there are different usages
| | -   Learner will be able to understand the different scopes
| | -   Learner will be able to identify differences in forms of dimensional modeling (star and snowflake schemas) and entity relationship modeling
| **CITA -- Associate** | -   Learner will be able to identify whether model is appropriate for usage, scope, level of detail and purpose
| | -   Learner will be able to identify when normal form versus non-normalized structure is needed
| **CITA -- Specialist** | -   Learner will be adjust model appropriate for usage, scope and flexibility for future changes
| | -   Learner will be able match models with known common data model patterns
| **CITA -- Professional** | -   Learner will be able critique models knowing when to need to follow common data model patterns and when differences are appropriate as dictated by requirements

## Model Information Flows and Lifecycles

These important aspects of information can be captured in models, where:

-   Flows will incorporate data movement from integration efforts (such as MDM and ETL) and analytical efforts (such as Data Marts,Data Warehouses and Business Intelligence (BI))
-   Lifecycles will follow the data's retention plan.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will be able to understand information flow diagrams
| | -   Learner will be able to understand information lifecycle diagrams
| **CITA -- Associate** | -   Learner will be able to assist in documenting information flow diagrams
| | -   Learner will be able to assist in documenting information lifecycle diagrams
| **CITA -- Specialist** | -   Learner will be able to discover, document and analyze information flow diagrams
| | -   Learner will be able to discover, document and analyze information lifecycle diagrams
| **CITA -- Professional** | -   Learner will be able to describe and critique each piece of the information flow diagrams
| | -   Learner will be able to describe and critique each piece of the information lifecycle diagrams

# Resources

-   [Agile Modeling](http://www.agilemodeling.com/){:target="_blank"}

-   The DAMA Guide to the Data Management Body of Knowledge (DAMA-DMBOK). Bradley Beach, NJ: Technics Publications, 2010.
-   Godinez, M., Hechler, E., et al. The Art of Enterprise Information Architecture, A Systems-Based Approach for Unlocking Business Insight. IBM Press, 2010.
-   Hay, David C. Data Model Patterns: Conventions of Thought. New York, NY: Dorset House Publishing, 2011.

# Author

![Bina Reed](media/b_reed.jpg)
**Bina Reed**
*Enterprise Information Architect -- MPI Research*

Bina has held many roles in IT over the past two decades, including Software Developer, Systems Programmer and Information Architect. She has worked in a variety of industries in the U.S. -- software, higher education, CPG, healthcare and drug-development -- implementing large, complex technology solutions with multiple components. She has extensive experience managing the interplay between enterprise, legacy, customized and vendor systems, with the objective of achieving beneficial results in cost-restricted environments.

She holds an M.S. in Computer Science from the University of Georgia and a Bachelor of Architectural Engineering degree from Penn State University.

Prior to switching careers into IT, she was a licensed Professional Electrical Engineer (P.E., State of Illinois). The irony of becoming an architect in IT after being an engineer in the building industry is not lost on her.
