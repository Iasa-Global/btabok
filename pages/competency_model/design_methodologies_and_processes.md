---
title: "Design Methodologies and Processes"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: design_methodologies_and_processes.html
folder: competency_model
summary: "Design is a critical part of the process of architecture, and yet in much architecture the design process is not reflected in the final delivered architecture. "
tags:
 - design
---

# Description

All architecture is design, but not all design is architecture -- Design methodologies are a collection of methods, procedures, standards, tools, and recommended practices used for creating architecture and the more detailed design which flows from the architecture.

Architects are expected to be able to recognize major components of the process in various design methods and be able to determine when a given design method is appropriate to the problem at hand.

# Overview

Design is a critical part of the process of architecture, and yet in much architecture the design process is not reflected in the final delivered architecture. Many architectures are simply a collection of artefacts (mostly models of some form), which describe the end result of the design process.

So why is this a problem? -- While models are useful artefacts they only capture ***what*** was designed, and not ***why*** a specific design was created. Models do not capture the process of design. The value of design is in the reasoning, the traceability back to the business requirements, and the decisions which led to the creation of a particular architecture.

Good design is justifications, reasons, and trade off considerations -- Design is often confused with models or diagrams, in reality the diagrams are the output of the design process. Since a number of solutions could satisfy a business need, the reasoning behind picking one design over another is where the real value of architecture lies.

This highlights a key distinction between the process of architecture and architecture deliverables. Architecture is more than a checklist of deliverables which must be created, it must also include the "design narrative" which captures why decisions were made and how the deliverables relate to and inform each other. Models are critical for simplifying both software and the software process; Simple design focuses on delivering a system that balances delivering on the immediate needs while considering future needs.

Design Methods and Processes also have an impact on the architecture process in terms of the expected deliverables used to seed the detailed design process. Different methods will have different implications for the architecture process. In Agile Development, for example, the architecture may begin at a high level, then allow agile design/development to proceed in order to validate a particular element of the architecture prior to formally documenting the design.

Scale of a project also impacts design. In small-scale projects, there may be very little architecture and mostly design, however as project complexity increases the importance of up-front architecture grows. In large-scale enterprise projects the development of an overall architecture is an essential precursor to the initiation of design since it provides the context into which the design activities will deliver.

> **Models are not Design -- **Models without design provide an illusion of understanding -- Architects & support organizations need to understand why certain design decisions were made during the architecture process so that future enhancements to the solution can be made with awareness of all the relevant information. Without recording the design decisions future architects and support organization are doomed to infer or make assumptions about why a solution was designed in a particular way. This impacts both the ability to maintain and enhance the solution, and also the ability for others to reuse elements of the architecture. Documenting design rationale allows architects to evaluate whether an existing architecture component is suitable for inclusion in a different architecture.

> You can reverse engineer an architecture from an existing solution, but not the design intent -- Most architecture deliverables can be reverse engineered from a solution, however it is not typically possible to determine the reasons that design decisions were made, or the context in which those decisions were made (alternatives considered, constraints, alignment with principles etc.).

# Corporate Best Practices

-   Establish common design methods and processes with appropriate tooling support. The level of commonality that can be achieved will be dependent on organizational structure, for example highly federated organizations tend to have greater diversity as a consequence of their business model. As always, architecture must be linked to business value so uniformity for the sake of uniformity doesn't add value.
-   Develop a repository where design artefacts can be shared, discovered and reused by architects. This helps deliver value by allowing architects to discover and reuse content, or actively collaborate on the development of new content. Without this, there is a risk that multiple independent designs for the same problem will be developed across an organization.
-   Adopt and adapt industry standard design methods and processes in preference to "home-grown" alternatives -- the availability of training and tooling is a significant benefit to this approach, as is the ability to recruit suitably skilled individuals.
-   Subject matter experts and junior architects often have a tendency towards building over buying, and building over reusing existing IP. This can lead to unnecessary cost in new development and additional maintenance costs. A key part of the design process is the recognition of opportunities to reuse or purchase functionality over building your own. Architects provide a unique cross discipline view of the activities involved in projects, across the business and the technical areas. The key challenge here is identifying the appropriate approach required for each project and selling to the stakeholders, even when they hold a different view.

# Sub-Components Skills

## Application of Design Methods and Processes

Design requires the use of techniques, tools, patterns, methodologies, and a host of other tools to assist in providing predictable, repeatable success. Everybody has a bad day, and leveraging methods and processes helps architects to remember what they've forgotten to consider in an architecture.

There is both art and science in architecture, but leveraging methods and processes will help architects be effective at designing solutions.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will be able to name the various types of design methods and processes used by the current organization and understand what they are used for
| | -   Learner will be able to explain the design methodology or tool of choice
| **CITA -- Associate** | -   Learner will be able to use a number of design methods and processes
| | -   Learner will be able to explain the signs of poor design
| | -   Learner will be able to explain MDA (Model Driven Architecture) and its impact on the design process.
| | -   Learner will be able to explain how an architect applies design patterns and common design principles in the design process.
| | -   Learner will be able to name some principles and tenets that help delivering efficient designs.
| **CITA -- Specialist** | -   Learner will be able to articulate the value of good design process to business stakeholders.
| | -   Learner will be an expert in some of the design methods and processes, and be able to highlight the advantages and disadvantages of each
| | -   Learner will be able to explain how to design for operations
| | -   Learner will be able to explain how to focus on design simplicity and still meets customer's needs.
| **CITA -- Professional** | -   Learner will be able to drive the introduction of new design methods and processes into the organization
| | -   Learner will be able to act as a mentor for the design methods and processes
| | -   Learner will be able to measure or control the design quality on the project.

## Design Tools and Techniques

Architects will need to advise on the appropriate tools for each of the architecture and design activities, and they are expected to be involved in their selection and usage. The architect will guide the project on issues such as adoption of modeling techniques, for example the use of UML. The architect will assist and mentor the development team with modelling activities and will provide governance over the design review processes.

Methodologies and Concepts

-   Models are critical for simplifying both software and the software process.
-   Simple design focuses on delivering a system that balances delivering on the immediate needs while considering future needs.
-   There are multiple levels or concerns in software development
-   Do not mix modeling notations in the same concern
-   Each model should represent the same level of granularity

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will be able to name the various types of design tools and techniques used by the current organization and understand what they are used for
| | -   Learner will be able to understand design models and documentation.
| | -   Learner will be able to explain the design process
| | -   Learner will be involved in design reviews
| | -   Learner will be able to draw a sample design model used in the past
| **CITA -- Associate** | -   Learner will be able to use a number of the design tools and techniques
| | -   Learner will be able to participate in the design process
| | -   Learner will be able to carry out design reviews
| | -   Learner will be able to share experiences: e.g. is UML (or ArchiMate) a good visualization tool to support design process?
| **CITA -- Specialist** | -   Learner will be an expert in some of the tools and techniques and be able to highlight the advantages and disadvantages of each
| | -   Learner will be able to carry out design reviews on complex areas.
| | -   Learner can explain their level of concern on a project and how to design and model it.
| **CITA -- Professional** | -   Learner will be able to drive the introduction of new tools and techniques into the organization
| | -   Learner will be able to act as a mentor for the tools and techniques
| | -   Learner will be involved in defining the design review process and the checklists to be used.

# Related Capabilities

[Application Development](application_development.md){:target="_blank"}
Understanding of common Solution Development Lifecycles and the role/placement of design process within them.

[Whole System Design](the_whole_systems_design.md){:target="_blank"}
Additional concerns when designing complex architectures spanning multiple systems.

[Architecture Description](architecture_description.md){:target="_blank"}
Representing design outputs in a formal ADL (Architecture Design Languages)

[Design Patterns and Styles](design_patterns_and_styles.md){:target="_blank"}
Patterns provide a mechanism to document an approach that has been successfully used to solve a problem in the past

# Author

![Sean Gordon](media/s_gordon.jpg)
## Sean Gordon
*Technical Expert for Solution Architecture -- Chevron*


Sean Gordon works for Chevron (<http://www.chevron.com/>) where he is Technical Expert for Solution Architecture. He has over 25 years of IT experience including 10 years working for Microsoft as a consultant in Architecture and Enterprise Integration. His current focus is on developing Target Architectures for Chevron's various asset classes.

Sean is an Honorary Lecturer at Dundee University School of Computing (<http://www.computing.dundee.ac.uk/>). He is also a member of the judging panel for the ScotlandIS Young Software Engineer of the Year Awards (<http://www.scotlandis.com/>).
