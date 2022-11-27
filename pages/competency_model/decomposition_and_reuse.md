---
title: "Decomposition and Reuse"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: decomposition_and_reuse.html
folder: competency_model
summary: "Understanding how and when to decompose a system is an important design skill as it can have a significant impact on the cost of building and maintaining a system."
tags:
  - design
---

# Description

Decomposition involves the analysis of a design or system, deciding on how to divide it up and organise its structure with the objective of optimising several quality attributes such as maintainability, testability, flexibility and extensibility.

Reuse is facilitated by decomposition and involves identifying repetitive patterns or commonly used features, then decomposing those parts into separate components which can be reused multiple times. This type of decomposition results in a separation of concerns as the reusable component encapsulates a set of related features and exposes the functionality through a defined interface. Separation of concerns is an underlying principle of component based design and the basis of service orientated and micro service architectures.

# Overview

Understanding how and when to decompose a system is an important design skill as it can have a significant impact on the cost of building and maintaining a system.

Advantages of a decomposed system:

-   Reduction of overall system complexity, therefore it is easier to understand and maintain.
-   More effective testing, testing can be concentrated on individual components.
-   Components can be refactored, retested or even replaced with reduced risk.

Reusing components and patterns improves developer productivity and reduces maintenance costs. A common philosophy for describing reuse is [Don't Repeat Yourself](http://en.wikipedia.org/wiki/Don%27t_repeat_yourself){:target="_blank"}.

Advantages of reusable components:

-   All consumers of a reusable component will benefit from any future improvements, such as performance or reliability improvements.
-   Prototyping a new solution is faster and easier as large parts of the new system can be built from existing components.
-   It is easier for developers to move between projects in a large organization as they become familiar with common reusable components.

While there are several advantages to decomposing a system; careful consideration must be given to the following:

-   System performance, especially when introducing process boundaries.
-   Delivering value, decomposing a system and designing for reuse involves trade-offs and the process can be taken too far, for instance, care must be taken not to spend too much time designing and developing components which will never be reused.

# Sub-Components Skills

## Analysis and Execution of Decomposition

Whether decomposing for structure or for reuse, a good understanding of the design or system is obviously a prerequisite. It is useful to review all existing documentation and specifications before you start your analysis.

**Decomposing for Structure:**

-   Analyse the overall structure of the design or system.
-   Decide on a desired structure, at a high level i.e. n-tier architecture.
-   Divide up each section of the high level structure into groupings of related objects, services or operations.
-   Create models or diagrams which represent the structure, using a consistent and descriptive naming convention for components, classes etc.
-   Add details to the design documentation, explaining the decisions made.

**Decomposing for Reuse:**

-   Analzse the design or system, taking note of how often a particular pattern of logic appears.
-   If the pattern count is greater than two or three then this is a candidate for reuse.
-   Design an interface which satisfies all occurrences of the pattern, this requires a good understanding of the different contexts of use and possible future uses.
-   Design the reusable component or choose a pre-built component. (see "Pre-Built Component Selection" and "Reusable Component Design" sections below).
-   Add details to your component catalog, explaining the design decisions made and how the component should be used.

**Refactoring Existing Systems**

When the decomposition analysis and design work has been completed on an existing system you should proceed with planning the refactoring work, creating estimates for the effort required. Refactoring work is generally carried out as part of broader project and it will therefore have an impact on the resources and timelines for that project. In order to get stakeholder buy-in ensure that the benefits of the work are outlined clearly.

The structure of the code can change significantly during this refactoring exercise therefore it must be planned carefully so that it does not disrupt other development on the same code base.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will be able to describe the basic concepts of decomposition and reuse.
| | -   Learner will be able to outline the benefits of decomposition and reuse
| **CITA -- Associate** | -   Learner will be able to analyze an existing design or system and identify where decomposition would be beneficial.
| | -   Learner will be able to analyze an existing design or system and identify a section which can be refactored for reuse.
| **CITA -- Specialist** | -   Learner can design a system with reuse in mind.
| | -   Learner will be able to formulate a plan for decomposing a design or system.
| | -   Learner will be able to demonstrate where decomposition and reuse are beneficial.
| **CITA -- Professional** | -   Learner will be able to mentor developers and assess whether decomposition has been applied correctly or taken too far.
| | -   Learner will be able to evaluate the cost benefit of a decomposition and refactoring exercise.

## Pre-Built Component Selection

The use of pre-built components, either commercial or open-source can significantly reduce the overall cost of a project and reduce the time-to-market. Analyzing a system for decomposition is also an opportunity to identify where pre-built components can be utilized. If a pre-built component is the product of a well established project then the code will have been well tested, tuned for performance, documented with examples and have an active support community.

Poor selection of pre-built components can have a negative impact on a project therefore careful consideration must be given to licensing, compatibility, interoperability, support, end-user environments etc. Examples of common pre-built components include data access & [ORM](http://en.wikipedia.org/wiki/Object-relational_mapping){:target="_blank"} frameworks, logging components, messaging middle-ware and [business rules engines](http://en.wikipedia.org/wiki/Business_rules_engine){:target="_blank"}.

**The Dependency Inversion Principle\
**

When using pre-built components it is generally advantageous to apply the [dependency inversion principle](https://en.wikipedia.org/wiki/Dependency_inversion_principle){:target="_blank"}{:target="_blank"} by adding a layer of abstraction between your system and the pre-built component. By defining and coding against your own interface it is easier to replace a pre-built component at a later date. In this scenario the only code which needs to change is the code in the abstraction layer.

For example, imagine we sell several applications to enterprise customers and our applications communicate via asynchronous messaging middle-ware. We have decided to use [AMQP](http://en.wikipedia.org/wiki/Advanced_Message_Queuing_Protocol){:target="_blank"} based messaging and have chosen a particular enterprise messaging system. To create an abstraction layer we have developed some wrapper code around the AMQP messaging client so that the systems using the component are not coded directly against the vendors client component.

Taking this example a step further we can set-up our abstraction layer to load the messaging wrapper by using [Dependency Injection](http://en.wikipedia.org/wiki/Dependency_injection){:target="_blank"}. If our next customer wants to leverage their existing [JMS](http://en.wikipedia.org/wiki/Java_Message_Service){:target="_blank"} messaging middle-ware instead of the AMQP messaging middle-ware then we can load a JMS messaging client via dependency injection without having to modify our system. This approach can make our systems more vendor agnostic although it does require some extra design and planning and may also require some compromise on features as a common set of features must be found across all interfaced components. This example is an implementation of the [Adapter Pattern](https://en.wikipedia.org/wiki/Adapter_pattern){:target="_blank"}.

**Package Managers**

[Package managers](http://en.wikipedia.org/wiki/Package_manager){:target="_blank"} provide an easy way to add pre-built components to your project. They will save you time but they can also lead to problems as it is extremely easy for a developer to add a new pre-built component to a project without understanding the full impact of the decision. For instance, adding a package to a web based solution may add a nice feature but it can also add a lot of bloat in the form of large JavaScript and CSS files, most of which may never be utilized by the project.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will be able to discuss the advantages of using pre-built components.
| | -   Learner will be able to identify where a pre-built component could be used.
| **CITA -- Associate** | -   Learner will be able to evaluate several pre-built components, listing the pro's and con's of each.
| | -   Learner will be able to explain why a poorly selected component is unsuitable.
| | -   Learner will be able to design an abstraction layer for a pre-built component.
| **CITA -- Specialist** | -   Learner will be able to perform a detailed analysis of costs, compatibility, interoperability etc.
| | -   Learner will be able to design a system where pre-built components can be replaced easily.
| **CITA -- Professional** | -   Learner will be able to mentor developers in pre-built component selection and explain how to choose the correct component.

## Reusable Component Design

Designing, developing and testing a reusable component is a strategic investment, a return on that investment will not be realised until the component has been used multiple times. When deciding to design a new component you must ensure that there are enough use cases to justify your decision.

Reusable component design is similar to any other design task, for more information see the "[Design Methodologies and Processes](design_methodologies_and_processes.md){:target="_blank"}" capability.

**Design Considerations:**

-   The initial design of a reusable component requires more time compared to the design of a single use component.
-   Configuration options must be added to cater for existing and future use cases.
-   Care must be taken not to over-design a component by adding features and configuration options which will never be used, aim for simplicity.
-   Reusable components can be developed in various forms, including but not limited to; component libraries, services, extensions, plugins or mixins.
-   Reusable components and their interfaces should be given generic names so that they do not feel out of place in future projects.
-   Since reusable components are used by multiple systems the code often lives longer than other system code, ensure the code well structured and easy to read so that it can be maintained by your successor.
-   Extra resources will be required for the initial development and testing.

Reusable components must be documented in detail so that developers wishing to use the component in the future will understand all of its features, configurations and limitations. Publishing a searchable component catalog is a very important part of making other architects and developers aware of their existence. Wiki's are a good way to document and publish these details as it is easy to search and to cross reference relevant sections. Developers can also add extra details and examples of usage scenarios or limitations.

Presenting and demonstrating reuse to the development team is an opportunity to inform others about the catalog of available components, so that they understand the benefits and can recognize when a reusable component should be used. A Lunch & Learn session is a good way to discuss reusable components, it is useful to get input from others, to discuss improvements and possible alternatives.

| **Iasa Certification Level** | **Learning Objective** |
| :-: | :-: |
| **CITA- Foundation** | -   Learner will be able to describe the design considerations of reusable component design.
| | -   Learner will be able to explain why cataloging reusable components is important.
| **CITA -- Associate** | -   Learner will be able to explain why a reusable component should be developed.
| | -   Learner will be able to review a catalog of reusable component and select a suitable component.
| **CITA -- Specialist** | -   Learner will be able design a reusable component taking future use cases into consideration.
| | -   Learner will be able to document and publish details of reusable components.
| | -   Learner will be able to present on reusable components and explain how and when they should be used.
| **CITA -- Professional** | -   Learner will be able to assess whether the documentation in the component catalog is of sufficient detail.
| | -   Learner will be able to mentor others on reusable component design and how to document and present details of reusable components.

# Related Capabilites

-   [Architecture Description](architecture_description.md){:target="_blank"}
-   [Whole System Design](the_whole_systems_design.md){:target="_blank"}
-   [Design Methods & Processes](design_methodologies_and_processes.md){:target="_blank"}
-   [Design Patterns & Styles](design_patterns_and_styles.md){:target="_blank"}

# Resources and Further Reading

-   [Decomposition in Computer Science](http://en.wikipedia.org/wiki/Decomposition_%28computer_science%29){:target="_blank"} (Wikipedia)
-   [Code Reuse](http://en.wikipedia.org/wiki/Code_reuse){:target="_blank"} (Wikipedia)
-   [Reusability](http://en.wikipedia.org/wiki/Reusability){:target="_blank"} (Wikipedia)
-   [Don't Repeat Yourself](http://en.wikipedia.org/wiki/Don%27t_repeat_yourself){:target="_blank"} (Wikipedia)
-   [Separation of Concerns](http://en.wikipedia.org/wiki/Separation_of_concerns){:target="_blank"} (Wikipedia)
-   [Software Reuse 101: What Is Software Reuse?](http://lombardhill.com/articles/software-reuse-101-what-is-software-reuse/)

# Author

![Declan Bright](media/declan_bright.jpg)
## Declan Bright 
*Chief Software Architect*

Declan Bright is a Chief Software Architect based in Dublin, Ireland. He has worked in the IT industry since 1999, primarily within the aviation, telecommunications and financial services sectors and has extensive experience in the design and implementation of enterprise solutions. Areas of specialisation include system integration, system evolution, user experience and analytics.  [www.declanbright.com](http://www.declanbright.com)
