---
title: "Architecture Description"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: architecture_description.html
folder: competency_model
summary: "Architects are expected to be familiar with different Architecture Description Languages (ADLs) and to be capable of determining when specific elements of an ADL are required to deliver value to the project at hand."
tags:
  - design
---

# Description

The Architecture Description describes the architecture of a system (or systems), and provides detailed architecture communication, includes diagramming notation, architecture views and viewpoints. The goal of the Architecture Description (AD) is to transform the collected and organized architectural information and intents into viable models, describing the functional and non-functional requirements of the architecture. The Architecture Description also captures the principles which guide the development of the architecture, significant architecture decisions and acts as a repository of knowledge for the architecture of a system.

Architecture Descriptions are generally expressed in a formal Architecture Description Language (ADL), such as UML; or in a more informal "boxes and connectors" style of language.

Architects are expected to be familiar with different Architecture Description Languages (ADLs) and to be capable of determining when specific elements of an ADL are required to deliver value to the project at hand. The architecture domains covered in the Architecture Description, and the level of detail contained will vary according to factors such as the complexity of the project, the scope and the SDLC to be employed to deliver the solution.

# Overview

The ability to clearly and concisely describe (and document) the architecture for a solution is a key skill for architects, since the Architecture Description forms the "common language" by which the technical team gains a consistent understanding of the system to be delivered; additionally the Architecture Description is the starting point for other views and perspectives which may need to be created to communicate to other (non-technical) stakeholders. Another important role of the AD is to quickly and consistently bring new members of the technical team up-to-speed with the architecture of the system; as such the AD must be maintained during the SDLC to ensure it reflects the current state of the architecture for the system.

The AD provides detailed architecture communication and acts as a repository of architecture decisions for current and new team members, and for future maintainers of the solution -- "If it's not documented it doesn't exist". Architects should not underestimate the level of writing and communication skills necessary to be able to clearly and concisely communicate complex in a clear and understandable manner, since much of a typical AD is made up of narrative text.

Architects must be capable of delivering Architecture Descriptions in the preferred ADL of an organization, and to guide the selection of an appropriate ADL if necessary. The Architect must be able to apply judgment with regard to the level of rigor required for a particular project and the level of detail that the AD must deliver to support the needs of the solution through the entire SDLC. The process of Architecting is contingent on the application of experience and knowledge, not simply following a prescribed set of deliverables -- all elements of the AD must add value and contribute to the success of the solution during the relevant phases of the SDLC. As such, the architect must be aware of the purpose and value of each component of the architecture description and be able to recognize (and justify) when to utilize (or not) each component of the AD.

Architecture description is the end-product of an architecture development process that begins with exploring and understanding the context within which a technology solution will be deployed (e.g., business architecture, business drivers, stakeholder concerns), constraints and risks, vision for and purpose of the system, its goal(s), and relevant usage scenarios. The Architecture Description will not contain only models, but also textual and other artifacts which provide context and background to the models, in addition to providing an overall "design narrative" for the architecture.

The AD should support the necessary views and perspectives needed to satisfy the requirements to both model the solution, and communicate the architecture to the key stakeholders (not just technologists). For example, a successful AD should:

-   Be suitable for communicating architecture to all interested parties.
-   Support the tasks of architecture creation, refinement, and validation.
-   Provide a basis for further implementation -- so it must be able to add information to the AD to enable the final system specification to be derived from the AD.
-   Provide the ability to represent most of the common architectural styles.
-   Support analytical capabilities or provide quick generating prototype implementations.
-   Provide Architecture vision and views
    -   **Conceptual Descriptions and Notations** -- Standard notations for representing architectural concepts that help promote mutual communication and understanding of high-level ideas, sketches and solution concepts.
    -   **Logical Descriptions and Notations** -- Notations and descriptions that promote the embodiment of early design decisions, and creation of a transferable abstraction of a system, comprised of components and connections among them.
    -   **Implementation Descriptions and Notations** -- Specific, concrete and implementation-ready descriptions of envisioned system that allow analysis, feasibility testing and implementation of architectural design decisions.
-   Summarize major competitive products
-   Provide an analysis of pros/cons in features and in technical implementations
-   Document patterns used
-   Document principles
-   Explicitly state known constraints and risks
-   Describe value to the business
-   State existing standards and strategies which will guide the development of the architecture

# Corporate Best Practices

-   Adopt industry standards wherever possible -- the easy availability of tooling and training is a significant benefit.
-   When adopting a standard AD, resist the urge to customize too much in the early phases of the adoption. Early customization requests often come from poor understanding. Grow maturity before adapting a standard.
-   Establish and formalize your architecture review process early.
-   The contents of the AD must add value to some part of the solution process:
    -   Balance the level of rigor required in your AD with the needs of your organization.
    -   Consider varying the rigor of your AD with project complexity and risk.
-   Architecture Description should be developed by a single architect or a small cohesive team of architects to ensure that the vision is coherent & consistent.
-   Adapt to fit the needs of your organization -- Even when adopting AD & ADL standards organizations may need to adapt and modify to suit pre-existing architecture work, or to better support the way the particular organization operates.
-   Connecting with Stakeholders
    -   The architecture will be more acceptable to a stakeholder if reflected from their view point.
    -   Create different models and views for the same concepts to suit people in different roles, responsibilities, and background

# Sub-Components Skills

## Architecture Description Languages

An Architecture Description Language (ADL) is a notation for representing architectures with the purpose of capturing the output of the architecture design process, aiding communication with stakeholders and capturing a model of the system. ADLs can be formal or informal, and typically consist of "box and line" style diagrams although textual ADLs exist. For further information on ADLs see the Resources section at the end of this topic.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will be able to describe the audience for conceptual, logical, and implementation diagrams.
| **CITA -- Associate** | -   Learner will be able to explain the design flow from conceptual to implementation description of architecture artifacts.
| | -   Learner will be able to explain how to transform collected architectural information and intents into viable models.
| | -   Learner will be able to depict functional requirements of the architecture.
| | -   Learner will be able to explain the vocabulary of their preferred Architecture Description Language (ADL).
| **CITA -- Specialist** | -   Learner will be able to compare interests of target audience for conceptual, logical and implementation descriptions of architecture.
| | -   Learner will be able to describe as-is and to-be architecture and how to notate the gaps.
| | -   Learner will be able to compare and contrast ADLs such as UML and ArchiMate (or an internal/corporate ADL).
| **CITA -- Professional** | -   Learner will be able to describe how to create/adopt effective architecture approaches, methodologies, or reference models.
| | -   Learner will be able to drive the introduction of new ADLs and AD processes, tools and techniques into the organization.
| | -   Learner will act as a mentor for the AD tools, processes and techniques.
| | -   Learner will speak publically and contribute to the development of AD processes & techniques and ADLs.

## Architecture Tools & Techniques

Architects will need to advise on the appropriate tools & techniques to support the development and management of Architecture Descriptions, and participate in their evaluation and selection. The architect will guide the project on the adoption of architecture tools and techniques, and provide assistance and mentoring to the team as required.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will be able to name the various types of tools and techniques used in the current organization and understand what they are used for.
| | -   Learner will be involved as an observer in project Architecture review to understand of the elements of an architecture review and their role in the process.
| | -   Learner will be able to understand and explain the Architecture Descriptions developed for projects within the organization.
| **CITA -- Associate** | -   Learner will be able to use a number of the tools and techniques
| | -   Learner will participate in project architecture reviews within the organization, and will understand the role of the architecture review in the organizations' governance processes.
| **CITA -- Specialist** | -   Learner will be expert in a number of the tools and techniques, and be able to highlight the advantages and disadvantages of each.
| | -   Learner will lead the review of Architecture Descriptions for projects within the organization.
| **CITA -- Professional** | -   Learner will be able to participate in the evaluation and selection of new tools and techniques into the organization.
| | -   Learner will mentor others in the development and review of Architecture Descriptions
| | -   Learner will be leading the definition of the architecture review process for Architecture Descriptions within the origination.

# Related Capabilities

-   [Requirements Modeling](requirements_modeling.md){:target="_blank"}
-   [Views and Viewpoints](views_viewpoints.md){:target="_blank"}
-   [Design Patterns and Styles](design_patterns_and_styles.md){:target="_blank"}
-   [Whole Systems Design](the_whole_systems_design.md){:target="_blank"}
-   [Design Methods and Processes](design_methodologies_and_processes.md){:target="_blank"}
-   [Software Architecture Tools](software_at.md){:target="_blank"}
-   [Writing Skills](writing_skills.md){:target="_blank"}

# Resources

## Architecture Description

-   ISO/IEC/IEE 42010 "Systems and software engineering -- Architecture description"
    (supersedes IEEE 1471) -- [https://standards.ieee.org/findstds/standard/42010-2011.html](https://standards.ieee.org/findstds/standard/42010-2011.html){:target="_blank"}
-   Architectural Blueprints -- The 4+1 View Model of Software Architecture -- [http://www.cs.ubc.ca/~gregor/teaching/papers/4+1view-architecture.pdf](http://www.cs.ubc.ca/~gregor/teaching/papers/4+1view-architecture.pdf){:target="_blank"}
-   Software Systems Architecture, Rozanski & Woods -- [http://www.viewpoints-and-perspectives.info](http://www.viewpoints-and-perspectives.info){:target="_blank"}
-   Documenting Software Architectures -- Views and Beyond, Clements et. al. -- [http://www.amazon.com/Documenting-Software-Architectures-Beyond-Engineering/dp/0321552687](http://www.amazon.com/Documenting-Software-Architectures-Beyond-Engineering/dp/0321552687){:target="_blank"}

## Architecture Description Languages

## Architecture Description Languages ("Mainstream")

Architecture Description languages are still largely a research activity with only 2 languages really considered "mainstream", with UML an established and generally accepted "lingua franca" of software design, and ArchiMate being a recently emerging but widely supported ADL.

-   UML -- [http://www.uml.org](http://www.uml.org){:target="_blank"}
-   ArchiMate -- [http://www.opengroup.org/subjectareas/enterprise/archimate](http://www.opengroup.org/subjectareas/enterprise/archimate){:target="_blank"}

## Architecture Description Languages ("Experimental")

There are a large number of less well known and less well supported ADL, including those below. When considering the selection of an ADL it is important to take into account the level of adoption and tool support available for that ADL. Unless you operate in a very specialized domain it is likely that one of the mainstream ADLs will meet your needs, in addition to having readily accessible training and tool support.

-   xADL -- [http://isr.uci.edu/projects/xarchuci/](http://isr.uci.edu/projects/xarchuci/){:target="_blank"}
-   ACME / ADML (CMU/USC) -- [http://www-2.cs.cmu.edu/~acme/](http://www-2.cs.cmu.edu/~acme/){:target="_blank"}
-   Rapide (Stanford) -- [http://complexevents.com/stanford/rapide/](http://complexevents.com/stanford/rapide/){:target="_blank"}
-   Wright(CMU) -- [http://www.cs.cmu.edu/~able/wright/](http://www.cs.cmu.edu/~able/wright/){:target="_blank"}
-   Unicon (CMU) --
-   ByADL (Build Your ADL) -- University of L'Aquila -- [http://byadl.di.univaq.it/](http://byadl.di.univaq.it/){:target="_blank"}
-   LePUS3 and Class-Z (University of Essex) -- [http://lepus.org.uk/](http://lepus.org.uk/){:target="_blank"}
-   ABACUS (UTS) -- [http://www.avolution.com.au/](http://www.avolution.com.au/){:target="_blank"}

# Author

![Sean Gordon](media/s_gordon.jpg)
**Sean Gordon**
*Technical Expert for Solution Architecture -- Chevron*

Sean Gordon works for Chevron [http://www.chevron.com/](http://www.chevron.com/){:target="_blank"} where he is Technical Expert for Solution Architecture. He has over 25 years of IT experience including 10 years working for Microsoft as a consultant in Architecture and Enterprise Integration. His current focus is on developing Target Architectures for Chevron's various asset classes.

Sean is an Honorary Lecturer at Dundee University School of Computing [http://www.computing.dundee.ac.uk/](http://www.computing.dundee.ac.uk/){:target="_blank"}. He is also a member of the judging panel for the ScotlandIS Young Software Engineer of the Year Awards [http://www.scotlandis.com/](http://www.scotlandis.com/){:target="_blank"}.

