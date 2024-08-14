---
title: "Software Architecture Development Methodologies and Processes"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: dmp.html
folder: competency_model
summary: "Regardless of the main focus of the method (artifacts, use cases, attributes, or domain), the architectural design process includes the following aspects."
---

# Description

A software-intensive system is any system where software contributes essential influences to the design, construction, deployment, and evolution of the system as a whole. Despite significant efforts to improve engineering practices and technologies, software-intensive systems continue to present formidable risks and difficulties in their design, construction, deployment, and evolution.

There is a general consensus on the importance of the architectural level of systems design, consisting of early decision making about overall design structure, goals, requirements, and development strategies. The architecture has different meaning for different stakeholders:

*   The specification of the system to be implemented (blueprint)
*   A medium of communication for achieving common understanding (a language)
*   A rationale for the choices about the system to be implemented
*   A documentation for current and future generations of users and developers of the acceptable practices (a narrative).

This multiplicity of views imply a need to describe the architecture from multiple complementary perspectives.

Broadly speaking the diverse software architecture development methods can be classified as:

*   Artifact driven methods: are defined in terms of the artifacts to be produced and the notations employed in their elaboration. Examples of this approach are the object oriented methods (such as OAD and OMT) with their emphasis on structural description of the system.
*   Use case driven methods: use the description of use cases as the primary artifact. Rational Unified Process and test (or compliance) driven processes exemplify this approach. Attribute driven methods use the quality attributes as the main driver for selecting one architectural option over others.
*   Domain driven methods: use concepts from the domain to drive the architecture definition. Domain analysis-based and product line-oriented methods like BAPO/CAFCR follow this approach.

# Overview

Regardless of the main focus of the method (artifacts, use cases, attributes, or domain), the architectural design process includes the following aspects

1.  Analysis of architecture requirements, identifying concerns, and providing context for decision making through the process
2.  Documentation of the desirable characteristics and supporting principles of the system and its evolution, to facilitate communicating them with the system’s stakeholders
3.  Evaluation and comparison of architecture alternatives in a consistent manner
4.  Verification of compliance of the actual system implementation with its architectural description
5.  Management of the evolution of the architecture.

# Proven Practices

*   Establish common design methods and processes across the organization, adapting them to the possibly different sub-organizations characteristic of large corporations. Traditional approaches tend to impose similar process to diverse teams regardless their sizes, and the characteristics of the system to be developed (e.g. internally versus externally developed systems). On the other extreme, so called “agile” methods leave to the teams the decision of what and how document architecture, if architecture was developed at all. More recently the “disciplined agile” approach looks for a middle ground balancing need for rigor with the need for agility.
*   Implement policies for ensuring the management of the software architecture throughout its full life cycle, including the periodic re-assessment of system goals and constraints and the evaluation of the architecture compliance, as well as the procedures to manage deviations.

# Sub-Capabilities

### **Architecture requirement analysis**

The Architecture requirement analysis is the process by which system’s goals and expected quality attributes are identified. Such requirements must be directly linked to business and mission goals, and explicitly involve system stakeholders.

One of the most important steps in analysis is the definition of the design context: where the final delivered system will fit into the current operational environment. The identification of stakeholders, system goals, and of scenarios and use cases all depend on how the boundaries are chosen.

Requirement elicitation can be done using diverse techniques such as the use of questionnaires and surveys, interviews, and analysis of existing documentation. Group elicitation techniques can be used to foster stakeholder buy-in and exploit team dynamics to elicit a richer understanding of needs and promote agreement among diverse stakeholders. Such techniques include brainstorming, focus groups, and consensus-building workshops. More formal methods also exist, which are based on a detailed model of the type of information to be gathered, such as quality attributes and their definition in terms of quality metrics.

*   **Iasa Certification LevelLearning ObjectiveCITA- Foundation**Learner will be familiar with the goals of the requirement analysis process
*   **CITA – Associate**Learner will be familiar with the techniques for requirement analysis
*   **CITA – Specialist** Learner will be capable of conducting requirement analysis processes to properly identify the context, goals and constraints of the system
*   Learner will be capable of assessing the quality of the requirement analysis results
*   **CITA – Professional** Learner will be capable of proposing a methodology for requirement analysis considering the organizational characteristics
*   Learner will be capable of proposing requirement analysis methods adapted to a particular problem domain or industry

### **Architecture synthesis**

This activity is the core of the architecture development process. It proposes solutions to the various concerns in terms of system organization patterns and development principles.

The description of the solution should be made from diverse viewpoints which reflect different concerns of the systems such as the mapping to problem domain and functional requirements, organization of development artifacts, runtime components and their behaviors, and mapping to the deployment infrastructure, among others. In order to be useful documented speciﬁcations have to be both suﬃciently detailed for analysis and adequately abstract for understanding.

It is desirable that the design process adopts a well defined architecture style, encapsulating important decisions about the architectural elements and emphasizes important constraints on the elements and their relationships.

The process is generally backed by a reference architecture that entails a set of best practices for the domain on which the system must operate. In certain industries and technology domains such reference architecture has been formalized. Some examples are the  [eTOM framework](http://www.cisco.com/c/en/us/products/collateral/services/high-availability/white_paper_c11-541448.html) for the telecommunications industry, and the [IOT-A reference architecture](http://www.iot-a.eu/arm/d1.3/at_download/file) for the Internet of Things domain.

*   **Iasa Certification LevelLearning ObjectiveCITA- Foundation**Learner will be familiar with the notions of architectural style, architecture pattern, reference architecture
*   **CITA – Associate**Learner will be capable to identify architectural styles and their attributes
*   Learner will be capable of identifying architectural patterns and their attributes
*   The learner will be capable of matching significant architectural decisions to relevant reference architecture
*   **CITA – Specialist** Learner will be capable of proposing architectural patterns to address specific concerns
*   Learner will be capable of using a reference architecture to guide the design process
*   **CITA – Professional** Learner will be able to evaluate the properties of proposed architecture styles and patterns
*   Learner will be able to propose a reference architecture for a problem domain

### **Analysis of alternative architectures**

The purpose of the analysis of a software system’s architecture is to verify that the quality requirements have been addressed in the design and identify to potential risks. Broadly speaking the evaluation methods can be classified as software metrics-based, scenario-based, and attribute model-based. The software metrics methods use module coupling and cohesion notions to identify potential quality issues. Methods based on scenarios focus on spotting requirement conflicts or incomplete design specification from a particular stakeholder’s perspective. Attribute model-based architecture evaluation methods focus on evaluating quality metrics. The evaluation techniques can be narratives, checklists, formal methods, simulation, or prototyping.

*   **Iasa Certification LevelLearning ObjectiveCITA- Foundation**Learner will be familiar with the notion of architecture quality attributes
*   **CITA – Associate**Learner will be familiar with the definition of different architecture quality attributes
*   Learner will be be capable of evaluating specific architecture quality attributes
*   **CITA – Specialist** Learner will be Be familiar with formal architecture evaluation methods
*   Learner will be capable of identifying relevant quality attributes for a system given its context and goals
*   **CITA – Professional** Learner will be capable of proposing an architecture evaluation methodology adapted to an organization’s context and system’s problem domain

### **Architecture compliance assessment**

A recurrent problem faced by software architects is to certify that a system is implemented according to its planned architecture. During the implementation and evolution of a system, it is common to observe deviations from the defined architecture, even in the first release, due to unawareness by developers, conflicting requirements, late changes in requirements, technical difficulties, and deadline or budget pressures. Such deviations usually accumulate with time, leading to the phenomena known as architectural erosion.

Architecture compliance is a measure to which degree the implemented architecture in the source code conforms to the planned architecture. For assessing the compliance, a model of the actual system must be created and compared to the architecture model, in order to identify violations such as unintended dependencies.

Alternatively, deviations from the intended architecture can be prevented by enforcing it through prescribed design patterns that offer well-established solutions to recurring design problems, following the architecture’s constraints, introducing frameworks whose architecture is aligned with the intended architecture, or using tools that generate architecture-compliant code.

*   **Iasa Certification LevelLearning ObjectiveCITA- Foundation**Learner will be familiar with the concept of architecture compliance and the sources of deviation from intended design
*   **CITA – Associate**Learner will be capable of assessing the compliance of a model for the actual system with the intended architecture
*   **CITA – Specialist** Learner will be capable of eliciting a model of the actual system implementation to assess its compliance with the intended architecture
*   Learner will be capable of proposing measures to prevent deviations of the actual system implementation from the intended architecture
*   **CITA – Professional** Learner will be capable of proposing tools and methods for eliciting the model of the actual system implementation to compare its compliance with the intended architecture
*   Learner will be capable of proposing policies and strategies to prevent and correct architecture erosion

### **Architecture evolution management**

A software system’s ability to easily accommodate future changes in business requirements, organizational context, and technology. It is a fundamental characteristic for increasing economic value of software and minimize technological risk in an organization. For long-lived systems, there is a need to address evolvability explicitly during the entire software lifecycle in order to prolong the productive lifetime of software systems.

*   **Iasa Certification LevelLearning ObjectiveCITA- Foundation**Learner will understand the importance of architectural evolvability
*   Learner will be familiar with the sources of evolution in a software architecture
*   **CITA – Associate**Learner will understand the software architecture attributes that are necessary to constitute an evolvable software system
*   Learner will be capable of Identifying the sources of change in an architecture
*   **CITA – Specialist** Learner will be capable of proposing measures for managing evolvability in the architecture
*   **CITA – Professional** Learner will be capable of proposing an policies and strategies for managing architectural evolution in an organization

# Related Capabilities

Requirements Modeling

Architecture Description

Software Quality Attributes

Software Stakeholder Management

Software Architecture Patterns

# Resources

### **Articles:**

Dobrica, L., & Niemelä, E. (2002). A survey on software architecture analysis methods. Software Engineering, IEEE Transactions on, 28(7), 638-653.

Hofmeister, C. , Kruchten, P., Nord, R.L., Obbink, H., Ran, A., America, P. A general model of software architecture design derived from five industrial approaches. The Journal of Systems and Software 80 (2007) 106–126

ISO/IEC 42010 IEEE Std 1471-2000 First edition – ISO/IEC Standard for Systems and Software Engineering – Recommended Practice for Architectural Description of Software-Intensive System. 2007

# Author

### 

![Pablo Chacin](media/pablo_chacin.jpg) 

**Pablo Chacin**

### CTO – Sensefields

I have more than 20 years of experience in the Information Technology industry and have been involved in software and technology architecture as consultant for large organizations primarily in the Banking, Telecommunications and Government sectors. I also have experienced in the academy, participating in several research projects and lecturing in subjects like operating systems, distributed systems, and performance evaluation .

I received a degree in Computer Sciences from the Central University of Venezuela in 1993, a Master degree in Information Technology Management from the ITESM, Mexico in 2004, and an a PhD in Computer Architecture at the Polytechnic University of Catalonia in 2011. In my PhD dissertation I proposed the design, implemented and evaluated a middleware for self-adaptive highly scalable web services.