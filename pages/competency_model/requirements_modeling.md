---
title: "Requirements Modeling"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: requirements_modeling.html
folder: competency_model
summary: "Requirements modeling is carried out after the requirements and constraints for an area have been captured and analysed, it is an important activity to ensure the consistency and completeness of the requirements."
tags:
  - design
---

# Description

Requirements modeling is carried out after the requirements and constraints for an area have been captured and analysed, it is an important activity to ensure the consistency and completeness of the requirements. There are multiple ways to model functional, quality attributes and constraints. The appropriate approach to take will depend on the type of system and the organizational standards, in some cases they are domain specific modelling languages which are used. An important aspect of this is how to transform models of one type into another. Traceability is also an important aspect of this, as some projects will need to map the delivery of specific requirements to the component(s) that delivers it.

# Overview

Architects are expected to be experienced with the different ways to model functional requirements, although on a project of any size it will usually be the responsibility of the analyst, the architect will need to have this capability to validate models which have been produced, especially to quickly identify the architecturally significant requirements. Architects may also have to model requirements for a specific area such as where a Proof of Concept is being produced early on, or for a technical area like operational management. Obviously the architect must be able to understand and interpret the requirements models to develop the architecture.

Depending on the organizations role definitions, or the analyst’s experience, the modelling of quality attributes will sometimes become the responsibility of the architect as they are reliant on understanding these due to their significant impact on producing an architecture which will meet the business need. This includes identifying and describing architectural trade-offs, which is covered by the capability: “Optimizing Quality Attributes”.

# Proven Practices

There are many ways requirements can be modelled; some of the most common requirements models which are used include the following:

The Domain Model

The Domain Model captures all things (Domain Concepts) the product or system “deals with”, i.e. represents and manipulates from a business perspective. The information captured for a Domain Concept is a description and often as well properties and their relationship to each other. The purpose of the Domain Model is to establish a common understanding of the static aspects of the business domain amongst all stakeholders. The Domain Model supports the creation of quality requirements by establishing a common vocabulary across all stakeholders reducing ambiguity and redundancy.

As a result, the following guidelines should be considered:

-   The contents should be written in the business language of the domain and avoid implementation specific or technical aspects (such as operations or actions, which some presentations do not rule out): Use good business names!
-   Stakeholders should be comfortable with the chosen representation of the Domain Model (see below) in order to be able to provide feedback. As a result, multiple views on the domain model may be necessary for different stakeholders.
-   The domain model is developed in iterations where necessary details are enriched over time.

An obvious way to identify Domain Concepts is to identify nouns and phrases in textual descriptions of a domain. The information about the Domain Concepts can come from existing documentation, industry standard documents for a specific domain, and output from the requirements elicitation.

The Domain Model can be represented in different ways. The representation is dependent on the methodology and the formality employed in the project as well as the experience of the stakeholders exposed to the Domain Model. It can stretch from a Word document, an Excel table, diagrammatic representations to a fully detailed model representation using a UML class diagram.

The Domain Driven Design approach is an extension of the Domain Model to produce an implementation which is linked to an evolving model of the domain, it is appropriate for a highly complex domain and produces a highly maintainable system, the implementation can be by an Domain Specific Language.

The Use Case Model

A Use Case Model describes the proposed functionality of a new system. A Use Case represents a discrete unit of interaction between a user, called an Actor, (human or machine) and the system. This interaction is a single unit of meaningful work, such as Create Account or View Account Details. Each Use Case describes the functionality to be built in the proposed system, which can include another Use Case’s functionality or extend another Use Case with its own behavior.

The Use Case contains:

-   General comments and notes describing the use case.
-   Requirements – The formal functional requirements of things that a Use Case must provide to the end user, such as “Withdraw Money” in an ATM example. These correspond to the functional specifications found in structured methodologies, and form a contract that the Use Case performs some action or provides some value to the system.
-   Constraints – The formal rules and limitations a Use Case operates under, defining what can and cannot be done. These include:
    -   Pre-conditions that must have already occurred or be in place before the use case is run; for example, must precede
    -   Post-conditions that must be true once the Use Case is complete; for example,
    -   Invariants that must always be true throughout the time the Use Case operates; for example, an order must always have a customer number.
-   Scenarios – Formal, sequential descriptions of the steps taken to carry out the use case, or the flow of events that occur during a Use Case instance. These can include multiple scenarios, to cater for exceptional circumstances and alternative processing paths. These are usually created in text and correspond to a textual representation of the Sequence Diagram.
-   Scenario diagrams – Sequence diagrams to depict the workflow; similar to Scenarios but graphically portrayed.
-   Additional attributes, such as implementation phase, version number, complexity rating, stereotype and status.

The Use Case model shows how the Actors interact with the Use Cases.

Some other models used to capture functionality include:

-   **Life Cycles** – these are descriptions of the valid states in each Domain Concept’s “life”, along with the relationships between those states (e.g. legal transitions). It is important to note that such Life Cycles are related to a single Domain Concept (i.e. not to the system as a whole, one or more Use Cases, or the interaction of the system with the outside world ). Life Cycles are often referred to as State Machines or State Charts.
-   **Business Process models** – The use of Business Process Modelling (BPM) to represent the functionality of the enterprise is an alternative approach to developing software as fundamental concept is to develop the model in a tool which can then be used to produce an executable model. Each element has KPIs attached to it so it is frequently used as part of a performance improvement process.
-   **User Stories** – In agile projects user stories are used to capture requirements, these are short descriptions of how a particular user wants to interact with a system, in the form “As a I want to , so that . The user story includes a set of acceptance criteria which describe the boundary of the story and defines when it is done.
-   **Traceability Matrix –** To fill the need for traceability a traceability matrix can be produced. This can be as simple as a table which cross references the requirements to the software component that fulfils it, however this can become very hard to maintain, so it is more common to use a requirements management tools when this level of formality is required.

# Sub-Capabilities

## Requirements Definition

Understand the various activities which are undertaken as part of requirements definition and how to represent these in the appropriate way for the project, using models. The ability to review requirements and ensure they are of high quality, namely: unambiguous, concise, consistent, complete, implementable, verifiable, clear and testable.

| **Iasa Certification Level** | **Learning Objective**                                                                                                                                                                             |
|------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **CITA- Foundation**         | Learner will be able to name the main types of activities in the process of capturing requirements Learner will be able to name the key qualities for requirements                                 |
| **CITA – Associate**         | Learner will be able to describe the different types of requirements produced by different user groups Learner will be able to review requirements produced and provide feedback on their quality. |
| **CITA – Specialist**        | Learner will be able to point out gaps in requirements, not spotted by the analysts. Learner will be able to capture requirements for complex areas                                                |
| **CITA – Professional**      | Learner will be able to support the analysts in capturing high quality requirements by introducing new techniques.                                                                                 |

## Functional Requirements Modeling

This covers the production of the appropriate set of requirements models for different projects is varying domains, using the techniques described in the proven practices section. This activity links the system produced to the business benefits delivered by the the system.

| **Iasa Certification Level** | **Learning Objective**                                                                                                                                                                                                       |
|------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **CITA- Foundation**         | Learner will be able to name the main types of models used to capture requirements Learner will be able to describe what each of the models are used for                                                                     |
| **CITA – Associate**         | Learner will be able to review the models produced on the project Learner will be produce the models needed to describe simple systems.                                                                                      |
| **CITA – Specialist**        | Learner will be able to advise when it is most appropriate to use which model type on a project, and highlight the advantages and disadvantages of each Learner will be able to produce requirement models for complex areas |
| **CITA – Professional**      |  Learner will be able to coach business analysts in modeling techniques                                                                                                                                                      |

## Requirements Management

During the project life time the requirements need to be prioritized, kept up to date and have traceability captured and maintained. This not usually the job of the architect, but typically will get involved and may have to help with this activity.

| **Iasa Certification Level** | **Learning Objective**                                                                                                                                                                                             |
|------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **CITA- Foundation**         | Learner will be able to name the steps in a typical requirements management process Learner will be able to describe the purpose of traceability                                                                   |
| **CITA – Associate**         |  Learner will be able to define the appropriate steps in a requirements management process for a project Learner will be able to review the traceability for a project and provide constructive feedback           |
| **CITA – Specialist**        |  Learner will be able work with the stakeholders to establish the priorities of a set of requirements Learner will be able to construct a traceability model, with particular focus on handling quality attributes |
| **CITA – Professional**      |  Learner will be able to coach business analysts in requirements management techniques                                                                                                                             |

# Related Capabilities

-   [Requirements Discovery and Constraint Analysis](requirements_discovery_and_constraints_analysis.md){:target="_blank"}
-   [Traceability through the Lifecycle](traceability_throughout_the_lifecycle.md){:target="_blank"}
-   [Information Modeling](information_modeling.md){:target="_blank"}

# Resources

**Articles:**

-   Use Case Modelling; Kurt Bittner, Ian Spence; 2002; Addison-Wesley
-   Writing Effective Use Cases; Alistair Cockburn; 2000; Addison-Wesley
-   [Domain-Driven Design: Tackling Complexity in the Heart of Software](http://www.domaindrivendesign.org/books/evans_2003){:target="_blank"}, [Evans, Eric](https://en.wikipedia.org/w/index.php?title=Eric_Evans_(technologist)&action=edit&redlink=1){:target="_blank"} (2004), Addison-Wesley

**Blogs/Webcasts/News/Reference Resources:**

- [http://www.sparxsystems.com/resources/tutorial/use_case_model.html](http://www.sparxsystems.com/resources/tutorial/use_case_model.html){:target="_blank"}
- [http://agiledata.org/essays/agileDataModeling.html](http://agiledata.org/essays/agileDataModeling.html\#InitialDomainModel){:target="_blank"}
- [http://agiledata.org/essays/agileDataModeling.html](http://agiledata.org/essays/agileDataModeling.html\#InitialDomainModel){:target="_blank"}
- [http://martinfowler.com/bliki/UbiquitousLanguage.html](http://martinfowler.com/bliki/UbiquitousLanguage.html){:target="_blank"}
- [http://web.archive.org/web/20061220024049/http://mason.gmu.edu/\~tdufresn/paper.doc](http://web.archive.org/web/20061220024049/http://mason.gmu.edu/\~tdufresn/paper.doc){:target="_blank"}

**Training:**

**Certifications:**

## Author

## Chris Cooper-Bland  
*Group Head of Architecture – Endava*
