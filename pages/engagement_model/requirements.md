---
title: "Requirements"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: requirements.html
folder: engagement_model
summary: "Requirements are recognized and developed throughout the entire portfolio of the enterprise."
tags: 
  - operating_model
---

> "The vast majority of ‘requirements’ are not required for value. They are really more about the preferences of a single system user. Start learning value management over user preferences now for better systems."
**Paul Preiss**

# Architecturally Significant Requirements

Architecturally significant requirements is a term used in the BTABoK to describe a set of concepts which relate to the development and delivery of value to an organization. Architecturally significant requirements can be broken into several different factors, depending on how the [engagement model](engagement.md){:target="_blank"} is implemented.

Requirements are recognized and developed throughout the entire portfolio of the enterprise. The goal of which is to represent value streams across the enterprise and to trace those value streams through the decision making process. Traditional architecturally significant requirements are mapped to innovation and ideation, business case development, project and or product requirements, epics and stories. And represent needs from both business and technology leadership.

For the purpose of the BTABoK, all thinking, ideas and desires about a business or technology system can be characterized as requirements, though depending on the full engagement model in use by an organization they may be called other names and use other format. 

![Figure_1](media/requirements001.png)

## Description

Architectural requirements are hard to determine, primarily because they need to be gathered so early in the lifecycle before details are known. Many organizations continually add detail and refinement to ASRs through the enterprise lifecycle with a common architecture goal of value traceability in decision making. Architects should start early in project life-cycles based on when an architect engages in a project, with the end goal being integration into the innovation and project/product funding lifecycle itself.

ASR representation in the [lifecycle](architecture_lifecycle.md){:target="_blank"}.

|  Characteristic       |  Explanation                                     |
|--------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Innovation/Ideation**  | ASRs are represented as ideas and characteristics according to the innovation cycle. These are funneled either into experimentation or into a business case by a value stream owner. All ASRs at this level are considered architecturally relevant.                         |
| **Business Case**        | ASRs are represented as course-grained ideas with the goal of understanding program cost or value generation. Traditionally these are used for rough scoping purposes to satisfy budget and staffing needs. Most ASRs at this level are considered architecturally relevant. |
| **Epic/Solution Story**  | For details on Epic and Story level integration with ASRs see the Lean and Agile Integration. Some ASRs at this level are considered architecturally relevant.                                                                                                               |
| **Detailed Requirement** | Few ASRs at this level are considered architecturally relevant though it is necessary for the architect to continuously review to ensure identification of architectural impact.                                                                                             |

Either way at some point the solution architect and business architect and will have to begin extracting relevant architectural requirements. So what exactly are ‘relevant’ requirements?

The BTABoK simplifies the guidelines for identifying ASRs. There are three primary types of requirements which will be important to your architecture design decisions.

## Types of Requirements

Requirements are typically placed into these categories:

-   Functional requirement ─ Describe the functionality that the system is to execute; for example, formatting some text or modulating a signal. They are sometimes known as features.
-   Non-functional requirements ─ Are the ones that act to constrain the solution. Nonfunctional requirements are known as quality attribute requirements.
-   Constraint requirements ─ Are the ones that act to constrain the solution. No matter how the problem is solved the constraint requirements must be adhered to.

## Architectural Relevance

Much work has gone into what makes a requirement significant to an architect. The SEI paper on the subject written by IBM provides significant detail on the subject. The literature suggests many categories of impacts which make a requirement relevant or not. However the thing that makes a requirement relevant is when an architect thinks it is.

The following describe categories of impact which potentially make a requirement relevant to the architecture.

1.  Requirements which deeply impact relevant product or frameworks within the business and technical roadmap.
2.  Requirements which impact managed quality attributes.
3.  Requirements which impact capabilities of the organization or the roadmap.
4.  Requirements which are deeply political or have an executive champion.
5.  Requirements which imply innovative business models or approaches.

> "The vast majority of ‘requirements’ are not required for value. They are really more about the preferences of a single system user. Start learning value management over user preferences now for better systems."
**Paul Preiss**

Architects are(n’t) engineers (btabok principle), which impacts the level and type of requirements to help understand critical design decisions but doing so based on best case overall value. Define what makes for a relevant architecture decision. Although this is a complicated topic in more mature environments which should use a calculation based on strategic importance.

## Architectural Structural Impacts

What is an architecturally significant component? This is a full article in its own right but for the sake of clarity let’s define it as a component that should be decided by the architect of a project instead of another stakeholder such as development, operations or business stakeholder.

A significant architectural component is controlled by two decisions. One decision is controlled by architectural complexity but can be decided based on total cost of ownership. This may be an application server, a new type of client we will support, an ESB or a rules engine, but it is definitely not a minor development pattern such as singleton or even minor component frameworks. The other type of decision is strategic importance. If we have done our jobs as architects we will have a target state architecture. Architectural component decisions that move us closer to our target state architecture are also significant at the project level.

When you are in the process of design you should gather any requirements that lend themselves to decisions about architecturally significant components. This is a skill that most seasoned architects take for granted since after many projects you will get a sense for these that is almost a bit like a ‘Spider Sense’.

## Quality Attribute Impacts

Another area of requirement decisions are those that deeply impact [quality attributes](quality_attributes.md){:target="_blank"}. Often called the ‘\~ilities and \~illiancies’ of a system, these are the horizontal cross-cutting concerns that impact a system such as performance, security, usability, RAS, and flexibility. During a requirements gathering phase the architect should be deeply alert for any requirement or idea that impact one of these items and should illicit requirements that allow for measurement of effective quality attributes. A great tool for the practicing architect is to build a set of questions which have definite impact on quality attributes and can be measured. Here are a couple of examples from my own practice:

-   “How many concurrent users do we need to support and in what portions of the system?”
-   “How flexible and decoupled should the system be? Which functional components will change often over time?”

## Technical Capability Impacts

One of architectures key roles is the understanding and management of technology capability impacts from both business and technology requirements. During the implementation of the engagement model the architecture team should determine what level of capability impact makes a requirement architecturally significant. These impacts can be compared with resource utilization, time impacts, business capability impacts, cost of delay, financial cost or value numbers based on the chosen value management implementation.

## Political and Stakeholder Impacts

Realistically certain requirements represent preferred capabilities, features or value perceived by a relevant or powerful stakeholder. These requirements become architecturally significant from a political and organizational perspective. Generally the higher the power or influence of a stakeholder the more relevant their preferred requirements will become.

## Incremental Business Innovation

The final type of architecturally significant requirement often comes from the architects themselves. These are technical capabilities that allow for incremental innovation in projects close to the customer. For example, if we are building a web interface to our system, could this be extended to a mobile application? If so, how beneficial would that mobile usage be to our organization? Often architects and project members identify innovative components which do not deeply impact a project scope or timeline. Even if they do, these ideas form the opportunity to innovate in the next round of projects or innovative ideation.

## Characteristics

Architectural requirements generally do no match detailed requirements specifications. Instead the following chart identifies areas of importance for ASRs.

| Characteristic |  Explanation                                                                                                                            |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------|
| **Complete**       | The requirement is fully stated in one place with no missing information.                                                                  |
| **Traceable**      | The requirement meets all or part of a business need as stated by stakeholders and authoritatively documented.                             |
| **Current**        | The requirement has not been made obsolete by the passage of time.                                                                         |
| **Verifiable**     | The implementation of the requirement can be determined through one of four possible methods: inspection, demonstration, test or analysis. |
| **Valuable**       | The implementation of the requirement can demonstrate measurable value to one or more areas of the organization.                           |


![image001](media/by-nc.png)

BTABoK 3.0 by [IASA](https://iasaglobal.org/) is licensed under a [Creative Commons Attribution-NonCommercial 4.0 International License](http://creativecommons.org/licenses/by-nc/4.0/). Based on a work at [https://btabok.iasaglobal.org/](https://btabok.iasaglobal.org/)