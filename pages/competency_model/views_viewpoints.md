---
title: "Views & Viewpoints"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: views_viewpoints.html
folder: competency_model
summary: "IT architects must have the ability to clearly understand the concepts of views, viewpoints, and perspectives, to understand the differences between them and how they work together to describe an architecture. "
tags:
  - design
---

# Description

The concept of views and viewpoints is widely understood across the architecture community, having originated back in the 1970's in Doug Ross' Structured Analysis and Design Technique (SADT). Later, the concept of views became widely accepted following the development of Kruchten's 4 + 1 architecture view model at Rational Software, and they have since been formalized in the  [ISO/IEC/IEEE 42010:2011](http://en.wikipedia.org/wiki/ISO/IEC_42010){:target="_blank"}, *Systems and software engineering --- Architecture description* standard.

The principles of views and viewpoints are defined in slightly different ways in different places; the definitions adopted by IASA are:

-   An architectural view is a representation of one or more aspects of an architecture that illustrates how the architecture addresses the concerns held by one or more of its stakeholders.
-   A viewpoint is a collection of patterns, templates, and conventions for constructing one type of view. It defines the stakeholders whose concerns are reflected in the viewpoint and the guidelines, principles, and template models for constructing its views.

An example would be to use an operational viewpoint to create a view targeted at the IT Operations group. The viewpoint is the template that contains information relevant to the operation of the system, and a view is the end product delivered to someone interested in maintaining the operational capability of the system.

IT architects must have the ability to clearly understand the concepts of views, viewpoints, and perspectives, to understand the differences between them and how they work together to describe an architecture. They must be able to discern various stakeholder groups typical of IT development projects, understand the typical concerns of each group, and determine the set of views needed to satisfy the requirements of a particular project.

# Overview

One of the main responsibilities of the architect is to present the vision of the system to the stakeholders interested in it. In anything other than the most trivial of systems it is not possible to show this effectively in a single diagram and so the concept of views and viewpoints has been developed to allow the architectural description to be decomposed into a set of related pieces that each provide the appropriate information in an appropriate way to interested stakeholders.

The ISO 42010 standard defines the relationship between the system, its architecture, the stakeholders and the architectural description:


Figure 1. Excerpt from Conceptual Framework of ISO42010

Most architectural description are structured as a set of views which contain the main architectural information. A number of viewpoint sets exist, which vary in different ways, but the viewpoints in most architectural frameworks will include a description of the system's functional structure, its key data structures, a viewpoint addressing how the software is developed, and some form of deployment viewpoint that explains how the software is deployed into its runtime environments.

# Proven Practices

A number of viewpoint-based architectural frameworks exist and  a comprehensive list is available here: [http://www.iso-architecture.org/42010/afs/frameworks-table.html](http://www.iso-architecture.org/42010/afs/frameworks-table.html){:target="_blank"}. For software intensive systems some of the more commonly used viewpoint sets are as follows:

Kruchten's 4 + 1 architecture view model

This approach forms the basis of the Rational Unified Process has a small set of fixed views defined, with viewpoints implied rather than being explicitly identified

The views of the model are concerned with:

-   **Logical view**: The logical view is concerned with the functionality that the system provides to end-users. UML Diagrams used to represent the logical view include [Class diagram](http://en.wikipedia.org/wiki/Class_diagram){:target="_blank"}, [Communication diagram](http://en.wikipedia.org/wiki/Communication_diagram){:target="_blank"}, [Sequence diagram](http://en.wikipedia.org/wiki/Sequence_diagram){:target="_blank"}.
-   **Development view**: The development view illustrates a system from a programmer's perspective and is concerned with software management. This view is also known as the implementation view. It uses the UML [Component diagram](http://en.wikipedia.org/wiki/Component_diagram){:target="_blank"} to describe system components. UML Diagrams used to represent the development view include the [Package diagram](http://en.wikipedia.org/wiki/Package_diagram){:target="_blank"}.
-   **Process view**: The process view deals with the dynamic aspects of the system, explains the system processes and how they communicate, and focuses on the runtime behavior of the system. The process view addresses concurrency, distribution, integrators, performance, and scalability, etc. UML Diagrams to represent process view include the [Activity diagram](http://en.wikipedia.org/wiki/Activity_diagram){:target="_blank"}.
-   **Physical view**: The physical view depicts the system from a system engineer's point of view. It is concerned with the topology of software components on the physical layer, as well as the physical connections between these components. This view is also known as the deployment view. UML Diagrams used to represent physical view include the [Deployment diagram](http://en.wikipedia.org/wiki/Deployment_diagram){:target="_blank"}.
-   **Scenarios**: The description of an architecture is illustrated using a small set of [use cases](http://en.wikipedia.org/wiki/Use_case){:target="_blank"}, or scenarios which become a fifth view. The scenarios describe sequences of interactions between objects, and between processes. They are used to identify architectural elements and to illustrate and validate the architecture design. They also serve as a starting point for tests of an architecture prototype. This view is **also known as use case view**.

Views and Beyond -- Documenting Software Architectures

The V&B approach, from the Software Engineering Institute, promotes a stakeholder-based view selection, but extends the concept to recognize that documentation beyond views is also essential to provide holistic insight into the overall design approach embodied by the architecture and the decision made in arriving at the architecture. The V&B approach takes a software centric stance and focuses on the structure of the software, the relationships between software components, and how the software relates to the external environment, it classifies views into 3 types:

-   **Module views** -- Modules represent a code-based way of considering the system. Modules are assigned areas of functional responsibility, and are assigned to teams for implementation. There is less emphasis on how the resulting software manifests itself at runtime. Module structures allow us to answer questions such as: What is the primary functional responsibility assigned to each module? What other software elements is a module allowed to use? What other software does it actually use? What modules are related to other modules by generalization or specialization (i.e., inheritance) relationships?
-   **Component-and-connector views** -- Here, the elements are runtime components (which are principal units of computation) and connectors (which are the communication vehicles among components). Component and connector structures help answer questions such as: What are the major executing components and how do they interact? What are the major shared data stores? Which parts of the system are replicated? How does data progress through the system? What parts of the system can run in parallel? How can the system's structure change as it executes?
-   **Allocation views** -- These views show the relationship between the software elements and elements in one or more external environments in which the software is created and executed. Allocation structures answer questions such as: What processor does each software element execute on? In what files is each element stored during development, testing, and system building? What is the assignment of the software element to development teams?

Software Systems Architecture

A fairly comprehensive set of viewpoints for information systems development is defined in the Rozanski and Woods "Software Systems Architecture" set, and includes the following viewpoint definitions:

-   [**Context**](http://www.viewpoints-and-perspectives.info/home/viewpoints/context){:target="_blank"} Describes the relationships, dependencies, and interactions between the system and its environment (the people, systems, and external entities with which it interacts). Many architecture descriptions focus on views that model the system's internal structures, data elements, interactions, and operation. Architects tend to assume that the "outward-facing" information --- the system's runtime context, its scope and requirements, and so forth -- is clearly and unambiguously defined elsewhere. However, you often need to include a definition of the system's context as part of your architectural description**.**
-   [**Functional**](http://www.viewpoints-and-perspectives.info/home/viewpoints/functional){:target="_blank"} Describes the system's functional elements, their responsibilities, interfaces, and primary interactions. A Functional view is the cornerstone of most ADs and is often the first part of the description that stakeholders try to read. It drives the shape of other system structures such as the information structure, concurrency structure, deployment structure, and so on. It also has a significant impact on the system's quality properties such as its ability to change, its ability to be secured, and its runtime performance.
-   [**Information**](http://www.viewpoints-and-perspectives.info/home/viewpoints/information){:target="_blank"} Describes the way that the architecture stores, manipulates, manages, and distributes information. The ultimate purpose of virtually any computer system is to manipulate information in some form, and this viewpoint develops a complete but high-level view of static data structure and information flow. The objective of this analysis is to answer the big questions around content, structure, ownership, latency, references, and data migration.
-   [**Concurrency**](http://www.viewpoints-and-perspectives.info/home/viewpoints/concurrency){:target="_blank"} Describes the concurrency structure of the system and maps functional elements to concurrency units to clearly identify the parts of the system that can execute concurrently and how this is coordinated and controlled. This entails the creation of models that show the process and thread structures that the system will use and the interprocess communication mechanisms used to coordinate their operation.
-   [**Development**](http://www.viewpoints-and-perspectives.info/home/viewpoints/development){:target="_blank"} Describes the architecture that supports the software development process. Development views communicate the aspects of the architecture of interest to those stakeholders involved in building, testing, maintaining, and enhancing the system.
-   [**Deployment**](http://www.viewpoints-and-perspectives.info/home/viewpoints/deployment){:target="_blank"} Describes the environment into which the system will be deployed, including capturing the dependencies the system has on its runtime environment. This view captures the hardware environment that your system needs (primarily the processing nodes, network interconnections, and disk storage facilities required), the technical environment requirements for each element, and the mapping of the software elements to the runtime environment that will execute them.
-   [**Operational**](http://www.viewpoints-and-perspectives.info/home/viewpoints/operational){:target="_blank"} Describes how the system will be operated, administered, and supported when it is running in its production environment. For all but the simplest systems, installing, managing, and operating the system is a significant task that must be considered and planned at design time. The aim of the Operational viewpoint is to identify system-wide strategies for addressing the operational concerns of the system's stakeholders and to identify solutions that address these.

TOGAF 9.1

Although primarily intended for enterprise architecture, TOGAF is used by some organisations for software projects. Here the concept of "domain" is sometimes used in a similar way to "viewpoint", although this is not the correct use of domains, as they are defined as being the commonly accepted subsets of an overall enterprise architecture. The following are defined in TOGAF:

-   The **Business Architecture** defines the business strategy, governance, organization, and key business processes.
-   The **Data Architecture** describes the structure of an organization's logical and physical data assets and data management resources.
-   The **Application Architecture** provides a blueprint for the individual applications to be deployed, their interactions, and their relationships to the core business processes of the organization.
-   The **Technology Architecture** describes the logical software and hardware capabilities that are required to support the deployment of business, data, and application services. This includes IT infrastructure, middleware, networks, communications, processing, standards, etc.

Archimate

Archimate is a modelling language developed specifically for the needs of enterprise architecture, which has evolved to support the TOGAF framework. Archimate defines 18 standard viewpoints to cover enterprise architecture work, serving the needs of a wide set of stakeholders. The approach and its viewpoints are comprehensively documented in the documentation available via the Open Group's [Archimate website](http://www.opengroup.org/subjectareas/enterprise/archimate){:target="_blank"}.

# Sub-Components Skills

## Selecting the Appropriate Set of Views or Viewpoints

It is common that large organizations mandate a framework which is defined in their architecture documentation template, but in other cases it will be up to the architect to make the selection. This decision will depend on the level of the architecture being defined and the type of system being described. Once experience has been gained with the standard viewpoint sets, architects often find that it is necessary to extend the standard viewpoint sets to meet the needs of their specific situation.  This is particularly important if a mandated framework only has a few views which do not address important concerns for the architect's specific situation (such as security, for example).  When non-functional concerns are not addressed using alternative approaches, such as perspectives, pragmatic architects often address them by adding extra views for these concerns.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will be able to describe views and viewpoints, and understand what they are
| | -   Learner will be able to name some of the different types of views and viewpoints
| **CITA -- Associate** | -   Learner will be able to describe the differences between various views and viewpoints
| | -   Learner will be able to describe the key elements of the commonly used views and viewpoints (covering functional, information and deployment as a minimum)
| **CITA -- Specialist** | -   Learner will be able to describe when it is most appropriate to use which views and viewpoints, and highlight the advantages and disadvantages of each
| | -   Learner will be able to describe how use at least one of the sets of views and viewpoints in detail for a project and be able to produce them
| **CITA -- Professional** | -   Learner will be able to identify new views and viewpoints for groups of stakeholders
| | -   Learner will know the risk of missing out some views and viewpoints and be able to justify this where appropriate

## Application of Views and Viewpoints

When the appropriate viewpoints have been selected, the architect needs to be able to produce the models defined and apply any techniques identified. This will usually entail using modelling languages like UML, Archimate or BPMN, as well as informal notations defined locally, along with the tools which support the notations in use.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will be able to name the various activities which are covered by the commonly used Viewpoints
| **CITA -- Associate** | -   Learner will be able to describe the activities and how they relate to each other across different Viewpoints
| | -   Learner will be able to use the commonly found models to produce Views on medium complexity projects
| | -   Learner will be able to use at least one of the modelling tools, like Enterprise Architect, Magic Draw, Rational Software Architect or Archi to define the models
| **CITA -- Specialist** | -   Learner will be able to use all the appropriate Viewpoints on the development of large and complex project environments
| | -   Learner will be able to define in detail all of the activities
| | -   The Learner will be able to relate the Views to the stakeholders objectives
| **CITA -- Professional** | -   Learner will be able to suggest significant specializations in the Viewpoints for an organization
| | -   Learner will be able to propose new combinations of Veiwpoints

## View and Viewpoint Management

Ideally a mature architecture organisation should have a process in place to manage viewpoints for re-use and leverage views that have been produced.  This will involve capturing when views are created and used in the organisation, the information that each requires, the modeling techniques that they use, and a rationale for each of these choices.  Ideally all of this information will be captured in some sort of enterprise repository.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will be able to describe the management process at their organization
| | -   Learner will be able to explain the reasons for managing Views and Viewpoints
| **CITA -- Associate** | -   Learner will be able to construct simple Views for inclusion in the process
| | -   Learner will be able to describe how and why they applied the Viewpoints for a project
| **CITA -- Specialist** | -   Learner will be able to critique content for inclusion in the repository
| | -   Learner will be able to define the principles to apply governing inclusion
| **CITA -- Professional** | -   Learner will be able to create meta-models for use by others
| | -   Learner will be able to invent and reinforce the management process

# Capabilities Resources

**Related Capabilities:**

-   Architecture Description
-   [Whole System Design](the_whole_systems_design.md){:target="_blank"}

**Resources:**

Rozanski & Woods: Software Systems Architecture (2nd Edition)

Software Engineering Institute: Software Architecture in Practice (3rd Edition)

Blogs/Webcasts/News/Reference sources:

TOGAF: [http://pubs.opengroup.org/architecture/togaf9-doc/arch/index.html](http://pubs.opengroup.org/architecture/togaf9-doc/arch/index.html){:target="_blank"}

Architmate:  [http://pubs.opengroup.org/architecture/archimate2-doc/chap08.html](http://pubs.opengroup.org/architecture/archimate2-doc/chap08.html){:target="_blank"}

Rozanski & Woods Web site: [http://www.viewpoints-and-perspectives.info/](http://www.viewpoints-and-perspectives.info/){:target="_blank"}

[http://www.iso-architecture.org/42010/](http://www.iso-architecture.org/42010/){:target="_blank"}

# Author

## Chris Cooper-Bland
*Group Head of Architecture -- Endava*
